ITERADORES
O método .findIndex()
11 minutos
Às vezes queremos encontrar a localização de um elemento em um array. É aí que o .findIndex()método entra! Chamar .findIndex()um array retornará o índice do primeiro elemento que avalia truena função de retorno de chamada.

const jumbledNums = [123, 25, 78, 5, 9]; 

const lessThanTen = jumbledNums.findIndex(num => {
  return num < 10;
});

jumbledNumsé uma matriz que contém elementos que são números.
const lessThanTen = declara uma nova variável que armazena o número de índice retornado da invocação .findIndex().
A função de retorno de chamada é uma função de seta que tem um único parâmetro, num. Cada elemento no jumbledNumsarray será passado para essa função como um argumento.
num < 10;é a condição em relação à qual os elementos são verificados. .findIndex()retornará o índice do primeiro elemento que for avaliado para trueessa condição.
Vamos dar uma olhada no que lessThanTené avaliado como:

console.log(lessThanTen); // Output: 3 

Se verificarmos qual elemento tem índice 3:

console.log(jumbledNums[3]); // Output: 5

Ótimo, o elemento em index 3é o número 5. Isso faz sentido, já que 5é o primeiro elemento que é menor que 10.

Se não houver um único elemento na matriz que satisfaça a condição no retorno de chamada, então .findIndex()retornará -1.

const greaterThan1000 = jumbledNums.findIndex(num => {
  return num > 1000;
});

console.log(greaterThan1000); // Output: -1

Instruções
Checkpoint 1 Passed
1 .
Invoque .findIndex()a animalsmatriz para encontrar o índice do elemento que tem o valor 'elephant'e salve o valor retornado em uma constvariável chamada foundAnimal.

Ponto de verificação 2 aprovado
2 .
Vamos ver se conseguimos encontrar o índice do primeiro animal que começa com a letra 's'.

Chame .findIndex()o animalsarray e retorne o índice do primeiro elemento que começa com 's'. Atribua o valor retornado a uma constvariável chamada startsWithS.