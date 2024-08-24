ITERADORES
O método .reduce()
14 minutos
Outro método de iteração amplamente usado é .reduce(). O .reduce()método retorna um único valor após iterar pelos elementos de um array, reduzindo assim o array. Dê uma olhada no exemplo abaixo:

const numbers = [1, 2, 4, 10];

const summedNums = numbers.reduce((accumulator, currentValue) => {
  return accumulator + currentValue
})

console.log(summedNums) // Output: 17

Aqui estão os valores de accumulatore currentValueconforme iteramos pela numbersmatriz:

Iteração	accumulator	currentValue	valor de retorno
Primeiro	1	2	3
Segundo	3	4	7
Terceiro	7	10	17

Agora vamos rever o uso .reduce()do exemplo acima:

numbersé uma matriz que contém números.
summedNumsé uma variável que armazena o valor retornado da invocação .reduce()em numbers.
numbers.reduce()chama o .reduce()método no numbersarray e recebe uma função de retorno de chamada como argumento.
A função de retorno de chamada tem dois parâmetros, accumulatore currentValue. O valor de accumulatorcomeça como o valor do primeiro elemento no array e o currentValuecomeça como o segundo elemento. Para ver o valor de accumulatore currentValuemudar, revise o gráfico acima.
À medida que .reduce()itera pela matriz, o valor de retorno da função de retorno de chamada se torna o accumulatorvalor para a próxima iteração e currentValueassume o valor do elemento atual no processo de loop.
O .reduce()método também pode receber um segundo parâmetro opcional para definir um valor inicial accumulator(lembre-se, o primeiro argumento é a função de retorno de chamada!). Por exemplo:

const numbers = [1, 2, 4, 10];

const summedNums = numbers.reduce((accumulator, currentValue) => {
  return accumulator + currentValue
}, 100)  // <- Second argument for .reduce()

console.log(summedNums); // Output: 117

Aqui está um gráfico atualizado que considera o segundo argumento de 100:

Iteração #	accumulator	currentValue	valor de retorno
Primeiro	100	1	101
Segundo	101	2	103
Terceiro	103	4	107
Quarto	107	10	117

Instruções
Checkpoint 1 Passed
1 .
Vamos praticar a chamada .reduce()e o uso console.log()para verificar os valores conforme .reduce()itera pela matriz.

Em main.js , há uma matriz de números, newNumbers.

Para começar, declare uma nova variável chamada newSumusando a constpalavra-chave . Atribua ao newSumvalor de chamar .reduce()em newNumbers. Você não precisa fornecer nenhum argumento para .reduce()ainda.

Você também verá um TypeError: undefined is not a functionmas corrigiremos isso depois de adicionar nossa função de retorno de chamada na próxima etapa!

Ponto de verificação 2 aprovado
2 .
Forneça .reducecom um argumento de uma função de retorno de chamada. A função de retorno de chamada tem dois parâmetros. O primeiro parâmetro é accumulatore o segundo parâmetro é currentValue. Use uma expressão de função ou uma função de seta.

Ponto de verificação 3 aprovado
3 .
Para verificar o valor que está sendo usado à medida que iteramos pela matriz, adicione três instruções ao corpo da função do retorno de chamada:

console.log('The value of accumulator: ', accumulator);
console.log('The value of currentValue: ', currentValue);
uma declaração de retorno que adiciona accumulatora currentValue.
Ponto de verificação 4 aprovado
4 .
Registre o valor de newSumno console para ver o valor de retorno da chamada .reduce()de newNumbers.

Ponto de verificação 5 aprovado
5 .
Enquanto temos esse código configurado, vamos também verificar o que acontece se você adicionar um segundo argumento a .reduce(). O segundo argumento atua como um valor inicial para o accumulator.

Adicione um segundo argumento de 10to .reduce().