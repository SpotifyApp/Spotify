Data | Responsável | Versão| Modificações |
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   | Criação do caso de uso |
27/05/2018 | Geovanne Santos |   2.0   | refatorar o fluxo alternativo e básico, criação das regras de negócio |

# ✅ [UC06] - Adquirir o plano premiun

## 1. Nome do Caso de Uso
- Adquirir o plano premiun

## 2.  Breve descrição
- O usuário deseja comprar o plano premiun, para ter acesso a mais funcionalidades.

## 3.  Atores
- Usuário free.

## 4.  Pré-Condição
- O usuário deve possuir uma conta free no spotify.
- Ter o aplicativo do Spotify instalado.
- Estar conectado à internet.
- Ter feito o login no aplicativo.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O usuário instala o spotify.
2. O usuário abre o aplicativo.
3. O sistema direciona pra página de início da conta.
4. O usuário acessa a página de experimentar conta premium.
5. O sistema direciona o usuário para página de colocar informações de compra.
6. O usuário aceita o contrato padrão de plano premium que deseja firmar e a forma de pagamento padrão, que é o cartão de crédito.
7. O usuário coloca as informações necessárias.
8. O sistema valida as informaçoẽs.
9. O sistema muda a conte de tipo free para tipo premium.

## 5.2 Fluxos alternativos

FA01 - O usuário deseja adquirir o plano premium estudantil
1. O usuário instala o spotify.
2. O usuário abre o aplicativo.
3. O sistema direciona para página de início da conta.
4. O usuário acessa a página de experimentar conta premium.
5. O sistema direciona o usuário para página de colocar informações de compra.
6. O usuário acessa a página de planos premiun alternativos.
7. O sistema direciona para a página de tipos de plano premiun.
8. O usuário escolhe o plano premium estudantil, aceita o contrato, esolhe a forma de pagamento US[] e coloca as informações necessárias.
9. O sistema valida as informações.
10. O sistema muda a conte de tipo free para tipo premium.

FA02 - O usuário deseja adquirir o plano premium familiar e dividir o preço do plano com várias pessoas
1. O usuário instala o spotify.
2. O usuário abre o aplicativo.
3. O sistema direciona pra página de início da conta.
4. O usuário acessa a página de experimentar conta premium.
5. O sistema direciona o usuário para página de colocar informações de compra.
6. O usuário acessa a página de planos premiun alternativos.
7. O sistema direciona para a página de tipos de plano premiun.
8. O usuário escolhe o plano premium familiar, aceita o contrato, escolhe a forma de pagamento US[] e coloca as informações necessárias.
9. O sistema valida as informações.[FE02][FE01]
10. O sistema muda a conte de tipo free para tipo premium.

## 5.3 Fluxos de Exceção
FE01 - Não ter acesso a internet durante a tentativa de adquirir um pacote premium
1. Aplicativo perder conexão com a internet
2. O sistema não abre a página de colocar informações de contrato.
3. O sistema permanece na página anterior com a mensagem de erro[M2].

FE02 - O usuário entra com as informações de estabelecer contrato premium inválidas:
1. O sistema identifica a informação inválida .
2. O sistema permanece na mesma página.
3. O sistema destaca o box com a informação inválida[M1].

FE03 - Usuário ao colocar as informações de contrato não paga de imediato o valor do contrato:
1. O sistema não muda de conta free para conta premium.


## 6 Mensagens
1. [M1] O dado da mensagem está inválido, por favor insira novamente o dado da mensagem.
2. [M2] Você está offline, por favor reestabeleça a conexão e tente novamente.

## Regras de Negócio

RN01
Descrição: Nome completo
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA1]-08 [FA2]-08

RN02
Descrição: Data de nascimento
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA1]-08 [FA2]-08

RN03
Descrição: E-mail
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA1]-08 [FA2]-08

RN04
Descrição: CPF
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA1]-08 [FA2]-08

RN05
Descrição: Número do telefone
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA1]-08 [FA2]-08

RN06
Descrição: Complemento
Obrigatoriedade: Não
Passo​ ​do​ ​Fluxo: [FB]07 [FA1]-08 [FA2]-08

RN07
Descrição: Cidade
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA1]-08 [FA2]-08

RN08
Descrição: CEP
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA1]-08 [FA2]-08

RN09
Descrição: Número do cartão
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA1]-08 [FA2]-08

RN10
Descrição: Senha do cartão
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA1]-08 [FA2]-08

RN10
Descrição: Estado
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA1]-08 [FA2]-08
