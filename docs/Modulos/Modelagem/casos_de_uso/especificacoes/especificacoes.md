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

Data | Responsável | Versão|
--------- | ------| --------|
25/04/2018 | Eduardo Júnio |   1.0   |

#  [UC01] - Gerenciar playlists

<object width="700" height="600" data="../diagrama_de_uso/caso-gerenciar_playlist.png"></object>

## 1. Nome do Caso de Uso
- Gerenciar playlists

## 2.  Breve descrição
- Gerenciar minhas playlists salvas

## 3.  Atores
- Usuário

## 4.  Fluxo de eventos

### 4.1 Fluxo básico

- O usuário abre o aplicativo
- O aplicativo exibe a tela inicial
- O usuário seleciona a opção “Sua biblioteca”
- O aplicativo apresenta um menu com várias opções
- O usuário seleciona a opção “playlists”
- O aplicativo lista todas as playlists salvas
- O usuário pode compartilhar, excluir, renomear ou reproduzir suas playlists

## 4.2 Fluxos alternativos

- O usuário não possui nenhuma playlist salva
- O aplicativo informa que o usuário não possui nenhuma playlist salva, logo ele não tem acesso às opções de gerenciamento de playlists (excluir, compartilhar, renomear ou reproduzir suas playlists).
- O aplicativo apresenta a opção de “Criar sua primeira playlist”
- Ao criar uma nova playlists, as opções de gerenciamento ficam novamente disponíveis.
- O fluxo principal é retomado.


## 4.3 Fluxos de Exceção

- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

## 5. Pré-condições

- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.
- Possuir conta de usuário no Spotify

----

Data | Responsável | Versão|
--------- | ------| --------|
23/04/2018 | Geovanne Santos |   1.0   |

#  [UC02] - Acessar opções de busca

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

----

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio |   1.0   |


#  [UC03] - Acessar playlists

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

-----

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Geovanne Santos |   1.0   |


#  [UC03] - Acessar rádio

## 1. Nome do Caso de Uso
- Acessar rádio

## 2.  Breve descrição
- O usuário deseja que o spotify escolha as músicas que serão tocadas, ou que possa criar qualquer estação de rádio escolhendo os artistas e playlists que irão basear a rádio.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta premium.
- Ter o aplicativo do Spotify instalado
- Ter feito o login.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso começa quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo.
3. O usuário seleciona a opção Acessar rádio.
4. O sistema exibe as opções de funcionalidades disponíveis na página rádio.[FA01] [FA02]
5. O usuário seleciona uma rádio baseada nas recomendações que spotify fez(de acordo com as músicas que o usuário ouve)
6. O sistema começa a tocar a rádio selecionada.

## 5.2 Fluxos alternativos

FA01 - O usuário ouve uma rádio de acordo com o gênero dela
1. O usuário seleciona uma rádio de acordo com o gênero dela(rock, samba, mpb, entre outros) FE01
2. O sistema começa a tocar a rádio selecionada.


FA02 - O usuário deseja criar uma estação de rádio, baseada em algumas playlists e artistas
1. O usuário seleciona a opção de criar uma rádio.
2. O sistema direciona o usuário para a página de criar rádio. FE01
3. O usuário escolhe os artistas e playlists que a rádio deve se basear, pelo campo de busca.
4. O sistema gera a rádio.
5. O usuário poderá somente ouvir a rádio ou adiciona-lá a biblioteca.

## 5.3 Fluxos de Exceção
FE01 - Não ter acesso a Internet durante o procedimento
1. O sistema informa "O spotify está offline"[M1].
2. A operação é interrompida.
3. O caso de uso se encerra.

FE02 - Aplicativo parar de funcionar
1. O sistema informa: "O aplicativo encerrou inesperadamente."[M2]
2. A operação é interrompida.
3. O caso de uso se encerra.

FE03 - O nome que o usuário procura não existe
1. O sistema informa [M1].

## 6 Mensagens
- [M1] O spotify está offline.
- [M2] O aplicativo encerrou inesperadamente.
- [M3] O nome desejado não existe, por favor tente um nome diferente.

-----

Data | Responsável | Versão|
--------- | ------| --------|
23/04/2018 | Geovanne Santos |   1.0   |

#  [UC02] - Adicionar música a uma playlist.

## 1. Nome do Caso de Uso
- Adicionar música a uma playlist.

## 2.  Breve descrição
- O usuário deseja adicionar uma música a uma playlist que ele criou.

## 3.  Atores
- Usuário cadastrado.

## 4.  Pré-Condição
- O usuário deve ser cadastrado.
- Ter o aplicativo do Spotify instalado.
- A música deve ser adicionada pelo mesmo usuário que criou a playlist.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativo e faz o login.
- O usuário está ouvindo uma música.
- Usuário clica nas opções de música.
- Usuário clica em adicionar música a uma playlist.
- Usuário seleciona a playlist e adiciona.

## 5.2 Fluxos alternativos

- [FA01]
- Não existe.

## 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

## 6 Mensagens
- Não existe.

----

