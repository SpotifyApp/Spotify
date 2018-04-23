Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

# ✅ [UC39] - atualizar biografia do artista

## 1. Nome do Caso de Uso
- atualizar biografia do artista

## 2.  Breve descrição
- O artista deseja mudar o conteúdo da biografia que está presente no seu perfil de artista.

## 3.  Atores
- Usuário artista.

## 4.  Pré-Condição
- O usuário deve ser usuário artista.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.
- Ter feito o login.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário vai na aba de biografia eclica em editar.
- Usuário faz a modificação e salva.

## 5.2 Fluxos alternativos

- Não existe.

## 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

- [FE02] Usuário ainda não tem perfil de artista autenticado:
- O sistema não deixará o usuário fazer nenhum ação que envolva o perfil artista até ser validado.

## 6 Mensagens
- [M1] A modificação da biografia não foi efetuada, sua conexão caiu.
