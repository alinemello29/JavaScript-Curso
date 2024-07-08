MATRIZES
O método .push()

Vamos aprender sobre alguns métodos JavaScript integrados que facilitam o trabalho com arrays. Esses métodos são chamados especificamente em arrays para tornar tarefas comuns, como adicionar e remover elementos, mais diretas.

Um método, .push(), nos permite adicionar itens ao final de um array. Aqui está um exemplo de como isso é usado:

const itemTracker = ['item 0', 'item 1', 'item 2'];

itemTracker.push('item 3', 'item 4');

console.log(itemTracker); 
// Output: ['item 0', 'item 1', 'item 2', 'item 3', 'item 4'];

Então, como funciona .push()?

Acessamos o pushmétodo usando a notação de ponto, conectando pushcom itemTrackerum ponto.
Então chamamos isso como uma função. Isso porque .push()é uma função e uma que o JavaScript nos permite usar diretamente em um array.
.push()pode receber um único argumento ou múltiplos argumentos separados por vírgulas. Neste caso, estamos adicionando dois elementos: 'item 3'e 'item 4'para itemTracker.
Observe que as .push()alterações, ou mutates , itemTracker. Você também pode ver .push()isso como um método de array destrutivo , pois ele altera o array inicial.
Se você está procurando um método que irá transformar um array adicionando elementos a ele, então este .push()é o método para você!

Instruções
Ponto de verificação 1 aprovado
1 .
Adicione dois elementos à choresmatriz usando .push().

Ponto de verificação 2 aprovado
2 .
Use console.logpara imprimir sua choresmatriz para garantir que seus itens foram adicionados.