Data | Responsável | Versão| Modificações |
--------- | ------| --------|  --------|
21/04/2018 | Geovanne Santos |   1.0   | Criação do caso de uso |
27/05/2018 | Geovanne Santos |   2.0   | refatorar o fluxo alternativo e básico, criação das regras de negócio |

#  [UC06] - Adquirir o plano premiun

## 1. Nome do Caso de Uso
- Adquirir o plano premiun

## 2.  Breve descrição
- O usuário deseja comprar o plano premiun, para ter acesso a mais funcionalidades.

## 3.  Atores
- Usuário free.

## 4.  Pré-Condição
- O usuário deve possuir uma conta free no spotify.
- Ter o aplicativo do Spotify instalado.
- Estar conectado à internet.
- Ter feito o login no aplicativo.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O usuário instala o spotify.
2. O usuário abre o aplicativo.
3. O sistema direciona pra página de início da conta.
4. O usuário acessa a página de experimentar conta premium.
5. O sistema direciona o usuário para página de colocar informações de compra.[FA01] [FA02] [FA03]
6. O usuário aceita o contrato padrão de plano premium(3 meses de premium por R$ 16.90, depois dos 3 meses vira  R$ 16.90 por mês) que deseja firmar e a forma de pagamento padrão, que é o cartão de crédito.
7. O usuário coloca as informações necessárias.
8. O sistema valida as informações.[FE02][FE01]
9. O sistema muda a conta de tipo free para tipo premium após o pagamento. [FE03]

## 5.2 Fluxos alternativos

FA01 - O usuário deseja adquirir o plano premium estudantil

1. O usuário acessa a página de planos premium alternativos.
2. O sistema direciona para a página de tipos de plano premiun.
3. O usuário escolhe o plano premium estudantil(R$ 8.50 por mês) e coloca as informações necessárias(inclusive a do cartão de crédito, que é a única forma de pagamento deste plano).
4. O sistema valida as informações.[FE02][FE01]
5. O sistema muda a conta de tipo free para tipo premium após o pagamento.[FE03]

FA02 - O usuário deseja adquirir o plano premium familiar e dividir o preço do plano com várias pessoas

1. O usuário acessa a página de planos premiun alternativos.
2. O sistema direciona para a página de tipos de plano premium.
3. O usuário escolhe o plano premium familiar(R$ 26.00 por mês, para 5 pessoas) e coloca as informações necessárias(inclusive a do cartão de crédito ou débito, que são as formas de pagamento deste plano).
4. O sistema valida as informações.[FE02][FE01]
5. O sistema muda a conte de tipo free para tipo premium após o pagamento.[FE03]

FA03 - O usuário deseja adquirir o plano premium comprando o plano que é pago por boleto

1. O usuário acessa a página de tipos de pagamento.
2. O sistema direciona para a página com as opções de pagamento.
3. O usuário acessa a opção de boleto.
4. O sistema mostra as opções(R$ 16,90 1 mês, R$ 49,00 3 mês, R$ 99,00 6 mês )
5. O usuário escolhe entre as três opções acima e coloca as informações necessárias.
6. O sistema valida as informações.[FE02][FE01]
7. O sistema gera o boleto
5. O sistema muda a conta de tipo free para tipo premium após o pagamento.[FE03]

## 5.3 Fluxos de Exceção
FE01 - Não ter acesso a internet durante a tentativa de adquirir um pacote premium
1. Aplicativo perder conexão com a internet
2. O sistema não abre a página de colocar informações de contrato.
3. O sistema permanece na página anterior com a mensagem de erro[M2].

FE02 - O usuário entra com as informações de estabelecer contrato premium inválidas:
1. O sistema identifica a informação inválida .
2. O sistema permanece na mesma página.
3. O sistema destaca o box com a informação inválida[M1].

FE03 - Usuário ao colocar as informações de contrato não paga de imediato o valor do contrato:
1. O sistema não muda de conta free para conta premium.


## 6 Mensagens
1. [M1] O dado da mensagem está inválido, por favor insira novamente o dado da mensagem.
2. [M2] Você está offline, por favor reestabeleça a conexão e tente novamente.

## Regras de Negócio

RN01
Descrição: Nome completo
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN02
Descrição: Data de nascimento
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN03
Descrição: E-mail
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN04
Descrição: CPF
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN05
Descrição: Número do telefone
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN06
Descrição: Complemento
Obrigatoriedade: Não
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN07
Descrição: Cidade
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN08
Descrição: CEP
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08 [FA03]-05

RN09
Descrição: Número do cartão
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA02]-03

RN10
Descrição: Senha do cartão
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA02]-03

RN10
Descrição: Estado
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA2]-08

RN10
Descrição: Comprovante de estudante
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FA01]-03

RN11
Descrição: Data de vencimento do cartão
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: [FB]07 [FA01]-03 [FA02]-03

---

Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

#  [UC06] - cadastro como perfil de artista

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

---

Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

#  [UC08] - Cadastro de usuário comum

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

---

Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

#  [UC09] - colocar a agenda de shows

## 1. Nome do Caso de Uso
- colocar a agenda de shows

## 2.  Breve descrição
- Usuário artista deseja divulgara agenda de shows no seu perfil.

