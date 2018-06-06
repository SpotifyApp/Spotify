<h1><center>Elicitação - Módulo: Integração do uso do Spotify em diferentes Hardwares</h1>
<h3>Histórico de revisão</h3>

Data | Responsável | Versão| Mudança realizada|
:--------- | :------:| :--------:| :------------ |
01/04/2018    | Lucas Filipe |   1.0   |  Construção do corpo do documento.   |
01/04/2018    | Lucas Filipe |   1.1   | Preenchimento de Conceitos e metodologia realizada para elicitação.  |
05/06/2018 | Eduardo Júnio| 1.2 | Adicionado requisitos identificados na especificação suplementar|

<h2> 1.Introdução </h2>
<p> A palavra Elicitar significa : <i>descobrir, tornar explicito, obter o máximo de informações para o conhecimento do objetivo em questão</i>. De acordo com Júlio Leite em Livro Vivo:Engenharia de Requisitos[1]: "Dentro da engenharia de requisitos cabe a Elicitação a tarefa de identificar os fatos que compõe os requisitos do sistema, de forma a prover o mais correto e mais completo entendimento do que é demandado daquele software." As tarefas que compõe a Elicitação são: Identificação das fontes de informação dentro do Universo de Informações(UdI), emprego de técnicas de coletas de fatos e plano de comunicação.  </p>

----
<h2> 2.Universo de informação(UdI) </h2>
<p> De Acordo com Leite,José[2] o universo de informação é onde contém todas as fontes de informação que vamos utilizar na elicitação.</p>
<p>As fontes de informações utilizadas para a realização dessa elicitação foram:</br>

* **Spotify**
  >* Aplicativo para celular Android.
  >* Aplicativo para PlayStation4.
  >* Aplicativo para Ipad.
  >* Aplicativo para SmartTv.
  >* WebPlayer para Chrome.
  >* Documentos Spotify Labs.
  >* Spotify for Developers.

* **Usuários do Spotify na equipe**
  >* Lucas Filipe


</p>

----
<h2>3.Técnicas de Coleta de Dados</h2>
<p>De acordo com José Leite[3], cabe ao engenheiro de requisitos selecionar as técnicas a serem utilizadas bem como o esquema de integração entre elas de acordo com o Universo de Informações(Contexto). No desenvolvimento da elicitação de requisitos de integração do Spotify foram utliizadas as seguintes técnicas:  </p>

<h3>3.1 Observação</h3>
<p>Técnica no qual o engenheiro de requisitos estabelece uma posição passiva dentro do universo de informações observando ambiente onde vai acontecer/acontece o uso do software, permitindo uma percepção aprimorada dos objetos, processos e linguagem do ambiente e no caso de reengenharia: uso do software. Para elicitação de requisitos de integração foi realizada duas observações que foram registradas em vídeo(links abaixo), no primeiro vídeo acontece a observação da tentativa/realização da integração de uso do Spotify nos dispositivos Ipad e PC, no segundo a tentativa/realização da integração do uso do Spotify nos dispositivos Playstation 4 e Celular Android.
</p>
</br>

* [Observação 1 - Integração Ipad e WebBrowser.](https://www.youtube.com/watch?v=xC-69a_j0A8)
* [Observação 2 - Integração PlayStation4 e Celular.]

<h3>3.2 Análise de Protocolo</h3>
<p> Técnica que analisa o trabalho/uso de determinada pessoa, através da verbalização no ato da execução da tarefa, ou através da verbalização detalhada de um trabalho que já foi feito, o objetivo dessa técnica de coleta de dados é procurar estabelecer o raciocínio do usuário enquanto executa uma determinada tarefa facilitando a obteção de fatos não facilmente observáveis visto que todos os atos são verbalizados. Para melhor aproveitamento das fontes de informações foi decidido fazer uma análise de protocolo do perfeito uso do Spotify alternando entre os dois dispositivos distintos( celular e computador), para melhor extração de informações a análise de protocolo foi registrada em vídeo(link abaixo).
</p>
</br>

* [Análise de Protocolo 1 - Integração do Celular Android e WebBrowser.](https://www.youtube.com/watch?v=6IyXEV9J0TQ)


----
<h2>4. Elicitação dos Requisitos.</h2>

Tabela com os requisitos e suas respectivas origens, em caso de dúvida consulte o item 2 deste documento.

Requisito | Observação 1 | Observação 2 | Análise de Protocolo 1|
:--------- | :------:| :--------:| :------------: |
R01 - Listar dispositivos disponíveis.    | X |  | X |  
R02 - Alertar sobre reprodução de música ativa em outros dispositivos logados com o mesma conta.    | X |   |  |
R03 - Visualizar informações de reprodução em outros dispositivos logados  com a mesma conta.    | X |  | X |
R04 - Controlar reprodução em outros dispositivos logados com o mesmo usuário.    | X | X | X |
R05 - Selecionar músicas/playlists para reprodução em dispositivo ativo através de outro dispositivo logado na mesma conta. | X | X | X |
R06 - Controlar volume de dispositivo com reprodução ativa através do aplicativo logado na mesma conta em outro dispositivo. | X | X | X |
R07 - Controlar volume de dispositivo com reprodução ativa através de controles de volume do hardware de outro dispositivo logado com a mesma conta. | X |  | X |
R08 - Trazer reprodução ativa de um dispositivo para outro logado na mesma conta. | X |  | X |
R09 - Listar dispositivos ativos para reprodução conectados pela mesma rede wi-fi. | | X |  |
R10 - Possibilitar login através de outro dispositivo já logado que esteja na mesma rede wi-fi. | | X |  |
R11 - Conectar conta do SPotify com conta da PSN. | | X | |
R12 - Reproduzir música enquanto jogo estiver sendo executado | | X | |
R13 - Listar preferencialmente músicas e playlists mais compatíveis com o dispositivo logado. | | X | |
RF14 - Efetuar Login por dispositivo secundário | X |  | |
RF15 - Importar músicas do seu celular para o aplicativo| X | | |
RF16 - Integração com redes sociais| X | | |
RF17 - Suporte técnico| X | | |
----
<h2>5. Priorização dos Requisitos. </h2>

[Planilha detalhada de priorização com suas devidas justificativas.](https://drive.google.com/open?id=1d0P6WYdMjdwabzobO2R6jwYwohe8vP4p1V9a5Pcw4wQ)

Must(deve ter)|Should(deveria ter)  |Could(poderia ter)  |Would(seria legal ter)|
:----------------: | :---------------:| :------------------:| :----------------------: |
R01    |R03   |R06 |R11
R02 |R04 |R07 | R10
R08| R05| |R13|
R09| R12|     |
|||RF14
RF15|||
RF16|||
RF17|||
-----
<h2> 6. Referências</h2>

* [1][Open Access] Leite, Julio Cesar Sampaio do Prado. Livro Vivo- Engenharia de Requisitos. [Disponível Aqui.](http://livrodeengenhariaderequisitos.blogspot.com.br/) Acesso em: 01 de Abril de 2018.
* [2][Open Access] Leite, Julio Cesar Sampaio do Prado. Livro Vivo : Engenharia de Requisitos - Universo de Informações. [Disponível Aqui.](http://livrodeengenhariaderequisitos.blogspot.com.br/2007/08/universo-de-informaes.html) Acesso em: 01 de Abril de 2018.
* [3][Open Access]Leite, Julio Cesar Sampaio do Prado. Livro Vivo- Engenharia de Requisitos - Notas de Aula. [Disponível Aqui.](http://livrodeengenhariaderequisitos.blogspot.com.br/) Acesso em: 01 de Abril de 2018.
