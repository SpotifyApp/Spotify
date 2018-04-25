# Especificações de Casos de Uso

* [Integração com Redes Sociais](#integracao-com-redes-sociais)
* [Gerenciar playlists salvas](#gerenciar-playlists-salvas)
* [Gerenciar artistas salvos](#gerenciar-artistas-salvos)
* [Cadastro como perfil de artista](#cadastro-como-perfil-de-artista)
* [Fazer login](#fazer-login)
* [Editar dados de conta](#editar-dados-de-conta)
* [Atualizar biografia do artista](#atualizar-biografia-do-artista)
* [Sair do aplicativo](#sair-do-aplicativo)
* [Mudar o tipo de perfil](#mudar-o-tipo-de-perfil)
* [Cadastro de usuário comum](#cadastro-de-usuario-comum)
* [Adquirir o plano premiun](#adquirir-o-plano-premiun)
* [Ficar em modo offline](#ficar-em-modo-offline)
* [Postar uma música](#postar-uma-musica)
* [Colocar a agenda de shows](#colocar-a-agenda-de-shows)


---

## Integração com Redes Sociais

### 1. Descrição

Descrição - Este caso de uso permite ao usuário facilidade de compartilhamento, usabilidade, podendo compartilhar playlists e músicas, entre outras funcioalidades.

### 2. Fluxo de Eventos

#### 2.1 Fluxo Básico
1. O fluxo básico começa quando o usuário acessa a plataforma Spotify e começa a utilizar o aplicativo (#R21 – Navegar (de acordo com o documento de Especificação suplementar)) .
1. O usuário acessa o Aplicativo.
2. O usuário navega dentro do aplicativo. [RF 21]
3. O usuário tem diversas opções dentro das funcionalidades disponíveis.
4. O usuário acessa uma playlist [RF 03] ou uma música
5. Dentro dessa funcionalidade ele pode compartilhar uma playlist ou músicas entre as redes sociais integradas, como o whatsapp e facebook.

#### 2.2 Fluxo Alternativo
1. Buscar uma música sem necessariamente acessar uma playlist.
    1. O usuário acessa o Aplicativo.
    2. O usuário navega dentro do aplicativo. [RF 21]
    3. O busca por uma música em especifica.
    4. Dentro dessa funcionalidade ele pode compartilhar uma playlist ou músicas entre as redes sociais integradas, como o whatsapp e facebook.

#### 2.3 Fluxos de Exceção
1. Erro na integração com outra rede social
    1. O usuário solicita alguma funcionalidade que exige dados de outra rede social.
    2. O sistema tenta o acesso e apresenta erro.
    3. O sistema volta para a página anterior.

### 3. Requisitos Especiais
 - Nenhum requisito especial identificado.

### 4. Condições Prévias
  - Estar conectado com a internet.
  - Possuir acesso as outras redes sociais.

### 5. Mensagens
[MES01] “Erro ao conectar ao aplicativo”.

---

## Gerenciar playlists salvas

### 1. Nome do Caso de Uso
- Gerenciar playlists

### 2.  Breve descrição
- Gerenciar minhas playlists salvas

### 3.  Atores
- Usuário

### 4.  Fluxo de eventos

#### 4.1 Fluxo básico

- O usuário abre o aplicativo
- O aplicativo exibe a tela inicial
- O usuário seleciona a opção “Sua biblioteca”
- O aplicativo apresenta um menu com várias opções
- O usuário seleciona a opção “playlists”
- O aplicativo lista todas as playlists salvas
- O usuário pode compartilhar, excluir, renomear ou reproduzir suas playlists

#### 4.2 Fluxos alternativos

- O usuário não possui nenhuma playlist salva
- O aplicativo informa que o usuário não possui nenhuma playlist salva, logo ele não tem acesso às opções de gerenciamento de playlists (excluir, compartilhar, renomear ou reproduzir suas playlists).
- O aplicativo apresenta a opção de “Criar sua primeira playlist”
- Ao criar uma nova playlists, as opções de gerenciamento ficam novamente disponíveis.
- O fluxo principal é retomado.


#### 4.3 Fluxos de Exceção

- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

### 5. Pré-condições

- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.
- Possuir conta de usuário no Spotify


---

## Gerenciar artistas salvos

### 1. Nome do Caso de Uso
- Gerenciar artistas salvos

### 2.  Breve descrição
- Gerenciar meus artistas salvos

### 3.  Atores
- Usuário

### 4.  Fluxo de eventos

#### 4.1 Fluxo básico
- O usuário abre o aplicativo
- O aplicativo exibe a tela inicial
- O usuário seleciona a opção “Sua biblioteca”
- O aplicativo apresenta um menu com várias opções
- O usuário seleciona a opção “artistas”
- O aplicativo lista todas os artistas salvas    
- O usuário pode ver o perfil do artista, acessar rádio do artista, compartilhar perfil do artista ou adicionar perfil do artista à tela inicial do celular

#### 4.2 Fluxos alternativos
- O usuário não possui nenhum artista salvo
- O aplicativo informa que o usuário não possui nenhum artista salvo, logo ele não tem acesso às opções de gerenciamento de artistas salvos (ver o perfil do artista, acessar rádio do artista, compartilhar perfil do artista ou reproduzir suas playlists).
- O aplicativo apresenta a opção de salvar músicas de artistas
- Ao salvar músicas de um artista ou seguir um perfil de artista, as opções de gerenciamento ficam novamente disponíveis.
- O fluxo principal é retomado.


#### 4.3 Fluxos de Exceção
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

### 5. Pré-condições
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.
- Possuir conta de usuário no Spotify

---

## Cadastro como perfil de artista

### 1. Nome do Caso de Uso
- Cadastro como perfil de artista

### 2.  Breve descrição
- O usuário deseja ter o perfil de artista para postar as próprias músicas.

### 3.  Atores
- Usuário não cadastrado.

### 4.  Pré-Condição
- O usuário deve ser não cadastrado.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

### 5.  Fluxo de eventos

#### 5.1 Fluxo básico

- O usuário instala o spotify for artists.
- O usuário abre o aplicativo.
- O usuário clica em fazer cadastro.
- Usuário coloca as informações necessárias para adquirir o perfil.
- Usuário faz um contrato com um distribuidor para a rede streaming.
- O usuário espera a certificação do aplicativo, para liberar o perfil de artista.

#### 5.2 Fluxos alternativos

- Não existe.

#### 5.3 Fluxos de Exceção
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

#### 6 Mensagens
- [M1] O dado da mensagem está inválido, por favor insira novamente o dado da mensagem.
- [M2] Perfil não autorizado, tente se cadastras novamente.

---
## Fazer login

### 1. Nome do Caso de Uso
- Fazer Login

### 2.  Breve descrição
- Usuário faz o login.

### 3.  Atores
- Usuário cadastrado.

### 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

### 5.  Fluxo de eventos

#### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário clica em fazer login.
- O usuário põem as informações de endereço de email e senha.
- Clica em entrar.
- O sistema vai para o template de usuário cadastrado.


### 5.2 Fluxos alternativos

- [FA01] Usuário faz o login pela sua conta no facebook:
- O usuário entra no aplicativo.
- O usuário clica em entrar pela conta do facebook.
- Coloca as informações da conta.
- Clica em confirmar.
- E direcionado a parte do aplicativo de funcionalidades para cadastrados.

### 5.3 Fluxos de Exceção
- [FE01] Errar algum dos dados de login:
- O sistema identifica o dado inválido(endereço de email ou senha) .
- O sistema permanece na mesma página.
- O sistema destaca o box com a informação inválida.

- [FE02] Usuário coloca dados de rede social inválido:
- O sistema identifica a informação inválida .
- O sistema permanece na mesma página.
- O sistema destaca a informação inválida.

### 6. Mensagens
- [M1] O email não existe.
- [M2] Senha incorreta.
- [M3]Dados de rede social inválidos.

---

## Editar dados de conta
### 1. Descrição
Editar as informações pessoais do usuário.

### 2. Atores
Usuário cadastrado

### 3. Pré-condição:
O usuário deve possuir uma conta no spotify.

### 4. Fluxo Principal:
<ul>
  <li>Faz o login.</li>
  <li>O usuário vai na página web do site.</li>
  <li>O usuário clica em editar perfil.</li>
  <li>Modifica os dados.</li>
  <li>Clica em salvar.</li>
</ul>

### 5. Fluxos Alternativos
<h6>[FA01]Usuário clica em modificar somente senha:</h6>
O usuário entra no site spotify.<br />
O usuário faz o login.<br />
O usuário clica em modificar somente senha.<br />
Modifica o dado.<br />
Clica em salvar.<br />
<h6>[FA02]Usuário modifica a foto do perfil pelo aplicativo:</h6>
O usuário entra no aplicativo spotify.<br />
vai no seu perfil.<br />
O usuário modifica sua foto de perfil.<br />

### 6. Fluxo de Exceção:
<h6>[FE01] Tenta modificar os dados que não sejam a foto de perfil pelo aplicativo:</h6>
O aplicativo não possui essa funcionalidade.

---

## Atualizar biografia do artista

### 1. Nome do Caso de Uso
- atualizar biografia do artista

### 2.  Breve descrição
- O artista deseja mudar o conteúdo da biografia que está presente no seu perfil de artista.

### 3.  Atores
- Usuário artista.

### 4.  Pré-Condição
- O usuário deve ser usuário artista.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.
- Ter feito o login.

### 5.  Fluxo de eventos

#### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário vai na aba de biografia eclica em editar.
- Usuário faz a modificação e salva.

### 5.2 Fluxos alternativos

- Não existe.

### 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

- [FE02] Usuário ainda não tem perfil de artista autenticado:
- O sistema não deixará o usuário fazer nenhum ação que envolva o perfil artista até ser validado.

### 6 Mensagens
- [M1] A modificação da biografia não foi efetuada, sua conexão caiu.

---

## Sair do aplicativo

### 1. Nome do Caso de Uso
- Sair do aplicativo

### 2.  Breve descrição
- Usuário sai da conta atual.

### 3.  Atores
- Usuário.

### 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Estar logado no aplicativo.
- Ter o aplicativo do Spotify instalado

### 5.  Fluxo de eventos

#### 5.1 Fluxo básico

- O usuário faz o login spotify.
- O usuário é direcionado a parte de usuário.
- O usuário sai da conta.

---

## Mudar o tipo de perfil

### 1. Nome do Caso de Uso
- Mudar o tipo de perfil

### 2.  Breve descrição
- O usuário comum deseja se tornar usuário artista.

### 3.  Atores
- Usuário comum.

### 4.  Pré-Condição
- O usuário deve ser comum.
- Ter o aplicativo desktop do Spotify instalado
- Estar conectado à internet.

### 5.  Fluxo de eventos

#### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário clica em requerir o perfil artista.
- Usuário coloca as informações necessárias, tais como a agência que irá distribuir a música para o aplicativo, o Twitter e outros.
- O usuário espera o aplicativo autenticar o perfil requerido para usar as funcionalidades novas.

#### 5.2 Fluxos alternativos

- Não existe.

#### 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

- [FE02] Usuário coloca alguma informação errada:
- O sistema identifica a resposta inválida .
- O sistema permanece na mesma página.
- O sistema destaca o box com a informação inválida.

- [FE03] Usuário tenta criar um perfil fake:
- O sistema não irá autorizar o requerimento do perfil.


#### 6 Mensagens
- [M1] O dado da mensagem está inválido, por favor insira novamente o dado da mensagem.
- [M2] O requerimento do perfil não foi autorizado.

---

## Cadastro de usuário comum

### 1. Nome do Caso de Uso
- Cadastro de usuário comum

### 2.  Breve descrição
- Criar um cadastro de usuário.

### 3.  Atores
- Usuário não cadastrado

### 4.  Pré-Condição
- O usuário deve possuir um endereço de email, conta no Facebook ou conta no Google+.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

### 5.  Fluxo de eventos

#### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e clica em "Cadastrar".
- O usuário coloca as informações de endereço de email, senha, data de nascimento e gênero.
- Usuário aceito os termos do aplicativo.
- O sistema vai para o template de usuário cadastrado.

#### 5.2 Fluxos alternativos

- [FA01] Seria o requisito RF07 .

#### 5.3 Fluxos de Exceção
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

#### 6 Mensagens
- [M1] Idade não permitida para uso do aplicativo.
- [M2] Senha com tamanho não permitido, mínimo 8 caracteres.

---

## Adquirir o plano premiun

### 1. Nome do Caso de Uso
- Adquirir o plano premiun

### 2.  Breve descrição
- Comprar o plano premiun, com mais funcionalidades.

### 3.  Atores
- Usuário free.

### 4.  Pré-Condição
- O usuário deve ser free.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

### 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário clica em adquirir plano premiun.
- Usuário coloca as informações para o contrato do plano ser firmado.
- O usuário escolhe a forma de pagamento.
- O usuário paga a fatura e mude do plano free para o plano premiun de imediato.

#### 5.2 Fluxos alternativos

- [FA01]
- Adquirir um plano premiun, pelo pacote estudantil.

- [FA02]
- Adquirir um plano premiun, pelo pacote família.

#### 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

- [FE02] Usuário coloca alguma informação errada:
- O sistema identifica a resposta inválida .
- O sistema permanece na mesma página.
- O sistema destaca o box com a informação inválida.

- [FE03] Usuário não paga a fatura:
- O sistema não muda de free para premiun .


### 6 Mensagens
- [M1] O dado da mensagem está inválido, por favor insira novamente o dado da mensagem.

---

## Ficar em modo offline

### 1. Nome do Caso de Uso
- ficar em modo offline

### 2.  Breve descrição
- Usuário faz login no aplicativo e deseja reproduzir as músicas em modo offline para não gastar pacote de internet.

### 3.  Atores
- Usuário comum.

### 4.  Pré-Condição
- O usuário deve ser comum.
- Ter o aplicativo do Spotify instalado.
- Ter feito o login.

### 5.  Fluxo de eventos

#### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário vai na parte de configurações.
- Usuário ativa o modo offline.

#### 5.2 Fluxos alternativos

- Não existe

#### 5.3 Fluxos de Exceção
- Não existe

### 6 Mensagens
- Não existe

---

## Postar uma música

### 1. Nome do Caso de Uso
- postar uma música

### 2.  Breve descrição
- Usuário artista deseja postar uma música no aplicativo spotify.

### 3.  Atores
- Usuário artista.

### 4.  Pré-Condição
- O usuário deve ser ter o perfil artista.
- Ter o aplicativo do Spotify instalado.
- Ter colocado a música no site da gravadora que ela tem contrato.

### 5.  Fluxo de eventos

#### 5.1 Fluxo básico

- O usuário artista instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário vai no site da gravadora(distribuidora) e posta a música no site deles.
- A gravadora direciona a música pro aplicativo spotify.

### 5.2 Fluxos alternativos

- Não existe

### 5.3 Fluxos de Exceção
- [FE01]Tentar postar uma música que já existe.

### 6 Mensagens
- [M1]Esta música já existe ou não de sua autoria.

---

## Colocar a agenda de shows

### 1. Nome do Caso de Uso
- colocar a agenda de shows

### 2.  Breve descrição
- Usuário artista deseja divulgara agenda de shows no seu perfil.

### 3.  Atores
- Usuário artista.

### 4.  Pré-Condição
- O usuário deve ter o perfil artista.
- Ter o aplicativo do Spotify instalado.
- Ter feito o login.

### 5.  Fluxo de eventos

#### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário vai na parte de adicionar agenda de shows.
- Usuário coloca as informações necessárias(data e cidade).

#### 5.2 Fluxos alternativos

- [FA01]Adicionar uma data e um local por cima de outro, devido a algum imprevisto.

#### 5.3 Fluxos de Exceção
- [FE01] Tentar adicionar alguma agenda de shows não possuindo o perfil de artista.
- [FE02] Faltar com alguma informação da parte de shows.

### 6 Mensagens
- [M1] está faltanto um campo obrigatório.
