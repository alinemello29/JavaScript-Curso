MATRIZES
O método .pop()

Outro método de array, .pop(), remove o último item de um array.

const newItemTracker = ['item 0', 'item 1', 'item 2'];

const removed = newItemTracker.pop();

console.log(newItemTracker); 
// Output: [ 'item 0', 'item 1' ]
console.log(removed);
// Output: item 2

No exemplo acima, chamando .pop()o newItemTrackerarray removido item 2do final.
.pop()não aceita nenhum argumento, ele simplesmente remove o último elemento de newItemTracker.
.pop()retorna o valor do último elemento. No exemplo, armazenamos o valor retornado em uma variável removedpara ser usada mais tarde.
.pop()é um método que altera o array inicial.
Quando você precisar modificar um array removendo o último elemento, use .pop().

Instruções
Checkpoint 1 Passed
1 .
Use o .pop()método para remover o último elemento de chores.

Ponto de verificação 2 aprovado
2 .
Uma linha depois de chamar chores.pop(), faça login choresno console para verificar se funcionou.

