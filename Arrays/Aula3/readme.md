MATRIZES
Acessando Elementos

Uma maneira de criar um array é usar um literal de array . Um literal de array cria um array envolvendo itens em colchetes

Arrays em JavaScript são indexados a zero , o que significa que as posições começam a contar a partir de 0em vez de 1. Portanto, o primeiro item em um array estará na posição 0. Vamos ver como poderíamos acessar um elemento em um array:

Diagrama descrevendo como acessar a propriedade de um array usando o índice do elemento
No trecho de código acima:

citiesé uma matriz que possui três elementos.
Estamos usando a notação de colchetes, []com o índice após o nome do array para acessar o elemento.
cities[0]acessará o elemento no índice 0do array cities. Você pode pensar nisso cities[0]como acessar o espaço na memória que contém a string 'New York'.
Você também pode acessar caracteres individuais em uma string usando a notação de colchetes e o índice. Por exemplo, você pode escrever:

const hello = 'Hello World';
console.log(hello[6]);
// Output: W

O console será exibido, Wpois é o caractere que está no índice 6.

Instruções
Ponto de verificação 1 aprovado
1 .
Elementos individuais em matrizes também podem ser armazenados em variáveis.

Crie uma variável chamada listIteme defina-a como igual ao primeiro item na famousSayingsmatriz usando a notação de colchetes ( []).

Em seguida, use console.log()para imprimir a listItemvariável no console.

Ponto de verificação 2 aprovado
2 .
Agora, console.log()o terceiro elemento na famousSayingsmatriz usa a notação de colchetes para acessar o elemento.

Não salve o elemento em uma nova variável antes de registrá-lo.

Ponto de verificação 3 aprovado
3 .
Incrível, você pode acessar cada elemento em um array usando o índice. Mas o que acontece se você tentar acessar um índice que está além do último elemento?

Tente registrar o item no índice [3]do famousSayingsconsole. O que está registrado no console?