Parâmetros padrão

Um dos recursos adicionados no ES6 é a capacidade de usar parâmetros padrão . Os parâmetros padrão permitem que os parâmetros tenham um valor predeterminado caso não haja nenhum argumento passado para a função ou se o argumento for undefinedchamado.

Dê uma olhada no trecho de código abaixo que usa um parâmetro padrão:

function greeting (name = 'stranger') {
  console.log(`Hello, ${name}!`)
}

greeting('Nick') // Output: Hello, Nick!
greeting() // Output: Hello, stranger!

No exemplo acima, usamos o =operador para atribuir ao parâmetro nameum valor padrão de 'stranger'. Isso é útil caso queiramos incluir uma saudação padrão não personalizada!

Quando o código chama, greeting('Nick')o valor do argumento é passado e, 'Nick', substituirá o parâmetro padrão para 'stranger'registrar 'Hello, Nick!'no console.

Quando não há um argumento passado para greeting(), o valor padrão de 'stranger'é usado e 'Hello, stranger!'registrado no console.

Ao usar um parâmetro padrão, consideramos situações em que um argumento não é passado para uma função que espera um argumento.

Vamos praticar a criação de funções que usam parâmetros padrão.

Instruções
Checkpoint 1 Passed
1 .
A função makeShoppingList()cria uma lista de compras com base nos itens que são passados ​​para a função como argumentos.

Imagine que você sempre compra leite, pão e ovos toda vez que vai fazer compras. Para facilitar a criação de uma lista de compras, vamos atribuir valores padrão aos parâmetros no arquivo makeShoppingList().

Altere os parâmetros makeShoppingList()para parâmetros padrão:

Atribua 'leite' como o valor padrão de item1.
Atribua 'pão' como o valor padrão de item2.
Atribua 'ovos' como o valor padrão de item3.
