Data | Responsável | Versão|
--------- | ------| --------|
26/04/2018 | Eduardo Júnio |   1.0   |

# ✅ [UC32] - Download de playlists
## 1. Nome do Caso de Uso
- Download de playlists

## 2.  Breve descrição
- Usuário faz o download de playlists que deseja.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta premium no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.
- Estar logado na conta de usuário.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico
- O usuário loga na conta de usuário
- A tela inicial do aplicativo é apresentada
- O usuário acessa a biblioteca clicando na opção sua biblioteca
- O usuário acessa suas playlists clicando na opção playlists
- O usuário seleciona a playlist que deseja realizar o download
- O usuário seleciona a opção download
- A plylist é baixada

## 5.2 Fluxos alternativos

- O usuário loga na conta do usuário
- O usuário entra na sua biblioteca
- O usuário seleciona a opção playlists
- O usuário não possui músicas em suas playlists ou não possui playlists
- Uma tela com a opção de criar playlists ou adicionar músicas é apresentado ao usuário
- Após selecionar uma das opções apresentadas, o fluxo pode ser retomado e o usuário pode baixar a playlist desejada.

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