## 3.  Atores
- Usuário artista.

## 4.  Pré-Condição
- O usuário deve ter o perfil artista.
- Ter o aplicativo do Spotify instalado.
- Ter feito o login.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário vai na parte de adicionar agenda de shows.
- Usuário coloca as informações necessárias(data e cidade).

## 5.2 Fluxos alternativos

- [FA01]Adicionar uma data e um local por cima de outro, devido a algum imprevisto.

## 5.3 Fluxos de Exceção
- [FE01] Tentar adicionar alguma agenda de shows não possuindo o perfil de artista.
- [FE02] Faltar com alguma informação da parte de shows.

## 6 Mensagens
- [M1] está faltanto um campo obrigatório. 

---

Data | Responsável | Versão|
--------- | ------| --------|
10/06/2018 | José Aquiles |   1.0   |

#  [UC10] - controle de reprodução

## 1. Nome do Caso de Uso
- controle de reprodução

## 2.  Breve descrição
- O Usuario pode controlar a reprodução que esta ativa em outros dispositivos.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- Ter acesso à internet.
- Ter aplicativo instalado.
- Estar logado no aplicativo.
- reprodução ativa em outro dispositivo.
- Ter conta premium do Spotify

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- usuário inicia o aplicativo.
- usuário acessa informações de reprodução.
- usuário altera volume da reprodução ativa.
- usuário muda a música da reprodução ativa.

## 5.2 Fluxos de Exceção
- [FE01] Não estar com reprodução ativa no dispositivo em uso.
- [FE02] perder sinal de internet.

---

Data | Responsável | Versão|
--------- | ------| --------|
10/06/2018 | José Aquiles |   1.0   |

#  [UC11] - criar estação

## 1. Nome do Caso de Uso
- criar estação

## 2.  Breve descrição
- O Usuario pode criar uma estação de rádio a partir de playlist, artista, musica entre outros

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- Conectado à internet
- logado na conta

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- Após acessar rádio
- O usuário clica na opção "Nova estação"
- O usuário insere o nome de uma música, um artista, um album ou uma playlist no campo de busca
- O usuário seleciona a música, artista, álbum ou playlist a qual gostaria de começar a estação
- O usuário tem acesso a estação
- O usuário passa a ter a estação salva em sua biblioteca

## 5.2 Fluxos de Exceção
- [FE01] internet parar de funcionar
- [FE02] aplicativo parar de funcionar
- [FE03] Celular desligar

----

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio |   1.0   |


#  [UC12] - Criar playlist

## 1. Nome do Caso de Uso
- Criar playlist

## 2.  Breve descrição
- Cria uma nova playlist que pode ser usada para adicionar músicas que o usuário desejar.

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
5. O usuário seleciona a opção Nova playlist.[FA01]
6. O sistema apresenta uma tela solicitando o nome da playlist, Imagem e descrição.
7. O usuário insere as informações requeridas e seleciona a opção criar.[FA01]
8. O sistema gera uma nova playlist.

## 5.2 Fluxos alternativos

FA01 - O usuário cancela a operação
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

## Regras de negócio

RN01
Descrição: Nome da playlist
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: FB06

RN02
Descrição: Descrição
Obrigatoriedade: Não
Passo​ ​do​ ​Fluxo: FB06

RN03
Descrição: Imagem
Obrigatoriedade: Não
Passo​ ​do​ ​Fluxo: FB06

---

Data | Responsável | Versão|
--------- | ------| --------|
11/08/2018 | José Aquiles |   1.0   |


#  [UC13] - divulgação de musicas próprias

## 1. Nome do Caso de Uso
- divulgação de musicas próprias

## 2.  Breve descrição
- O spotify divulga musicas de artistas que tem contrato com gravadora que tem parceria com spotify.

## 3.  Atores
- Usuário artista.
- Gravadora

## 4.  Pré-Condição
- Ser usuário "artista".
- Ter acesso a internet.
- Estar logado no aplicativo.
- Ter contrato com a gravadora.
- Ter o aplicativo Instalado. 

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. usuário acessa Spotify
2. usuário começa a usar o aplicativo
3. Gravadora divulga suas músicas

## 5.2 Fluxos de Exceção
FE01 - Perca de sinal com a internet

FE02 - Problemas com a gravadora

----

Data | Responsável | Versão|
--------- | ------| --------|
23/04/2018 | Geovanne Santos |   1.0   |

#  [UC14] - Editar foto de perfil de conta

## 1. Nome do Caso de Uso
- Editar foto de perfil de conta

## 2.  Breve descrição
- O usuário quer mudar a foto de perfil da sua conta.

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
- O usuário acessa a sua biblioteca.
- O usuário clica no boneco, que leva para a página do perfil.
- Clica em mudar foto, escolhe um arquivo e substitui.

## 5.2 Fluxos alternativos
- [FA01]
- colocar a figura do perfil sem nenhuma foto, só com a imagem padrão do aplicativo.

## 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

## 6 Mensagens
- [M1] Você talvez tenha perdido a conexão com a internet, tente mais tarde.

---

