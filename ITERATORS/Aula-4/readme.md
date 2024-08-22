ITERADORES
O método .filter()
10 minutos
O segundo iterador que vamos cobrir é .filter(). Quando .map()é chamado em um array, ele pega um argumento de uma função de retorno de chamada e retorna um novo array! Dê uma olhada em um exemplo de chamada de .filter():.filter()retorna um array de elementos após filtrar certos elementos do array original. A função de retorno de chamada para o .filter()método deve retornar trueou falsedependendo do elemento que é passado a ele. Os elementos que fazem a função de retorno de chamada retornar truesão adicionados ao novo array. Dê uma olhada no exemplo a seguir:

const words = ['chair', 'music', 'pillow', 'brick', 'pen', 'door']; 

const shortWords = words.filter(word => {
  return word.length < 6;
});

wordsé uma matriz que contém elementos de string.
const shortWords = declara uma nova variável que armazenará o array retornado da invocação .filter().
A função de retorno de chamada é uma função de seta que tem um único parâmetro, word. Cada elemento no wordsarray será passado para essa função como um argumento.
word.length < 6;é a condição na função de retorno de chamada. Qualquer um worddo wordsarray que tenha menos de 6caracteres será adicionado ao shortWordsarray.
Vamos também verificar os valores de wordse shortWords:

console.log(words); // Output: ['chair', 'music', 'pillow', 'brick', 'pen', 'door']; 
console.log(shortWords); // Output: ['chair', 'music', 'brick', 'pen', 'door']

Se dermos uma olhada wordsem shortWords:

Instruções
Checkpoint 1 Passed
1 .
Chame o .filter()método on randomNumberspara retornar valores menores que 250. Salve-os em um novo array chamado smallNumbers, declarado com const.

Ponto de verificação 2 aprovado
2 .
Agora vamos trabalhar com um array de strings. Invoque .filter()no favoriteWordsarray para retornar elementos que tenham mais de 7 caracteres. Salve o array retornado em uma constvariável chamada longFavoriteWords.

