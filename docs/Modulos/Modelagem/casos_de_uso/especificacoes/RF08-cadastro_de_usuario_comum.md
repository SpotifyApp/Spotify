Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

# ✅ [UC08] - Cadastro de usuário comum

## 1. Nome do Caso de Uso
- Cadastro de usuário comum

## 2.  Breve descrição
- Criar um cadastro de usuário.

## 3.  Atores
- Usuário não cadastrado

## 4.  Pré-Condição
- O usuário deve possuir um endereço de email, conta no Facebook ou conta no Google+.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e clica em "Cadastrar".
- O usuário coloca as informações de endereço de email, senha, data de nascimento e gênero.
- Usuário aceito os termos do aplicativo.
- O sistema vai para o template de usuário cadastrado.

## 5.2 Fluxos alternativos

- [FA01] Seria o requisito RF07 .

## 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

- [FE02] Usuário coloca a data de nascimento que comprova menor idade:
- O sistema identifica a idade inválida .
- O sistema permanece na mesma página.
- O sistema destaca o box com a informação de idade inválida.

- [FE03] Usuário coloca senha com menos de 8 caracteres:
- O sistema identifica a senha inválida .
- O sistema permanece na mesma página.
- O sistema destaca o box com a informação de idade inválida.

## 6 Mensagens
- [M1] Idade não permitida para uso do aplicativo.
- [M2] Senha com tamanho não permitido, mínimo 8 caracteres.