Data | Responsável | Versão|
--------- | ------| --------|
26/04/2018 | Eduardo Júnio |   1.0   |
27/05/2018 | Eduardo Júnio |   2.0   |

#  [UC15] - Excluir playlists
## 1. Nome do Caso de Uso
- Excluir playlists

## 2. Breve descrição
- Permite a exclusão de uma playlist selecionada pelo usuário.

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
5. O usuário seleciona uma playlist.[FA01]
6. O sistema apresenta as músicas salvas na playlist.
7. O usuário seleciona a opção apagar.[FA01]
8. O sistema exclui a playlist.

## 5.2 Fluxos alternativos

FA01 - O usuário cancela a operação
1. O usuário cancela a operação corrente.
2. O sistema redireciona o usuário para outra tela.

FA02 - O usuário não possui playlists salvas.
1. O usuário não possui playlists.
2. O sistema apresenta ao usuário a opção criar playlist.

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

---

Data | Responsável | Versão| Modificações |
--------- | ------| --------| --------|
21/04/2018 | Geovanne Santos |   1.0   | criação do caso de uso |
26/05/2018 | Geovanne Santos |   2.0   | refatoração do caso de uso |

#  [UC06] - Ficar em modo offline

## 1. Nome do Caso de Uso
- ficar em modo offline

## 2.  Breve descrição
- Usuário faz login no aplicativo e deseja reproduzir as músicas em modo offline para não gastar pacote de internet.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve ter o aplicativo do Spotify instalado.
- O usuário deve ter feito o login.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso começa quando o usuário abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo sem estar logado.
3. O usuário acessa a página de login e põem os dados de login.
4. O sistema valida os dados.
5. O usuário acessa sua conta no spotify.
6. O usuário acessa a página de configurações.
7. O usuário clica no botão do modo offline para ativar a função.

## 5.2 Fluxos alternativos

FA01 - O login do usuário já está feito no aplicativo
1. O fluxo alternativo começa quando o usuário abre o aplicativo.
2. O sistema exibe a tela da conta do usuário, na página de início.
3. O usuário acessa a página de configurações.
4. O usuário clica no botão do modo offline para ativar a função.

## 5.3 Fluxos de Exceção
- Não existe

## 6 Mensagens
- Não existe

## 7 Regras de Negócio
- Não existe

---

Data | Responsável | Versão|
--------- | ------| --------|
11/06/2018 | José Aquiles |   1.0   |


#  [UC17] - Informações de reprodução

## 1. Nome do Caso de Uso
- informações de reprodução

## 2.  Breve descrição
- Trazer informações sobre reprodução de músicas em andamento em outro dispositivo

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- aplicativo Instalado.
- Estar logado no Spotify.
- Ter acesso à internet.
- Spotify reproduzindo música em outro dispositivo. 

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. usuário inicia o aplicativo.
2. aplicativo alerta sobre reprodução ativa em outro dispositivo. [FA01]
3. usuário clica em música.
4. usuário acompanha reprodução ativa. 

## 5.2 Fluxos alternativos

FA01 - O usuário interrompe reprodução ativa em outro dispositivo
1. O usuário cancela a operação corrente.
2. O sistema redireciona o usuário para outra tela.


## 5.3 Fluxos de Exceção
FE01 - Não ter acesso a Internet durante o procedimento
1. O sistema informa "O spotify está offline"[M1].
2. A operação é interrompida.
3. O caso de uso se encerra.

## 6 Mensagens
- [M1] O spotify está offline.

----

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio |   1.0   |


#  [UC18] - Tornar Playlist secreta

## 1. Nome do Caso de Uso
- Tornar playlist secreta

## 2.  Breve descrição
- Permite ao usuário tornar uma playlist secreta para que apenas o mesmo possa visualiza-la

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
5. O usuário seleciona a opção Playlists.[FA02]
6. O sistema lista todos as playlists salvas na biblioteca do usuário [FA01]
7. O usuário seleciona a playlist que deseja tornar secreta.
8. O sistema apresenta o conteúdo da playlist e o menu de gerenciamento da playlist.
9. O usuário seleciona a opção Tornar secreta.

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

---

Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

#  [UC06] - Mudar o tipo de perfil

## 1. Nome do Caso de Uso
- Mudar o tipo de perfil

## 2.  Breve descrição
- O usuário comum deseja se tornar usuário artista.

## 3.  Atores
- Usuário comum.

## 4.  Pré-Condição
- O usuário deve ser comum.
- Ter o aplicativo desktop do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário clica em requerir o perfil artista.
- Usuário coloca as informações necessárias, tais como a agência que irá distribuir a música para o aplicativo, o Twitter e outros.
- O usuário espera o aplicativo autenticar o perfil requerido para usar as funcionalidades novas.

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

- [FE03] Usuário tenta criar um perfil fake:
- O sistema não irá autorizar o requerimento do perfil.


## 6 Mensagens
- [M1] O dado da mensagem está inválido, por favor insira novamente o dado da mensagem.
- [M2] O requerimento do perfil não foi autorizado.

---

Data | Responsável | Versão|
--------- | ------| --------|
11/06/2018 | José Aquiles |   1.0   |


