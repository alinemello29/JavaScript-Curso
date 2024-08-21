ITERADORES
O método .map()
12 minutos
O segundo iterador que vamos cobrir é .map(). Quando .map()é chamado em um array, ele pega um argumento de uma função de retorno de chamada e retorna um novo array! Dê uma olhada em um exemplo de chamada de .map():

const numbers = [1, 2, 3, 4, 5]; 

const bigNumbers = numbers.map(number => {
  return number * 10;
});

.map()funciona de maneira semelhante a .forEach()— a principal diferença é que .map()retorna uma nova matriz.

No exemplo acima:

numbersé uma matriz de números.
bigNumbersarmazenará o valor de retorno da chamada .map()em numbers.
numbers.mapiterará por cada elemento na numbersmatriz e passará o elemento para a função de retorno de chamada.
return number * 10é o código que desejamos executar em cada elemento do array. Isso salvará cada valor do numbersarray, multiplicado por 10, em um novo array.
Se dermos uma olhada numbersem bigNumbers:

console.log(numbers); // Output: [1, 2, 3, 4, 5]
console.log(bigNumbers); // Output: [10, 20, 30, 40, 50]

Observe que os elementos numbersnão foram alterados e bigNumbersé uma nova matriz.

Instruções
Checkpoint 1 Passed
1 .
Adicione seu código abaixo do animalsarray e antes da linhaconsole.log(secretMessage.join(''));

Use .map()para criar um novo array que contém o primeiro caractere de cada string no animalsarray. Salve o novo array em uma constvariável chamada secretMessage.

Ponto de verificação 2 aprovado
2 .
Use .map()para dividir todos os números em bigNumberspor 100. Salve os valores retornados em uma variável declarada com constchamada smallNumbers.