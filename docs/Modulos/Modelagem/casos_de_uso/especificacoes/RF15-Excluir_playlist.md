Data | Responsável | Versão|
--------- | ------| --------|
26/04/2018 | Eduardo Júnio |   1.0   |

# ✅ [UC32] - Excluir playlists
## 1. Nome do Caso de Uso
- Excluir playlists

## 2.  Breve descrição
- Usuário exclui playlists que deseja.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.
- Estar logado na conta de usuário.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico
- O usuário loga na conta de usuário
- A tela inicial do aplicativo é apresentada
- O usuário acessa a biblioteca clicando na opção sua biblioteca
- O usuário acessa suas playlists clicando na opção playlists
- O usuário seleciona a playlist que deseja excluir
- O usuário seleciona a opção Apagar playlist
- A playlist é apagada

## 5.2 Fluxos alternativos

- O usuário loga na conta do usuário
- O usuário entra na sua biblioteca
- O usuário seleciona a opção playlists
- O usuário não possui músicas em suas playlists ou não possui playlists

## 5.3 Fluxos de Exceção
[FE01] Perda de conexão com a internet
- O usuário loga na conta do spotify
- O usuário acessa sua biblioteca
- O aplicativo perde  conexão com a internet
- Uma mensagem informando problema de conexão é apresentado ao usuário

[FE02] Mal funcionamento do aplicativo
- O usuário loga na conta do spotify
- O usuário acessa sua biblioteca
- O aplicativo fecha indevidamente

## 6 Mensagens
- [M1] Sem conexão com a internet.
- [M2] O aplicativo fechou inesperadamente
