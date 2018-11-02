# sistemaPHP
Esse conjunto de código foi criado para facilitar quem quer iniciar seus estudos com php. Nele Foram criados um conjunto de funções que torna processos como consulta em banco de dados, assim como sua conexão, mais fácies e práticas

# Iniciando
Para iniciar um projeto com esse framework, pasta copiar a pasta sistema para o seu projeto. Após isso, você deve incluir o arquivo system.php (include 'system.php'). No arquivo system.php você deve preencher os requitos de banco de dados, com host, username, password. Bem como a URLBASE, que a url index do seu projeto. 

# Usando
Para usar uma funçao simples como a DBread, que lê do banco de dados e retorna em forma de array, basta inciar a conexão com

$link = DBconnc();

dar set na variável e fazê-la receber a função, que tem como parâmetros a conexão, a tabela, a query e os campos que devem ser tragos.

$teste = DBread($link, 'tabela_teste', "WHERE id = '1'", 'id, nome, sobrenome');

Após isso, deve-se fechar a conexão com

DBclose($link);
