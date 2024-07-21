Percorrendo matrizes

for loops são muito úteis para iterar sobre estruturas de dados. Por exemplo, podemos usar um forloop para executar a mesma operação em cada elemento de um array. Arrays contêm listas de dados, como nomes de clientes ou informações sobre produtos. Imagine que temos uma loja e queremos aumentar o preço de todos os produtos do nosso catálogo. Isso pode ser muito código repetido, mas usando um forloop para iterar pelo array, podemos realizar essa tarefa facilmente.

Para percorrer cada elemento de uma matriz, um forloop deve usar a propriedade da matriz .lengthem sua condição.

Confira o exemplo abaixo para ver como foros loops iteram em matrizes:

const animals = ['Grizzly Bear', 'Sloth', 'Sea Lion'];
for (let i = 0; i < animals.length; i++){
  console.log(animals[i]);
}

Este exemplo lhe dará a seguinte saída:

Grizzly Bear
Sloth
Sea Lion

No loop acima, nomeamos nossa variável iteradora i. Esta é uma convenção de nomenclatura de variáveis ​​que você verá em muitos loops. Quando usamos iiterar por arrays, podemos pensar nisso como uma abreviação para a palavra i ndex. Observe como nossa condição de parada verifica se ié menor que animals.length. Lembre-se de que arrays são indexados por zero, o índice do último elemento de um array é equivalente ao comprimento desse array menos 1. Se tentássemos acessar um elemento no índice de, animals.lengthteríamos ido longe demais!

Com forloops, é mais fácil trabalhar com elementos em matrizes.

Instruções
Checkpoint 1 Passed
1 .
Escreva um forloop que itere em nossa vacationSpotsmatriz usando icomo variável iteradora.

Dentro do bloco do forloop, use console.log()para registrar cada elemento no vacationSpotsarray após a string 'I would love to visit '. Por exemplo, a primeira rodada do loop deve imprimir 'I would love to visit Bali'no console.

Ao escrever/alterar loops, há uma chance de que nossa condição de parada não seja atendida e tenhamos um temido loop infinito que essencialmente impede nossa programação de executar qualquer outra coisa! Para sair de um loop infinito em um exercício, atualize a página - então corrija o código para seu loop.