#  [UC17] - Mudar Reprodução ativa

## 1. Nome do Caso de Uso
- Mudar reprodução ativa

## 2.  Breve descrição
- Mudar o dispositivo com reprodução ativa. 

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- aplicativo Instalado.
- Estar logado no Spotify.
- Ter acesso à internet.
- Spotify reproduzindo música em outro dispositivo. 

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. usuário inicia o aplicativo
2. usuário acessa informações de reprodução.
3. usuário acessa dispositivos disponíveis
4. usuário seleciona dispositivo em uso [FA01].
5. usuário ouve música no dispositivo em uso. 

## 5.2 Fluxos alternativos

FA01 - O usuário interrompe reprodução ativa em outro dispositivo
1. O usuário cancela a operação corrente.
2. O sistema redireciona o usuário para outra tela.


## 5.3 Fluxos de Exceção
FE01 - Não ter acesso a Internet durante o procedimento
1. O sistema informa "O spotify está offline"[M1].
2. A operação é interrompida.
3. O caso de uso se encerra.

## 6 Mensagens
- [M1] O spotify está offline.

---

# Integração com redes Sociais

<object width="700" height="600" data="../diagrama_de_uso/caso-integracao_redes.png"></object>

# Indice Analítico

1. Nome do Caso de Uso
    1. Breve descrição
2. Fluxo de eventos
    1. Fluxo Básico
    2. Fluxos Alternativos
        1. Visualizar Caderno de Acordo com a Cronologia e Categoria das Tarefas
    3. Fluxos de Exceção
        1. Visualizar Caderno Inexistente
3. Requisitos Especiais
    1. Primeiro Requisito Especial
4. Condições Prévias   
    1. Condição Prévia Um
5. Mensagens


# Especificação de Caso de Uso <Visualizar Caderno>

## 1. #UC1 – Integração de Redes sociais

### 1.1 Breve Descrição

Descrição - Este caso de uso permite ao usuário facilidade de compartilhamento, usabilidade, podendo compartilhar playlists e músicas, entre outras funcioalidades.

## 2. Fluxo de Eventos

