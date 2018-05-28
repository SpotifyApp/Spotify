Data | Responsável | Versão|
--------- | ------| --------|
23/04/2018 | Geovanne Santos |   1.0   |
27/05/2018 | Eduardo Júnio |   2.0   |

# ✅ [UC26] - Renomear playlists

## 1. Nome do Caso de Uso
- Renomear playlists

## 2.  Breve descrição
- Permite ao usuário modificar o nome de uma playlist criada por ele.

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
5. O usuário seleciona a opção playlists.
6. O sistema lista todas as playlists salvas na biblioteca do usuário [FA01]
7. O usuário seleciona a playlist que deseja renomear.[FA02]
8. O sistema apresenta o conteúdo da playlist e o menu de gerenciamento da playlist.
9. O usuário seleciona a opção Editar detalhes.
10. O sistema apresenta ao usuário uma tela solicitando o novo nome que será dado à playlist.
11. O usuário insere o nome da playlist.
12. O sistema salva o novo nome da playlist.

## 5.2 Fluxos alternativos

FA01 - O usuário não possui playlists
1. O sistema apresenta a opção "Criar playist".
2. O usuário seleciona a opção apresentada.
3. O sistema apresenta músicas em destaque e categorias.
4. O usuário seleciona alguma das opções e a adiciona à sua playlist.
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