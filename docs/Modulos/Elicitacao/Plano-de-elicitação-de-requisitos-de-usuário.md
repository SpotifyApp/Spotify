<h1>Elicitação de requisitos de usuário</h1>
<h3>Histórico de revisão</h3>

Data | Responsável | Versão| Mudança realizada|
--------- | ------| --------| ------------ |
29/03/2018     | Geovanne Saraiva |   1.0   |  Primeira versão do plano de elicitação   |
02/04/2018     | Geovanne Saraiva |   1.1   |  Segunda versão do plano de elicitação   |
03/04/2018     | Geovanne Saraiva |   1.2   |  Terceira versão do plano de elicitação   |
20/04/2018     | Geovanne Saraiva |   1.3   |  Terceira versão do plano de elicitação   |
25/05/2018     | Eduardo e Geovanne |   2.0  |  Quarta versão do plano de elicitação(Atualizando requisitos e moscow)   |
05/06/2018     | Eduardo Júnio|   2.1  |  Adicionando novos requisitos identificados na especificação suplementar |



<h3> Introdução </h3>
Este documento foi desenvolvido para a disciplina de Requisitos em Software, da Universidade de Brasília, no qual o grupo procura elicitar o aplicativo Spotify, que é obter o máximo de informações necessárias para o conhecimento de um objeto. No contexto da engenharia de software, a elicitação de requisitos provê o mais correto e completo entendimento do que é demandado de um determinado software. A análise foi dividida em tópicos, os mesmos são: usuário, marketing,  monetização, música, integração e design.

<h3> Objetivo </h3>
O documento presente visa definir as técnicas que serão aplicadas como forma de levantar requisitos de Usuário do Spotify, focando nos processos de elicitação: observação participativa e HistoryTelling.

<h3> Universo de informação </h3>
As informações necessárias para coleta de requisitos e para a construção de todo o trabalho foram mapeadas pelas seguintes fontes:<br />
<ul>
  <li>Usuários do Spotify: Geovanne Santos e Renato Valerio</li>
  <li>Observação participativa</li>
  <li>E-mail</li>
  <li>Redes Sociais: Facebook e Instagram</li>
  <li>Sites e Revistas</li>
</ul>

<h1>Plano de elicitação</h1>
Não há uma técnica padrão de elicitação de requisitos, por isso é necessário conhecer diversas técnicas e avaliar qual/quais serão mais adequadas ao projeto, facilitando o processo de elicitação. No desenvolvimento deste projeto serão utilizadas as técnicas a seguir:

<h3>Observação Participativa</h3>
A observação participante é uma técnica de investigação social em que o observador partilha, na medida em que as circunstâncias o permitam, as atividades, as ocasiões, os interesses e os afetos de um grupo de pessoas ou de uma comunidade (Anguera, Metodologia de la observación en las Ciencias Humanas, 1985).<br />
Por orientação dos professores que estão acompanhando a elicitação dos requisitos, foi feito um video no qual gravamos a utilização do aplicativo, por um usuário(Geovanne Saraiva) e depois analisamos o video e levantamos os requisitos do mesmo, que foram:<br />

* Perfil de artista
  * Postar músicas
  * Receber royalties pagos pelo aplicativo spotify
  * Ver o relatório de informações sobre suas músicas e seus respectivos álbuns, um feedback que mostra a frequência com que os álbuns são acessados.
  * Verificar a autenticidade do perfil de artista.

* Perfil de usuário comum
  * Cadastro como perfil de usuário comum
  * Adquirir o plano premium como: plano família, plano estudantil e plano tradicional.
  * Seguir amigos para conhecer o que eles ouvem.
  * Escolher as notificações que deseja receber.
  * Ficar em modo offline, onde só tocará músicas baixadas.
  * Sair da conta.
  * Fazer login
  * Apagar cache e dados salvos.
  * Editar dados de conta.
  * Mudar senha.
  * Editar foto de perfil.
  * Ajustar o volume de acordo com o seu ambiente.
  * Mudar o perfil padrão para perfil de artista.
  * Mudar reprodução ativa
  * Sair do aplicativo

