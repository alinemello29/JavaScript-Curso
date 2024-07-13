MATRIZES
Matrizes aninhadas

Mencionamos anteriormente que os arrays podem armazenar outros arrays. Quando um array contém outro array, ele é conhecido como array aninhado . Examine o exemplo abaixo:

const nestedArr = [[1], [2, 3]];

Para acessar os arrays aninhados, podemos usar a notação de colchetes com o valor do índice, assim como fizemos para acessar qualquer outro elemento:

const nestedArr = [[1], [2, 3]];

console.log(nestedArr[1]); // Output: [2, 3]

Observe que nestedArr[1]irá capturar o elemento no índice 1 que é o array [2, 3]. Então, se quisermos acessar os elementos dentro do array aninhado, podemos encadear ou adicionar mais notação de colchetes com valores de índice.

const nestedArr = [[1], [2, 3]];

console.log(nestedArr[1]); // Output: [2, 3]
console.log(nestedArr[1][0]); // Output: 2

Na segunda console.log()instrução, temos duas notações de colchetes encadeadas nestedArr. Sabemos que esse nestedArr[1]é o array [2, 3]. Então, para pegar o primeiro elemento desse array, usamos nestedArr[1][0]e obtemos o valor de 2.

Instruções
Checkpoint 1 Passed
1 .
Vamos fazer um array aninhado! Crie uma variável numberClusters. Atribua como seu valor um array com três elementos de array.

O primeiro elemento da matriz deve conter os elementos 1e 2nessa ordem.
O segundo elemento da matriz deve conter os elementos 3e 4nessa ordem.
O terceiro elemento da matriz deve conter os elementos 5e 6nessa ordem.
Ponto de verificação 2 aprovado
2 .
Incrível, você fez um array aninhado! Agora declare uma variável nomeada targetusando a constpalavra-chave e assign para acessar o elemento 6dentro de numberClusters.

