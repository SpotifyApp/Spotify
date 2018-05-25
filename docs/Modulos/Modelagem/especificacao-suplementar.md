4# Histórico da Revisão

| Data | Versão | Descrição | Autor |
| --- | --- | --- | --- |
| 17/04/2018 | 0.1 | Criação, funcionalidade, interfaces de comunicações, interfaces de Software, interfaces de hardware, interfaces de usuário, usabilidade | Eduardo Júnio |
| 17/04/2018 | 0.2 | Finalidade, Definições e acrônimos e abreviações | Renato Valério |
| 17/04/2018 | 0.3 | Requisitos de usabilidade, Requisitos de Sistema de Ajuda e de Documentação de Usuário On-line, Componentes de Terceiros, Requisitos de Licenciamento, Observações Legais, de Direitos Autorais etc | Amanda Bezerra |
| 17/04/2018 | 0.4 | --- | Geovanne Santos |

# 1.Introdução
## 1.1 Finalidade
<p align="justify">O objetivo deste documento de especificação suplementar é detalhar todos os aspectos não abordados diretamente nos documentos de visão, caso de uso ou arquitetura. São estes aspectos, legais e reguladores, como as normas estabelecidas para bom funcionamento do sistema, atributos de qualidade, como padrões de usabilidade, confiabilidade, desempenho e suportabilidade.

## 1.2 Escopo
<p align="justify">Esta especificação suplementar documenta aspectos do Spotify, serviço de streaming desenvolvido e mantido pela empresa Spotify AB.
O software de música permitirá que os assinantes possam ouvir qualquer álbum e música de todos os artistas no qual a gravadora tenha contrato com a empresa spotify.

## 1.3 Definições, Acrônimos e Abreviações  
<p align="justify">Alguns termos utilizados neste documento, são derivados de outra língua, possui origem estrangeira, são abreviações ou acrônimos. Os mais relevantes são os seguintes:

+ **Streaming**: streaming ou Broadcast é o nome da transmissão de áudio e/ou vídeo pela internet, tecnologia esta que permite a transmissão de áudio e vídeo sem que seja necessário fazer o download de todo o conteúdo a ser transmitido, antes de ouvir ou assistir, como era feito antigamente, a transmissão do conteúdo é feita de modo contínuo, ou seja, enquanto a pessoa está ouvindo/assistindo.
+ **Broadcast**: broadcasting (do inglês to broadcast, "transmitir") é um método de transferência de mensagem para todos os receptores simultaneamente.
+ **Freemium**: Modelo de negócios baseado em planos, onde existe um plano gratuito com algumas funcionalidades, que servem para captação de usuários, e que influencia a migração para o plano “Premium” que possui acesso as outras funcionalidades e geralmente é pago.  