<h3>Introspecção</h3>
Consiste em entender quais propriedades o sistema deve possuir para ser um sucesso, deve-se imaginar o que o usuário gostaria, se lhe tivesse dado uma respectiva tarefa, neste caso será analisado o usuário padrão e artista do aplicativo spotify. <br />
<h4>Relato de introspecção: comportamento de usuário artista logado</h4>
<h5>Relator: Geovanne Santos</h5>
1. Atualizar sua biografia. <br />
2. Postar suas playlists. <br />
3. Controlar como os fãns te veem no spotify. <br />
4. Ver uma série de gráficos, com dados de como suas músicas estão sendo ouvidas pelos usuários, como estão descobrindo e ouvindo suas músicas, estas informações podem te ajudar a promover campanhas, fazer novas músicas e planejar novas rotas pra uma futura turnê. <br />
5. Atualizar sua foto de perfil, ou do seu álbum.<br />
6. Controlar a música na parte superior do perfil do artista. É uma ótima maneira de informar aos fãs sobre uma faixa em que você participa, anunciar sua próxima turnê, exibir uma nova playlist. Escolha qualquer faixa, álbum ou lista de reprodução e adicione uma imagem legal dos bastidores e uma breve mensagem sobre por que você adora isso. <br />
7. Permitir o artista colocar os locais onde serão feitos os shows, no próprio profile.
8. Distribuidor cria o perfil de artista do seu cliente(artista)

<h2>🎧 Moscow (priorização de requisitos)</h2>
Os requisitos listados abaixo foram obtidos a partir das técnicas de elicitação apresentadas anteriormente. Os videos de observação que serviram para elicitar os requisitos de usuário foram gravados por Eduardo e Amanda e podem ser vistos  [aqui](https://drive.google.com/drive/folders/1AO_csKjmjIGtgCR_OSzN0olOFou4VTwR)

<h5>Explicação de como foi avaliado os requisitos em: must, should, could, would.</h5>
<p>
- Must: O que acontece se esse requisito não for atendido? ”Se a resposta for cancelar o projeto então deve se usar o must, não é possível entregar na data prevista sem isso, Inseguro sem isso.
</p>
<p>
- Should: Importante, mas não vital, pode ser doloroso deixar de fora, mas a solução ainda é viável.
</p>
<p>
- Could: Os requisitos rotulados como Could são desejáveis, mas não necessários, e podem melhorar a experiência do usuário ou a satisfação do cliente por um pequeno custo de desenvolvimento. Estes serão tipicamente incluídos se o tempo e os recursos permitirem..
</p>
<p>
- Would: Requisitos rotulados como Would terão que ser acordados pelas partes interessadas como os itens menos críticos e de menor retorno, ou não são apropriados naquele momento. Como resultado, os requisitos não serão planejados no cronograma do próximo timebox de entrega. Os requisitos não serão eliminados ou reconsiderados para inclusão em um timebox posterior..
</p>

Requisitos|Must(deve ter)|Should(deveria ter)  |Could(poderia ter)  |Would(seria legal ter)|
---------------- |---------------- | ---------------| ------------------| ---------------------- |
Adquirir o plano premium | | x | | |
Apagar cache e dados salvos | | | x | |
Atualizar sua biografia | | x | | |
Atualizar a foto do seu álbum | | x | | |
Ativar o status de transmissão(permitir outros apps verificarem o que está ouvindo) | | x | | |
Distribuidor cria o perfil de artista do seu cliente(artista) | x | | | |
Cadastro como perfil de usuário comum | x | | | |
Controlar a música que aparecerá na parte superior do perfil do artista | | x | | |
Configurar o volume | x | | | |
Colocar a agenda de shows | | | x | |
Escolher as notificações que deseja receber | | | x | |
Editar foto de perfil conta | x | | | |
Fazer login | x | | | |
Ficar em modo offline | | x | | |
Postar músicas| x | | | |
Mudar o perfil de usuário comum para perfil de artista | | x | | |
Mudar senha | x | | | |
Seguir amigos para conhecer o que eles ouvem | | | x | |
Sair da conta | x | | | |
Ver os relatórios de informações sobre seus álbuns | | x | | |
Verificar a autenticidade do perfil de artista | x | | | |
Mudar reprodução ativa | x | | | |
Sair do aplicativo | x | | | |

21 requisitos de usuário foram elicitados neste módulo.

<h2> Bibliografia </h2>
- Anguera, Metodologia de la observación en las Ciencias Humanas, 1985. <br />
- https://artists.spotify.com/guide/spotify-for-artists<br />
- McIntyre, John (October 20, 2016). "Moscow or Kano - how do you prioritize?
