Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

# ✅ [UC06] - cadastro como perfil de artista

## 1. Nome do Caso de Uso
- Cadastro como perfil de artista

## 2.  Breve descrição
- O usuário deseja ter o perfil de artista para postar as próprias músicas.

## 3.  Atores
- Usuário não cadastrado.

## 4.  Pré-Condição
- O usuário deve ser não cadastrado.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify for artists.
- O usuário abre o aplicativo.
- O usuário clica em fazer cadastro.
- Usuário coloca as informações necessárias para adquirir o perfil.
- Usuário faz um contrato com um distribuidor para a rede streaming.
- O usuário espera a certificação do aplicativo, para liberar o perfil de artista.

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

- [FE03] Usuário não possui contrato com uma distribuidora de streaming:
- O sistema mostra permanece na página de cadastro.

- [FE04] Usuário tenta criar um perfil de artista falso ou existente:
- O sistema irá validar as informações e não permitirá a criação do perfil com informações incorretas.

## 6 Mensagens
- [M1] O dado da mensagem está inválido, por favor insira novamente o dado da mensagem.
- [M2] Perfil não autorizado, tente se cadastras novamente.
