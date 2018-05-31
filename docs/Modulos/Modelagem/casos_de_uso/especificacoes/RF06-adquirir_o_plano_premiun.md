Data | Responsável | Versão| Modificações |
--------- | ------| --------|  --------|
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
5. O sistema direciona o usuário para página de colocar informações de compra.[FA01] [FA02] [FA03]
6. O usuário aceita o contrato padrão de plano premium(3 meses de premium por R$ 16.90, depois dos 3 meses vira  R$ 16.90 por mês) que deseja firmar e a forma de pagamento padrão, que é o cartão de crédito.
7. O usuário coloca as informações necessárias.
8. O sistema valida as informações.[FE02][FE01]
9. O sistema muda a conta de tipo free para tipo premium após o pagamento. [FE03]

## 5.2 Fluxos alternativos

FA01 - O usuário deseja adquirir o plano premium estudantil

1. O usuário acessa a página de planos premium alternativos.
2. O sistema direciona para a página de tipos de plano premiun.
3. O usuário escolhe o plano premium estudantil(R$ 8.50 por mês) e coloca as informações necessárias(inclusive a do cartão de crédito, que é a única forma de pagamento deste plano).
4. O sistema valida as informações.[FE02][FE01]
5. O sistema muda a conta de tipo free para tipo premium após o pagamento.[FE03]

FA02 - O usuário deseja adquirir o plano premium familiar e dividir o preço do plano com várias pessoas

1. O usuário acessa a página de planos premiun alternativos.
2. O sistema direciona para a página de tipos de plano premium.
3. O usuário escolhe o plano premium familiar(R$ 26.00 por mês, para 5 pessoas) e coloca as informações necessárias(inclusive a do cartão de crédito ou débito, que são as formas de pagamento deste plano).
4. O sistema valida as informações.[FE02][FE01]
5. O sistema muda a conte de tipo free para tipo premium após o pagamento.[FE03]

FA03 - O usuário deseja adquirir o plano premium comprando o plano que é pago por boleto

1. O usuário acessa a página de tipos de pagamento.
2. O sistema direciona para a página com as opções de pagamento.
3. O usuário acessa a opção de boleto.
4. O sistema mostra as opções(R$ 16,90 1 mês, R$ 49,00 3 mês, R$ 99,00 6 mês )
5. O usuário escolhe entre as três opções acima e coloca as informações necessárias.
6. O sistema valida as informações.[FE02][FE01]
7. O sistema gera o boleto
5. O sistema muda a conta de tipo free para tipo premium após o pagamento.[FE03]

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
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN02
Descrição: Data de nascimento
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN03
Descrição: E-mail
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN04
Descrição: CPF
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN05
Descrição: Número do telefone
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN06
Descrição: Complemento
Obrigatoriedade: Não
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN07
Descrição: Cidade
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN08
Descrição: CEP
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN09
Descrição: Número do cartão
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA02]-03

RN10
Descrição: Senha do cartão
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA02]-03

RN10
Descrição: Estado
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08

RN10
Descrição: Comprovante de estudante
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FA01]-03

RN11
Descrição: Data de vencimento do cartão
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA02]-03
