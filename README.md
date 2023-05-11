<h2>PROBLEM STATEMENT: "Ferb, já sei o que vamos fazer hoje!"</h2>
---
<p>Depois de um início de período atípico, os Cinners estão entrando de férias e irão aproveitar a oportunidade para desopilar! Enquanto esperava por esse momento, você utilizou seu tempo livre para assistir um episódio de Phineas e Ferb e os irmãos acabaram te inspirando a aproveitar o recesso pra realizar várias invenções!</p>
<p>Para colocar a ideia em prática, você decidiu que deveria começar organizando as etapas e os gastos para garantir que seu projeto conseguisse ser executado.</p>
<h3>Input</h3>
---
<p>Inicialmente, você receberá o nome da invenção:</p>
- nome_invencao 
<br/><br/>
<p>Em seguida, serão fornecidas n vezes as informações acerca de cada etapa:</p>
- nome_etapa
<br/>
- custo_etapa
<br/>
- tentativas_etapa
<br/><br/>
<p>OBS.1: Há casos em que nem todas as entradas sobre a etapa serão necessárias; nessas situações, elas não serão fornecidas. As etapas "concluir" e "desistir" não possuem custo nem tentativas, a entrada "dar um plus" possui custo mas não tentativas, todas outras etapas possuem custo E tentantivas</p>
<p>OBS.2: Para uma mesma etapa, todas as tentativas têm o mesmo custo.</p>
<p>Para cada tentativa, você receberá uma entrada que indicará o status dessa etapa, o qual será "correto" ou "incorreto":</p>
- status_etapa
<br/><br/>
<p>OBS.3: No máximo um dos status será "correto". Após recebê-lo, você não deverá continuar realizando as tentativas restantes.</p>
<h3>Output</h3>
---
<p>Enquanto você recebe as entradas das etapas, você deve imprimir:
<br/>
Caso a etapa seja "desistir" ou "concluir":</p>
-> A jornada da construção do(a) {invencao} acaba aqui.
<br/><br/>
<p>Nesse caso, não serão fornecidas as entrada de custo nem de tentativas e deve-se interromper a chamada de novas etapas.
<br/>
Caso a entrada seja "dar um plus":</p>
-> Agora o(a) {invencao} ficou ainda mais legal! Pena que precisei gastar R${custo}
<br/><br/>
<p>Nesse caso, será fornecida apenas a entrada de custo, a entrada de tentativas não será fornecida.</p>
<p>Ambos os casos citados acima não serão contabilizados no andamento do projeto como etapas realizadas.</p>
<p>Para os outros casos, você imprimirá:
<br/>
Se o status for "incorreto" :</p>
-> Ainda não consegui {etapa} corretamente, e essa tentativa me custou R${custo}
<p>Se o status for "correto":</p>
-> Oba! consegui {etapa}, o que me custou R${custo}
<br/><br/>
<p>Em que, {custo} é um valor inteiro referente à realização daquela única etapa.
<br/>
Após realizar todas as tentativas necessárias de cada etapa, você deve imprimir:</p>
-> ANDAMENTO DO PROJETO: Etapas realizadas - {etapas_REALIZADAS} ; Tentativas falhas - {total_falhas}
<br/><br/>
<p>Por fim, você deve imprimir:
<br/>
Se você desistiu:</p>
-> Infelizmente, o sonho do(a) {invencao} foi interrompido e levou junto com ele R${despesa_total}
<br/><br/>
<p>Se você concluiu:</p>
-> Uhuuu, finalmente o(a) {invencao} tá pronto(a)! Esse projeto me custou R${despesa_total}