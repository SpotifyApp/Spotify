Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

# ✅ [UC06] - Mudar o tipo de perfil

## 1. Nome do Caso de Uso
- Mudar o tipo de perfil

## 2.  Breve descrição
- O usuário comum deseja se tornar usuário artista.

## 3.  Atores
- Usuário comum.

## 4.  Pré-Condição
- O usuário deve ser comum.
- Ter o aplicativo desktop do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário clica em requerir o perfil artista.
- Usuário coloca as informações necessárias, tais como a agência que irá distribuir a música para o aplicativo, o Twitter e outros.
- O usuário espera o aplicativo autenticar o perfil requerido para usar as funcionalidades novas.

## 5.2 Fluxos alternativos

- Não existe.

## 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

- [FE02] Usuário coloca alguma informação errada:
- O sistema identifica a resposta inválida .
- O sistema permanece na mesma página.
- O sistema destaca o box com a informação inválida.

- [FE03] Usuário tenta criar um perfil fake:
- O sistema não irá autorizar o requerimento do perfil.


## 6 Mensagens
- [M1] O dado da mensagem está inválido, por favor insira novamente o dado da mensagem.
- [M2] O requerimento do perfil não foi autorizado.
