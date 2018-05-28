Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio | 1.0 |

# ✅ [UC44] - Compartilhar programa de vídeo

## 1. Nome do Caso de Uso
-  Compartilhar programa de vídeo

## 2.  Breve descrição
- Permite ao usuário compartilhar programas de vídeo com outras redes sociais.

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
5. O usuário seleciona a opção Vídeos.[FA02]
6. O sistema lista todos os vídeos salvos na biblioteca.[FA01]
7. O usuário seleciona o vídeo que deseja compartilhar e seleciona a opção compartilhar.[FA02]
8. O sistema apresenta as opções de compartilhamento.[FA02]
9. O usuário seleciona a rede social que deseja compartilhar o programa de vídeo.[FA02]
10. O sistema compartilha o podacast.

## 5.2 Fluxos alternativos

FA01 - Usuário não possui programas de vídeo salvos
1. O sistema apresenta a opção Ir para navegar.
2. O usuário seleciona a opção apresentada.
3. O sistema apresenta sugestões de programas que podem ser acessados pelo usuário.
4. O usuário acessa o conteúdo desejado e o salva em sua biblioteca.
5. O fluxo básico pode ser retomado.

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