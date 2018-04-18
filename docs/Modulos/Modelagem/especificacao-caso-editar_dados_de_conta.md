|Data|Versão|Descrição|Autor|
|----|-----|----|------|
|18/04/2018|1.0|Especificação da UC08|Geovanne Santos|

<h1>RF14 - Editar dados de conta</h1>
<object width="700" height="600" data="../caso_de_uso_editar_dados.png"></object>


<h4>Descrição:</h4><br />
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
