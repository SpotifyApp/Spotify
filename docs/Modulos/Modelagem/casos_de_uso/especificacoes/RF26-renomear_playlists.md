Data | Responsável | Versão|
--------- | ------| --------|
23/04/2018 | Geovanne Santos |   1.0   |

# ✅ [UC26] - Renomear playlists

## 1. Nome do Caso de Uso
- Renomear playlists

## 2.  Breve descrição
- O usuário deseja mudar o nome de uma playlist por ele criado.

## 3.  Atores
- Usuário cadastrado.

## 4.  Pré-Condição
- O usuário deve ser cadastrado.
- O usuário tem que ter feito o login no aplicativo.
- A playlist que se deseja mudar tem que ter sido feita pelo mesmo usuário.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativo e faz o login.
- O usuário clica na página de busca.
- Usuário digita o nome da playlist que se deseja mudar o nome.
- Seleciona a playlist.
- Usuário clica na opção da playlist(renomear), então digita o novo nome e salva.

## 5.2 Fluxos alternativos

- [FA01]
- O usuário faz o login.
- Usuário acessa sua biblioteca.
- Usuário clica no símbolo que faz o link com seu perfil.
- Usuário clica em playlists e aparecerá todas as playlists que pertencem aquele perfil.
- Usuário seleciona a playlist que deseja mudar.
- Usuário clica na opção da playlist(renomear), então digita o novo nome e salva.

## 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

- [FE02] Usuário tenta mudar o nome de uma playlist que não pertence ao seu perfil:
- O sistema não mostrará a opção de renomear para a playlist que não pertence ao mesmo perfil.

## 6 Mensagens
- Nãõ existe.
