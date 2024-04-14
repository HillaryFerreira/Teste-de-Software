# Teste-de-Software
#Teste-caixa-branca
<H2>A DOCUMENTAÇÃO FOI DESCRITA NO CÓDIGO?</H2>

<p>Únicos comentarios feito são para indicar onde faz a instrucao da SQL  e onde finaliza a Classe. Como por exemplo: //INSTRUCAO SQL, //FIM DA CLASSE. </p>

<H2>AS VARIÁVEIS E CONSTANTES POSSUEM BOA NOMENCLATURA?</H2>
<P>As variáveis e constantes não possuem uma nomenclatura muito descritiva. Por exemplo, 'conn', 'sql', 'result', 'nome', poderiam ter nomes mais claros para indicar sua função no código.</P>

<h2>EXISTEM LEGIBILIDADE E ORGANIZAÇÃO NO CÓDIGO?</h2>
<p>O código poderia estar melhor identado, com espaçamento melhor para visualização mais clara e com mais comentarios do que esta sendo feito em cada trecho do código.</p>

<h2>TODOS OS NULLPOINTERS FORAM TRATADOS?</h2>
<p>não houve tratamento adequado para possíveis NullPointerExceptions. O código não verifica se os objetos retornados, como Connection, Statement e ResultSet, são nulos antes de tentar acessá-los ou utilizá-los. Isso pode levar a exceções não tratadas se esses objetos não forem inicializados corretamente ou se ocorrerem erros durante sua criação ou execução.<br>
Por exemplo, se a tentativa de obter uma conexão com o banco de dados falhar, o objeto conn permanecerá como null. Se tentarmos usar esse objeto posteriormente sem verificar se é nulo, isso resultará em uma NullPointerException.</p>
