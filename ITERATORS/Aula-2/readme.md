ITERADORES
O método .forEach()
10 minutos
O primeiro método de iteração que vamos aprender é .forEach(). Bem nomeado, .forEach()executará o mesmo código para cada elemento de um array.
Diagrama descrevendo as partes de um iterador de matriz, incluindo o identificador da matriz, a seção que é o iterador e a função de retorno de chamada

O código acima registrará uma lista bem formatada de mantimentos no console. Vamos explorar a sintaxe de invocação de .forEach().

groceries.forEach()chama o forEachmétodo no groceriesarray.
.forEach()recebe um argumento de função de retorno de chamada. Lembre-se, uma função de retorno de chamada é uma função passada como argumento para outra função.
.forEach()faz um loop pelo array e executa a função de retorno de chamada para cada elemento. Durante cada execução, o elemento atual é passado como um argumento para a função de retorno de chamada.
O valor de retorno para .forEach()sempre será undefined.
Outra maneira de passar um retorno de chamada .forEach()é usar a sintaxe da função de seta.

groceries.forEach(groceryItem => console.log(groceryItem));

Também podemos definir uma função de antemão para ser usada como função de retorno de chamada.

function printGrocery(element){
  console.log(element);
}

groceries.forEach(printGrocery);

O exemplo acima usa uma declaração de função, mas você também pode usar uma expressão de função ou uma função de seta.

Todos os três trechos de código fazem a mesma coisa. Em cada método de iteração de array, podemos usar qualquer um dos três exemplos para fornecer uma função de retorno de chamada como um argumento para o iterador. É bom estar ciente das diferentes maneiras de passar funções de retorno de chamada como argumentos em iteradores porque os desenvolvedores têm diferentes preferências estilísticas. No entanto, devido à forte adoção do ES6, usaremos a sintaxe da função de seta nos exercícios posteriores.

Instruções
Checkpoint 1 Passed
1 .
Itere sobre o fruitsarray para logar I want to eat a mais o nome de cada fruta para o console. Por exemplo, I want to eat a mango.

Você pode usar qualquer forma de retorno de chamada que preferir.