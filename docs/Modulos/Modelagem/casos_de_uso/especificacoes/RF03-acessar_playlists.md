Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio |   1.0   |


# ✅ [UC03] - Acessar playlists

## 1. Nome do Caso de Uso
- Acessar playlists

## 2.  Breve descrição
- Apresenta playlists contendo músicas que foram adicionadas à elas.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso começa quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo.
3. O usuário seleciona a opção Acessar biblioteca.
4. O sistema exibe as opções de funcionalidades disponíveis na biblioteca.
5. O usuário seleciona a opção playlists
6. O sistema lista todas as playlists do usuário [FA01]

## 5.2 Fluxos alternativos

FA01 - O usuário não possui playlists salvas
1. O sistema apresenta uma mensagem [M1] informando ao usuário que o mesmo não possui playlists salvas e mostra-lhe a opção de criar playlist ou cancelar a operação[FA02].
2. O usuário seleciona uma das opções apresentadas, se selecionado cancelar, [FA02].
3. O usuário cria uma playlist com o nome desejado.
4. O sistema apresenta segestões de músicas para salvar na playlist.
5. O fluxo básico pode ser retomado.

FA02 - O usuário cancela a operação
1. O sistema redireciona o usuário para a tela inicial.

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
