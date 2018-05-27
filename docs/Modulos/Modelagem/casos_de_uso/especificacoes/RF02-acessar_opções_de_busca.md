Data | Responsável | Versão|
--------- | ------| --------|
23/04/2018 | Geovanne Santos |   1.0   |

# ✅ [UC02] - Acessar opções de busca

## 1. Nome do Caso de Uso
- Acessar opções de busca

## 2.  Breve descrição
- O usuário deseja procurar por alguma playlist, música ou artista, acessando a página de busca.

## 3.  Atores
- Usuário cadastrado.

## 4.  Pré-Condição
- O usuário deve ser cadastrado.
- Ter o aplicativo do Spotify instalado.
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativo e faz o login.
- O usuário clica na página de busca.
- Usuário digita o nome que deseja, para encontrar artistas, playlist e música relacionado.

## 5.2 Fluxos alternativos

- [FA01]
- O usuário usa a opção escanear, que é achar uma playlist, artista ou música escaneando o código de um outro smartphone.

## 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

- [FE02] Usuário digitar um nome que não existe:
- O sistema identifica a resposta inválida .
- O sistema dispara uma mensagem de erro.
- O sistema fica na mesma página.

## 6 Mensagens
- [M1] Este nome não existe, tente buscar por algo diferente.