### 2.1 Fluxo Básico
1. O fluxo básico começa quando o usuário acessa a plataforma Spotify e começa a utilizar o aplicativo (#R21 – Navegar (de acordo com o documento de Especificação suplementar)) .
1. O usuário acessa o Aplicativo.
2. O usuário navega dentro do aplicativo. [RF 21]
3. O usuário tem diversas opções dentro das funcionalidades disponíveis.
4. O usuário acessa uma playlist [RF 03] ou uma música
5. Dentro dessa funcionalidade ele pode compartilhar uma playlist ou músicas entre as redes sociais integradas, como o whatsapp e facebook.

### 2.2 Fluxo Alternativo
1. Buscar uma música sem necessariamente acessar uma playlist.
    1. O usuário acessa o Aplicativo.
    2. O usuário navega dentro do aplicativo. [RF 21]
    3. O busca por uma música em especifica.
    4. Dentro dessa funcionalidade ele pode compartilhar uma playlist ou músicas entre as redes sociais integradas, como o whatsapp e facebook.

### 2.3 Fluxos de Exceção
1. Erro na integração com outra rede social
    1. O usuário solicita alguma funcionalidade que exige dados de outra rede social.
    2. O sistema tenta o acesso e apresenta erro.
    3. O sistema volta para a página anterior.

## 3. Requisitos Especiais
 - Nenhum requisito especial identificado.

## 4. Condições Prévias
  - Estar conectado com a internet.
  - Possuir acesso as outras redes sociais.

## 5. Mensagens
[MES01] “Erro ao conectar ao aplicativo”.

---

Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

#  [UC23] - postar uma música

## 1. Nome do Caso de Uso
- postar uma música

## 2.  Breve descrição
- Usuário artista deseja postar uma música no aplicativo spotify.

## 3.  Atores
- Usuário artista.

## 4.  Pré-Condição
- O usuário deve ser ter o perfil artista.
- Ter o aplicativo do Spotify instalado.
- Ter colocado a música no site da gravadora que ela tem contrato.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário artista instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário vai no site da gravadora(distribuidora) e posta a música no site deles.
- A gravadora direciona a música pro aplicativo spotify.

## 5.2 Fluxos alternativos

- Não existe

## 5.3 Fluxos de Exceção
- [FE01]Tentar postar uma música que já existe.

## 6 Mensagens
- [M1]Esta música já existe ou não de sua autoria.

----

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio | 1.0 |

#  [UC24] - Compartilhar playlists

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

---

Data | Responsável | Versão|
--------- | ------| --------|
23/04/2018 | Geovanne Santos |   1.0   |
27/05/2018 | Eduardo Júnio |   2.0   |

#  [UC26] - Renomear playlists

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

---

Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

#  [UC27] - Sair do aplicativo

## 1. Nome do Caso de Uso
- Sair do aplicativo

## 2.  Breve descrição
- Usuário sai da conta atual.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Estar logado no aplicativo.
- Ter o aplicativo do Spotify instalado

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário faz o login spotify.
- O usuário é direcionado a parte de usuário.
- O usuário sai da conta.

---

Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |
25/05/2018 | Lucas Cunha | 2.0 |

#  [UC29] - Fazer login

## 1. Nome do Caso de Uso
- Fazer Login

## 2.  Breve descrição
- Autentica o usuário no aplicativo dando a ele acesso às informações de sua conta e as funcionalidades.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso começa quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo sem estar logado.
3. O usuário acessa a tela de login.
4. O sistema exibe campos de entrada para Email/Nome de Usuário e senha.
5. O usuário digita o seu Email/Nome de Usuário e sua senha. [FA01]
6. O usuário envia os dados.
7. O sistema autentica o usuário. [FE 01],[FE02]


## 5.2 Fluxos alternativos

FA01 - O usuário esqueceu a senha
1. Logo após digitar o Email/Nome de Usuário, o usuário seleciona opção para resetar a senha.
2. O sistema envia um e-mail ao ator para trocar a senha.
3. O usuário redefine sua senha.
4. O fluxo principal é recomeçado.

## 5.3 Fluxos de Exceção
FE01 - Não ter acesso a Internet durante o procedimento e sem login posterior no mesmo aparelho.
1. O sistema informa "Verifique as configurações de aplicativo"[M2].
2. A operação é interrompida.
3. O caso de uso se encerra.

FE02 - Preenchimento incorreto dos dados
1. O sistema informa "O e-mail e senha inseridos não correspondem a nenhuma conta do Spotify. Tente de novo."[M1]


## 6 Mensagens
- [M1] O e-mail e senha inseridos não correspondem a nenhuma conta do Spotify. Tente de novo.
- [M2] Verifique as configurações de aplicativo.

## Regras de Negócio

RN01
Descrição: E-mail
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: FB05

RN02
Descrição: Nome de Usuário.
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: FB05

RN03
Descrição: Senha​ ​ de​ ​ no​ ​ mínimo​ ​ 6 caracteres.
Obrigatoriedade: Sim
Passo​ ​do​ ​Fluxo: FB05

---

Data | Responsável | Versão|
--------- | ------| --------|
23/04/2018 | Geovanne Santos |   1.0   |

#  [UC30] - Ver gráficos de rendimento sobre seus álbuns

## 1. Nome do Caso de Uso
- Ver gráficos de rendimento sobre seus álbuns.

## 2.  Breve descrição
- O usuário artista deseja acessar os gráficos que mostram o desempenho dos seus álbuns e músicas no aplicativo.

## 3.  Atores
- Usuário artista.

## 4.  Pré-Condição
- O usuário deve ser usuário artista.
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativo e faz o login.
- O usuário acessa a parte de gráficos e verifica o número de acessos ao perfil, as músicas mais populares.

## 5.2 Fluxos alternativos

- [FA01]
- O usuário acessa o site spotify.
- O usuário faz o login.
- O usuário clica na parte de gráficos e verifica as informações disponíveis.

## 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas ou estarão desatualizadas.

## 6 Mensagens
- Não existe.

----

Data | Responsável | Versão|
--------- | ------| --------|
26/04/2018 | Eduardo Júnio |   1.0   |

#  [UC32] - Download de playlists
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

---

Data | Responsável | Versão|
--------- | ------| --------|
23/04/2018 | Geovanne Santos |   1.0   |

#  [UC02] - mudar de senha

## 1. Nome do Caso de Uso
- Mudar de senha

## 2.  Breve descrição
- O usuário deseja mudar de senha.

## 3.  Atores
- Usuário cadastrado.

## 4.  Pré-Condição
- O usuário deve ser cadastrado.
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário acessa o site spotify.
- O usuário faz o login.
- O usuário acessa a página de mudar senha.
- Usuário digita as informações necessárias que o site irá pedir(senha atual, nova senha, repetir nova senha).

## 5.2 Fluxos alternativos

- [FA01]
- O usuário não consegue fazer o login no spotify, com as informações que colocou.
- O usuário clica no botão de ajuda do spotify.
- O usuário é direcionado a uma nova tela de redefenir senha.
- Digita o email da sua conta spotify.
- Vá no seu email e clique no email que o spotify te enviou, ele te direcionará para uma página.
- Coloque as informações necessárias(nova senha, confirmação de nova senha).

## 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

- [FE02] Usuário digita um email não válido, ou seja, que não pertence a sua conta:
- O sistema identifica a resposta inválida .
- O sistema dispara uma mensagem de erro.
- O sistema fica na mesma página.

## 6 Mensagens
- [M1] Este endereço de email ou nome de usuário não pertence a nenhuma conta spotify.

--

|Data|Versão|Descrição|Autor|
|----|-----|----|------|
|18/04/2018|1.0|Especificação da UC08|Geovanne Santos|

<h1>RF14 - Editar dados de conta</h1>
<h4>Descrição:</h4>
Editar as informações pessoais do usuário.<br />
<h4>Atores:</h4>
Usuário cadastrado<br />
<h4>Pré-condição:<br /></h4>
O usuário deve possuir uma conta no spotify.<br />

<h4>Fluxo Principal:</h4>
<ul>
  <li>Faz o login.</li>
  <li>O usuário vai na página web do site.</li>
  <li>O usuário clica em editar perfil.</li>
  <li>Modifica os dados.</li>
  <li>Clica em salvar.</li>
</ul>

<h4>Fluxos Alternativos</h4>
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

<h4>Fluxo de Exceção:</h4>
<h6>[FE01] Tenta modificar os dados que não sejam a foto de perfil pelo aplicativo:</h6>
O aplicativo não possui essa funcionalidade .

---

Data | Responsável | Versão|
--------- | ------| --------|
21/04/2018 | Geovanne Santos |   1.0   |

#  [UC39] - atualizar biografia do artista

## 1. Nome do Caso de Uso
- atualizar biografia do artista

## 2.  Breve descrição
- O artista deseja mudar o conteúdo da biografia que está presente no seu perfil de artista.

## 3.  Atores
- Usuário artista.

## 4.  Pré-Condição
- O usuário deve ser usuário artista.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.
- Ter feito o login.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

- O usuário instala o spotify.
- O usuário abre o aplicativa e faz o login.
- O usuário vai na aba de biografia eclica em editar.
- Usuário faz a modificação e salva.

## 5.2 Fluxos alternativos

- Não existe.

## 5.3 Fluxos de Exceção
- [FE01]
- Aplicativo perder conexão com a internet
- O sistema informa que o aplicativo está offline.
- As funcionalidades não podem ser acessadas.

- [FE02] Usuário ainda não tem perfil de artista autenticado:
- O sistema não deixará o usuário fazer nenhum ação que envolva o perfil artista até ser validado.

## 6 Mensagens
- [M1] A modificação da biografia não foi efetuada, sua conexão caiu.

----

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio | 1.0 |

#  [UC43] - Compartilhar podcasts

## 1. Nome do Caso de Uso
-  Compartilhar podcasts

## 2.  Breve descrição
- Permite ao usuário compartilhar podcasts em outras redes sociais.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.
- Possuir conta na rede social que deseja compartilhar o podcast.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso inicia quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo.
3. O usuário seleciona a opção Acessar biblioteca.
4. O sistema exibe as opções de funcionalidades disponíveis na biblioteca.
5. O usuário seleciona a opção Podcasts.[FA02]
6. O sistema lista todos os podcasts salvos na biblioteca.[FA01]
7. O usuário seleciona o podcast que deseja compartilhar e seleciona a opção compartilhar.[FA02]
8. O sistema apresenta as opções de compartilhamento.[FA02]
9. O usuário seleciona a rede social que deseja compartilhar o podcast.[FA02]
10. O sistema compartilha o podacast.

## 5.2 Fluxos alternativos

FA01 - Usuário não possui podcasts salvos
1. O sistema apresenta a opção Ir para navegar.
2. O usuário seleciona a opção apresentada.
3. O sistema apresenta sugestões de podcasts que podem ser acessados pelo usuário.
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

---

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio | 1.0 |

#  [UC44] - Compartilhar programa de vídeo

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

---

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio |   1.0   |


#  [UC47] - Acessar podcasts na biblioteca

## 1. Nome do Caso de Uso
- Acessar podcasts na biblioteca

## 2.  Breve descrição
- Apresenta a lista de podcasts salvos na biblioteca do usuário.

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
5. O usuário seleciona a opção podcasts.[FA02]
6. O sistema lista todos os podcasts salvos na biblioteca do usuário [FA01]

## 5.2 Fluxos alternativos

FA01 - O usuário não possui podcasts salvos
1. O sistema apresenta uma opção de "Ir para navegar".
2. O usuário seleciona a opção apresentada.
3. O sistema apresenta categorias de podcasts e episódios em destaque.
4. O usuário seleciona alguma das opções e a adiciona à sua biblioteca.
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

--

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio |   1.0   |


#  [UC48] - Acessar podcasts na biblioteca

## 1. Nome do Caso de Uso
- Acessar vídeos na biblioteca

## 2.  Breve descrição
- Apresenta a lista de vídeos salvos na biblioteca do usuário.

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
5. O usuário seleciona a opção vídeos.[FA02]
6. O sistema lista todos os vídeos salvos na biblioteca do usuário [FA01]

## 5.2 Fluxos alternativos

FA01 - O usuário não possui vídeos salvos ou sendo seguidos
1. O sistema apresenta a opção "Ir para navegar".
2. O usuário seleciona a opção apresentada.
3. O sistema apresenta programas em destaque e episódios em destaque.
4. O usuário seleciona alguma das opções e a adiciona à sua biblioteca.
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

----

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio |   1.0   |


#  [UC55] - Acessar álbuns salvos na biblioteca

## 1. Nome do Caso de Uso
- Acessar álbuns salvos na biblioteca

## 2.  Breve descrição
- Permite ao usuário acessar os álbuns salvos por ele.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso inicia quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo.
3. O usuário seleciona a opção Acessar biblioteca.
4. O sistema exibe as opções de funcionalidades disponíveis na biblioteca.
5. O usuário seleciona a opção Álbuns.[FA02]
6. O sistema lista todos os álbuns salvos na biblioteca do usuário [FA01]

## 5.2 Fluxos alternativos

FA01 - O usuário não possui álbuns salvos
1. O sistema apresenta a opção Ir para navegar.
2. O usuário seleciona a opção apresentada.
3. O sistema apresenta categorias (podcasts, paradas, gêneros e momentos, lançamentos e mais, lista com com os melhores lançamentos e novos álbuns e singles).
4. O usuário seleciona alguma das opções e a adiciona aos seus álbuns.
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

---

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio | 1.0 |

#  [UC56] - Acessar artistas seguidos

## 1. Nome do Caso de Uso
- Acessar artistas seguidos

## 2.  Breve descrição
- Permite ao usuário acessar a lista de artistas que estão sendo seguidos.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso inicia quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo.
3. O usuário seleciona a opção Acessar biblioteca.
4. O sistema exibe as opções de funcionalidades disponíveis na biblioteca.
5. O usuário seleciona a opção Artistas.[FA02]
6. O sistema lista todos os Artistas que estão sendo seguidos.[FA01]

## 5.2 Fluxos alternativos

FA01 - O usuário não possui artistas salvos
1. O sistema apresenta a opção Ir para navegar.
2. O usuário seleciona a opção apresentada.
3. O sistema apresenta sugestões de artistas.
4. O usuário seleciona um artista ou usa a funcionalidade para buscar o artista desejado.
5. O usuário ativa a funcionalidade seguir artista.
6. O fluxo básico pode ser retomado.

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

----


Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio | 1.0 |

#  [UC57] - Acessar mídias tocadas recentemente

## 1. Nome do Caso de Uso
- Acessar mídias tocadas recentemente

## 2.  Breve descrição
- Permite ao usuário acessar o conteúdo de mídia recentemente reproduzido.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso inicia quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo.
3. O usuário seleciona a opção Acessar biblioteca.
4. O sistema exibe as opções de funcionalidades disponíveis na biblioteca.
5. O usuário seleciona a opção Tocados recentemente.[FA02]
6. O sistema lista todo o conteúdo de mídia reproduzido recentemente.[FA01]

## 5.2 Fluxos alternativos

FA01 - Usuário recente do spotify
1. O sistema apresenta a opção Ir para navegar.
2. O usuário seleciona a opção apresentada.
3. O sistema apresenta sugestões de conteúdos que podem ser acessados pelo usuário.
4. O usuário acessa o conteúdo desejado.
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

---

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio | 1.0 |

#  [UC58] - Acessar Daily Mix

## 1. Nome do Caso de Uso
-  Acessar Daily Mix

## 2.  Breve descrição
- Permite acessar conteúdos de mídia recomendados pelo spotify ao usuário.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso inicia quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo.
3. O usuário seleciona a opção Acessar biblioteca.
4. O sistema exibe as opções de funcionalidades disponíveis na biblioteca.
5. O usuário seleciona a opção Seu Daily Mix.[FA02]
6. O sistema lista todo o conteúdo de mídia recomendado ao usuário.[FA01]

## 5.2 Fluxos alternativos

FA01 - Usuário recente do spotify
1. O sistema apresenta a opção Ir para navegar.
2. O usuário seleciona a opção apresentada.
3. O sistema apresenta sugestões de conteúdos que podem ser acessados pelo usuário.
4. O usuário acessa o conteúdo desejado.
5. O sistema gera recomendações de conteúdos ao usuário.
6. O fluxo básico pode ser retomado.

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

---

Data | Responsável | Versão|
--------- | ------| --------|
27/05/2018 | Eduardo Júnio | 1.0 |

#  [UC59] - Compartilhar música

## 1. Nome do Caso de Uso
-  Compartilhar música

## 2.  Breve descrição
- Permite ao usuário compartilhar músicas com outras redes sociais.

## 3.  Atores
- Usuário.

## 4.  Pré-Condição
- O usuário deve possuir uma conta no spotify.
- Ter o aplicativo do Spotify instalado
- Estar conectado à internet.
- Possuir conta na rede social que deseja compartilhar a música.

## 5.  Fluxo de eventos

### 5.1 Fluxo básico

1. O caso de uso inicia quando o ator abre o aplicativo.
2. O sistema exibe a tela inicial do aplicativo.
3. O usuário seleciona a opção Acessar biblioteca.
4. O sistema exibe as opções de funcionalidades disponíveis na biblioteca.
5. O usuário seleciona a opção músicas.[FA02]
6. O sistema lista todas as músicas salvas.[FA01]
7. O usuário seleciona a música que deseja compartilhar e seleciona a opção compartilhar.[FA02]
8. O sistema apresenta as opções de compartilhamento.
9. O usuário seleciona a rede social que deseja compartilhar o conteúdo.[FA02]
10. O sistema compartilha a música.

## 5.2 Fluxos alternativos

FA01 - Usuário não possui músicas salvas
1. O sistema apresenta a opção Ir para navegar.
2. O usuário seleciona a opção apresentada.
3. O sistema apresenta sugestões de conteúdos que podem ser acessados pelo usuário.
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