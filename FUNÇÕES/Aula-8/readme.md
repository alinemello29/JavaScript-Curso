FUNÇÕES
Expressões de Função

Outra maneira de definir uma função é usar uma expressão de função . Para definir uma função dentro de uma expressão, podemos usar a functionpalavra-chave. Em uma expressão de função, o nome da função geralmente é omitido. Uma função sem nome é chamada de função anônima . Uma expressão de função geralmente é armazenada em uma variável para fazer referência a ela.

Considere a seguinte expressão de função:

definindo uma expressão de função
Para declarar uma expressão de função:

Declare uma variável para fazer com que o nome da variável seja o nome, ou identificador, da sua função. Desde o lançamento do ES6, é prática comum usar constcomo palavra-chave para declarar a variável.

Atribua como valor dessa variável uma função anônima criada usando a functionpalavra-chave seguida por um conjunto de parênteses com parâmetros possíveis. Em seguida, um conjunto de chaves que contém o corpo da função.

Para invocar uma expressão de função, escreva o nome da variável na qual a função está armazenada, seguido de parênteses envolvendo todos os argumentos que estão sendo passados ​​para a função.

variableName(argument1, argument2)

Ao contrário das declarações de função, as expressões de função não são elevadas, portanto não podem ser chamadas antes de serem definidas.

Vamos definir uma nova função usando uma expressão de função.

Instruções
Checkpoint 1 Passed
1 .
Digamos que temos uma planta que precisamos regar uma vez por semana às quartas-feiras. Poderíamos definir uma expressão de função para nos ajudar a verificar o dia da semana e se a planta precisa ser regada:

Crie uma variável nomeada plantNeedsWaterusando a constpalavra-chave variável.
Atribua uma função anônima que receba um parâmetro dayto plantNeedsWater.
Ponto de verificação 2 aprovado
2 .
Agora precisamos adicionar algum código ao corpo da função plantNeedsWater():

No corpo da função, adicione uma ifcondicional que verifique day === 'Wednesday'.
Se a condicional for verdadeira, dentro do ifbloco de código, use a returnpalavra-chave para retornar true.
Ponto de verificação 3 aprovado
3 .
Nos dias que não são 'Wednesday', plantNeedsWater()deve retornar false:

Adicione uma elsedeclaração após a ifdeclaração.
Dentro da elseinstrução use a returnpalavra-chave para retornar false.
Ponto de verificação 4 aprovado
4 .
Chame o plantNeedsWater()e passe 'Tuesday'como argumento.

Ponto de verificação 5 aprovado
5 .
Vamos verificar se plantNeedsWater()retornou o valor esperado.

Faça logon plantNeedsWater('Tuesday')no console. Se funcionou corretamente, você deverá ver falselogado no console.