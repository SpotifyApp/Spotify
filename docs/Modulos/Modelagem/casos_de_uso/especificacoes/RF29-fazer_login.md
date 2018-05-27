Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |
25/05/2018 | Lucas Cunha | 2.0 |

# ✅ [UC29] - Fazer login

## 1. Nome do Caso de Uso
- Fazer Login

## 2.  Breve descrição
- Autentica o usuário no aplicativo dando a ele acesso às informações de sua conta e as funcionalidades.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso começa quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo sem estar logado.
3. O usuário acessa a tela de login.
4. O sistema exibe campos de entrada para Email/Nome de Usuário e senha.
5. O usuário digita o seu Email/Nome de Usuário e sua senha. [FA01]
6. O usuário envia os dados.
7. O sistema autentica o usuário. [FE 01],[FE02]


## 5.2 Fluxos alternativos

FA01 - O usuário esqueceu a senha
1. Logo após digitar o Email/Nome de Usuário, o usuário seleciona opção para resetar a senha.
2. O sistema envia um e-mail ao ator para trocar a senha.
3. O usuário redefine sua senha.
4. O fluxo principal é recomeçado.

## 5.3 Fluxos de Exceção
FE01 - Não ter acesso a Internet durante o procedimento e sem login posterior no mesmo aparelho.
1. O sistema informa "Verifique as configurações de aplicativo"[M2].
2. A operação é interrompida.
3. O caso de uso se encerra.

FE02 - Preenchimento incorreto dos dados
1. O sistema informa "O e-mail e senha inseridos não correspondem a nenhuma conta do Spotify. Tente de novo."[M1]


## 6 Mensagens
- [M1] O e-mail e senha inseridos não correspondem a nenhuma conta do Spotify. Tente de novo.
- [M2] Verifique as configurações de aplicativo.

## Regras de Negócio

RN01
Descrição: E-mail
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: FB05

RN02
Descrição: Nome de Usuário.
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: FB05

RN03
Descrição: Senha​ ​ de​ ​ no​ ​ mínimo​ ​ 6 caracteres.
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: FB05
