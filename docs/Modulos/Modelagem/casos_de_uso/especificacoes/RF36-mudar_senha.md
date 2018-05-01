Data | Responsável | Versão|
--------- | ------| --------|
23/04/2018 | Geovanne Santos |   1.0   |

# ✅ [UC02] - mudar de senha

## 1. Nome do Caso de Uso
- Mudar de senha

## 2.  Breve descrição
- O usuário deseja mudar de senha.

## 3.  Atores
- Usuário cadastrado.

## 4.  Pré-Condição
- O usuário deve ser cadastrado.
- Estar conectado à internet.
- Ter feito login na versão site do spotify.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário acessa o site spotify.
- O usuário faz o login.
- O usuário acessa a página de mudar senha.
- Usuário digita as informações necessárias que o site irá pedir(senha atual, nova senha, repetir nova senha).

## 5.2 Fluxos alternativos

- [FA01]
- O usuário acessa o site do spotify, na parte de redefinir senha.
- Digita o email da sua conta spotify.
- Vá no seu email e clique no email que o spotify te enviou, ele te direcionará para uma página.
- Coloque as informações necessárias(nova senha, confirmação de nova senha).

## 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

- [FE02] Usuário digita um email não válido, ou seja, que não pertence a sua conta:
- O sistema identifica a resposta inválida .
- O sistema dispara uma mensagem de erro.
- O sistema fica na mesma página.

## 6 Mensagens
- [M1] Este endereço de email ou nome de usuário não pertence a nenhuma conta spotify.
