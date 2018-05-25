Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

# ✅ [UC29] - Fazer login

## 1. Nome do Caso de Uso
- Fazer Login

## 2.  Breve descrição
- Usuário faz o login.

## 3.  Atores
- Usuário cadastrado.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário clica em fazer login.
- O usuário põem as informações de endereço de email e senha.
- Clica em entrar.
- O sistema vai para o template de usuário cadastrado.


## 5.2 Fluxos alternativos

- [FA01] Usuário faz o login pela sua conta no facebook:
- O usuário entra no aplicativo.
- O usuário clica em entrar pela conta do facebook.
- Coloca as informações da conta.
- Clica em confirmar.
- E direcionado a parte do aplicativo de funcionalidades para cadastrados.

## 5.3 Fluxos de Exceção
- [FE01] Errar algum dos dados de login:
- O sistema identifica o dado inválido(endereço de email ou senha) .
- O sistema permanece na mesma página.
- O sistema destaca o box com a informação inválida.

- [FE02] Usuário coloca dados de rede social inválido:
- O sistema identifica a informação inválida .
- O sistema permanece na mesma página.
- O sistema destaca a informação inválida.

## 6 Mensagens
- [M1] O email não existe.
- [M2] Senha incorreta.
- [M3]Dados de rede social inválidos.