## 1.4 Referências
+ “Broadcasting”. Disponível [aqui](https://pt.wikipedia.org/wiki/Broadcasting_)
+ “Streaming”. Disponível [aqui](https://www.sitehosting.com.br/streaming/)
+ “Spotify - Integrações”. Disponível [aqui](https://support.spotify.com/br/using_spotify/app_integrations/)
+ “Spotify - Carros” Disponível [aqui](https://support.spotify.com/br/listen_everywhere/in_the_car/)
+ “Termos e Condições de Uso do Spotify”. Disponível [aqui](https://www.spotify.com/br/legal/end-user-agreement/)
+ “Suporte - Spotify”. Disponível [aqui](https://support.spotify.com/br/)

## 1.5 Visão Geral
<p align="justify">Essa especificação define os requisitos não-funcionais do sistema, como confiabilidade, usabilidade, desempenho e suportabilidade, bem como os requisitos funcionais comuns a vários casos de uso.

# 2. Funcionalidade
<p align="justify">Abaixo apresentamos uma lista com os requisitos funcionais,  alguns desses serão abordados nos diagramas de caso de uso.

## Requisitos funcionais

 Identificador | Funcionalidade
 --- | ---
RF 01 | Acessar biblioteca
RF 02 | Acessar opções de busca
RF 03 | Acessar playlists
RF 47 | Acessar podcasts na biblioteca
RF 04 | Acessar rádio
RF 48 | Acessar videos na biblioteca
RF 50 | Alertar Reprodução Ativa
RF 38 | Atualizar biografia do artista
RF 05 | Adicionar música a uma playlist
RF 06 | Adquirir o plano premiun
RF 32 | Ativar o status de transmissão(permitir outros apps verificarem o que está ouvindo)
RF 33 | Atualizar a foto do álbum
RF 07 | Cadastro com perfil de artista
RF 08 | Cadastro de usuário comum
RF 09 | Colocar a agenda de shows
RF 51 | Controlar Músicas/Playlists através de outros Dispositivos
RF 52 | Controlar Reprodução Ativa
RF 53 | Controlar Volume em dispositivo secundário
RF 10 | Controle de reprodução.
RF 11 | Criar estação
RF 12 | Criar playlist
RF 43 | Compartilhar podcasts
RF 44 | Compartilhar programas de videos
RF 13 | Comprar plano de divulgação de músicas próprias
RF 34 | Configurar o volume
RF 32 | Download de playlists
RF 14 | Editar foto de pefil conta
RF 37 | Editar dados de conta
RF 55 | Efetuar Login por dispositivo secundário
RF 15 | Excluir playlist
RF 29 | Fazer login
RF 16 | Ficar em modo offline
RF 17 | Informações de reprodução
RF 35 | Importar músicas do seu celular para o aplicativo
RF 21 | Integração redes sociais
RF 49 | Listar Dispositivos Disponíveis
RF 19 | Mudar o tipo de perfil
RF 36 | Mudar senha
RF 20 | Mudar reprodução ativa
RF 22 | Ouvir lançamentos
RF 18 | Ocultar playlist
RF 23 | Postar uma música
RF 39 | Procurar playlist
RF 24 | Compartilhar playlists
RF 25 | Seguir artistas
RF 26 | Renomear playlists
RF 45 | Reproduzir episodios de podcasts
RF 46 | Reproduzir videos
RF 27 | Sair do aplicativo
RF 28 | Seguir amigos para conhecer o que eles ouvem
RF 31 | Salvar músicas
RF 41 | Seguir podcasts
RF 42 | Seguir programas de videos
RF 40 | Suporte técnico
RF 30 | Ver gráficos de rendimento sobre seus álbuns


## Requisitos não funcionais

|Identificador | Descrição
|--- | ---
|RNF 01|sistema de autenticação de usuário(Segurança)
|RNF 02|serviço de busca(base de dados)
|RNF 03|telas de interação responsivas(usabilidade)
|RNF 04|integração spotify e facebook()
|RNF 05|Interface simples e interativa ao usuário (usabilidade)
|RNF 06|vinhetas durante a programação musical para quem está no modelo “Free”
|RNF 07|Limitações de uso ao plano gratuito(usabilidade-controle de liberdade de usuário)
|RNF 08| Vincular contas com PSN.

## Requisitos para plataformas específicas

Identificador | Dispositivos | Modelo | Sistema operacional
--- | --- | --- | ---
RNF 01 | Iphone | iPhone 4S ou superior | iOS 9 ou superior. 100 MB de espaço livre
RNF 02|Ipad | iPad 2 ou superior | iOS 9 ou superior. 100 MB de espaço livre
RNF 03 | Ipod | iPod Touch de 5ª geração ou superior. | iOS 9 ou superior. 100 MB de espaço livre
RNF 04 | Smartphones Android | Qualquer dispositivo | Android OS 4.0.3 ou superior. 500 MB de espaço livre
RNF 05 | Tablets Android | Qualquer dispositivo | Android OS 4.0.3 ou superior. 500 MB de espaço livre
RNF 06 | Mac | Qualquer dispositivo | OS X 10.9 ou superior
RNF 07 | Windows |Qualquer dispositivo |Windows 7 ou superior
RNF 08 | Safari | Qualquer dispositivo | Versão 6 ou superior.
RNF 09 | Internet Explorer | Qualquer dispositivo | Versão 10 ou superior.
RNF 10 | Google Chrome | Qualquer dispositivo | Última versão
RNF 11 | Mozilla Firefox | Qualquer dispositivo | versão mais recente ou imediatamente anterior
RNF 12 | Opera | Qualquer dispositivo| 12 ou superior.
RNF 13 | Yandex | Qualquer dispositivo | 1 ou superior.
RNF 14 | PS4 | 94 MB de espaço livre.


# 3. Usabilidade
## 3.1 Facilidade de uso
<p align="justify">Os recursos e funcionalidades do serviço devem apresentar-se de forma intuitiva para que o usuário possa facilmente navegar por eles, não sendo necessário a realização de qualquer tipo de treinamento prévio por parte do usuário.

## 3.2 Mensagens de Erro
<p align="justify">O serviço deve apresentar mensagens de erro de forma clara e objetiva, localizadas próximas ao conteúdo ou ação que motivou o erro.

## 3.3  Eficiência
<p align="justify">O sistema deve fornecer rápido acesso a qualquer funcionalidade.

## 3.4 Consistência e padronização
<p align="justify">O sistema deve manter a maior parte da interface a mesma para cada tipo de usuário, apenas adicionando alguns detalhes sobre a mesma de acordo com o nível de cada tipo de usuário.

## 3.5 Design simples
<p align="justify">O sistema deve ter ícones intuitivos.
Para cada tipo de usuário haverá um certo nível de funcionalidades disponíveis

# 4. Confiabilidade
## 4.1 Disponibilidade
O sistema estará disponível no modo 24/7.

## 4.2 Suportabilidade
O sistema deve suportar 4 bilhões de usuários ativos simultaneamente.

## 4.3 Direitos autorais
* O sistema deve garantir que os direitos autorais dos artistas seja preservado;
* O sistema deve oferecer suporte para que o usuário possa realizar denúncias ao se deparar com conteúdos que violem direitos de propriedade intelectual ou conteúdos que sejam ofensivos.

## 4.4 Segurança e Privacidade
* O sistema deve assegurar a segurança e privacidade dos dados gerados, armazenando senhas e dados sensiveis de forma segura.
* O sistema deve ser transparente quanto as informações coletadas referentes a dados pessoais do usuário e preferencias de conteudo e fornecer ao usuario a possibilidade de ajustar a visibilidade de tais informações.
* O sistema deve fornecer ao usuário controle sobre o conteúdo de comunicação que irá receber, como notificações e e-mails.

# 5. Desempenho
## 5.1 Tempo de resposta
<p align="justify">O aplicativo tem de responder as ações do usuário de imediato, como passar música, pausar, procurar por algum artista . Agora situações de casos de uso mais específicos, como a autenticação do perfil de artista, será relatado em um documento individual, assim como seu tempo de execução particular.

## 5.2 Volume de assinantes
<p align="justify">O sistema será capaz de suportar 4 bilhões de usuários ativos simultaneamente, tanto que em 2018 o aplicativo chegou a marca de 140 milhões de usuários .

## 5.3 Modo de degradação
<p align="justify">Se o sistema estiver sofrendo com algo que degrade o aplicativo, como a internet com sinal fraco, terá páginas que não serão carregadas, mas a maioria delas funcionarão da mesma forma, com apenas uma espera de alguns segundos a mais para aparecer as informações requeridas .

## 5.4 Utilização de recursos

+ iOS 9 ou superior.
100 MB de espaço livre
+ iOS 9 ou superior.
100 MB de espaço livre
+ iOS 9 ou superior.
100 MB de espaço livre
+ Android OS 4.0.3 ou superior.
500 MB de espaço livre
+ Android OS 4.0.3 ou superior.
500 MB de espaço livre
+ OS X 10.9 ou superior
+ Windows 7 ou superior
+ Versão 6 ou superior.


# 6. Suportabilidade
## 6.1 Software do assinante
<p align="justify">O assinante será capaz de utilizar o sistema através de um aplicativo disponível para android e ios. Não será necessário que nenhum software personalizado resida no smartphone do assinante. Estes são os requisitos de sistema para usar o Spotify e acessar seu conteúdo por meio do aplicativo

Dispositivo | Modelo
-- | --
Iphone | iPhone 4S ou superior
Ipad  | iPad 2 ou superior
Ipod | iPod Touch de 5ª geração ou superior
Smartphones Android | Qualquer dispositivo
Tablets Android | Qualquer dispositivo
Mac | Qualquer dispositivo


# 7. Restrições de Design
## 7.1 Restrição de Design Um
<p align="justify">O sistema deverá ser disponibilizado em diversas línguas, quando o usuário mudar o idioma do celular o aplicativo também se modificará.

## 7.2 Responsividade
<p align="justify">O sistema deverá se ajustar de forma responsiva, ou seja, ajustando todo o conteúdo da tela à plataforma que o usuário estiver utilizando, android ou ios.

## 7.3 Restrição de Design Três
<p align="justify">Os cincos escopos de telas principais do aplicativo deverão estar na parte de baixo do aplicativo, elas são: início, navegar, buscar, rádio e sua biblioteca.

## 7.4 Restrição de Design Quatro
<p align="justify">As opções de compartilhamento deverão ser com o símbolo da rede social na qual se deseja compartilhar algo.

## 7.5	Restrição de Design Cinco
<p align="justify">Antes do usuário poder ver as funcionalidades do aplicativo, terá que ter uma tela inicial com a opção de login e cadastro.

## 7.6 Restrição de Design Seis
<p align="justify">O botão de compartilhamento de música deverá ser colocado abaixo da foto da música no canto direito, assim como a opção de adicionar a música sua biblioteca será colocada abaixo da foto da música no canto esquerdo.

## 7.7 Restrição de Design Sete
<p align="justify">O nome da página sempre estará no topo do layout, se a página do aplicativo está na parte de busca, no topo da tela estará escrito busca.

# 8. Requisitos de Sistema de Ajuda e de Documentação de Usuário On-line
<p align="justify">O serviço deverá possuir uma seção destinada a ajudar o usuário a utilizar o serviço, responder suas dúvidas e encontrar soluções. Esta seção deverá disponibilizar:
+ Área de busca para encontrar soluções para as questões mais frequentes
+ Tutoriais claros e objetivos de como o usuário pode utilizar os recursos do serviço
+ Fórum para que os usuários possam interagir e compartilhar soluções e ideias

# 9. Componentes de Terceiros
<p align="justify">Devido a grande quantidade de softwares de terceiros utilizados pelo serviço Spotify, não cabe a esta especificação suplementar descrever todas as restrições e informações de licenciamento, que deverão ser reunidas em documento próprio a ser disponibilizado no serviço em área de fácil acesso ao usuário.

# 10. Interfaces
## 10.1 Interfaces de Usuário
<p align="justify">O usuário interage com o sistema por meio das interfaces. Abaixo apresentamos alguns exemplos de interfaces disponíveis aos usuários.
+ Tela onde o usuário pode fazer Login.
+ Tela onde o usuário pode se cadastrar.
+ Tela inicial onde o usuário pode escolher por qual funcionalidade navegar.

## 10.2 Interfaces de Hardware
<p align="justify">O software oferece suporte aos dispositivos apresentados abaixo.
+ Smartphones.
+ Computadores Notebooks.
+ Computadores Desktop.
+ Carros
+ Videogames
+ Televisores

## 10.3 Interfaces de Software
<p align="justify">O Spotify possui integrações com outros softwares e serviços, abaixo apresentamos alguns desses

+ Integração com o waze
+ Playlists em grupo com o Messenger
+ Last.fm
+ Discord
+ Shazam
+ Runkeeper
+ Nike+ Run Club
+ Tinder
+ Bumble
+ WhoSampled

## 10.4	Interfaces de Comunicações
<p align="justify">As comunicações entre os serviços são feitas por meio de conexão  remota via internet (wifi, internet móvel e etc)

# 11. Requisitos de Licenciamento
<p align="justify">Todo o conteúdo e o próprio Serviço Spotify são de propriedade da empresa Spotify. Ao usuário é concedido apenas uma licença limitada e não comercial para que este faça uso pessoal do conteúdo e do serviço.

# 12. Observações Legais, de Direitos Autorais e outros
<p align="justify">Todas as marcas comerciais, marcas de serviço, nomes comerciais, logotipos, nomes de domínio são de propriedade exclusiva da empresa Spotify. Não é concedido qualquer direito ao usuário de utilizar os recursos da marca Spotify, comercialmente ou não.
