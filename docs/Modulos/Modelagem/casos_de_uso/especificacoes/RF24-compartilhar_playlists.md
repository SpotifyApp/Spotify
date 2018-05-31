Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio | 1.0 |

# ✅ [UC24] - Compartilhar playlists

## 1. Nome do Caso de Uso
-  Compartilhar playlists

## 2.  Breve descrição
- Permite ao usuário compartilhar playlists de músicas com outras redes sociais.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.
- Possuir conta na rede social que deseja compartilhar o programa.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso inicia quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo.
3. O usuário seleciona a opção Acessar biblioteca.
4. O sistema exibe as opções de funcionalidades disponíveis na biblioteca.
5. O usuário seleciona a opção Playlists.[FA02]
6. O sistema apresenta todas as playlists salvas na biblioteca.[FA01]
7. O usuário seleciona a playlist que deseja compartilhar e seleciona a opção compartilhar.[FA02]
8. O sistema apresenta as opções de compartilhamento.[FA02]
9. O usuário seleciona a rede social que deseja compartilhar a playlist.[FA02]
10. O sistema compartilha a playlist.

## 5.2 Fluxos alternativos

FA01 - Usuário não possui playlists salvas
1. O sistema apresenta a opção Criar playlist.
2. O usuário seleciona a opção apresentada.
3. O sistema solicita o nome, imagem e descrição da playlist.[FA02]
4. O usuário seleciona a opção Criar.
5. O sistema cria a playlist.
6. O sistema apresenta sugestões de músicas que podem ser adicionadas à playlist e playlists que podem ser salvas pelo usuário.
7. O usuário seleciona o conteúdo desejado e o salva em sua playlist.
8. O fluxo básico pode ser retomado.

FA02 - O usuário cancela a operação
1. O usuário cancela a operação corrente.
2. O sistema redireciona o usuário para outra tela.

## 5.3 Fluxos de Exceção

FE01 - Não ter acesso a Internet durante o procedimento
1. O sistema informa "O spotify está offline"[M1].
2. A operação é interrompida.
3. O caso de uso se encerra.

FE02 - Aplicativo parar de funcionar
1. O sistema informa: "O aplicativo encerrou inesperadamente."[M2]
2. A operação é interrompida.
3. O caso de uso se encerra.

## 6 Mensagens
- [M1] O spotify está offline.
- [M2] O aplicativo encerrou inesperadamente.