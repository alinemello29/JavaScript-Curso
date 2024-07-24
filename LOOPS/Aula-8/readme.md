Instruções Do...While

Em alguns casos, você quer que um pedaço de código seja executado pelo menos uma vez e então faça um loop com base em uma condição específica após sua execução inicial. É aqui que a do...while declaração entra.

Uma do...whiledeclaração diz para fazer uma tarefa uma vez e então continuar fazendo até que uma condição especificada não seja mais atendida. A sintaxe para uma do...whiledeclaração se parece com isso:

let countString = '';
let i = 0;

do {
  countString = countString + i;
  i++;
} while (i < 5);

console.log(countString);

Neste exemplo, o bloco de código faz alterações na countStringvariável anexando a forma de string da ivariável a ela. Primeiro, o bloco de código após a dopalavra-chave é executado uma vez. Então a condição é avaliada. Se a condição for avaliada como true, o bloco será executado novamente. O looping para quando a condição for avaliada como false.

Note que o loop whileand do...whilesão diferentes! Ao contrário do whileloop, do...whileserá executado pelo menos uma vez, independentemente de a condição ser avaliada como true.

const firstMessage = 'I will print!';
const secondMessage = 'I will not print!'; 

// A do while with a stopping condition that evaluates to false
do {
 console.log(firstMessage)
} while (true === false);

// A while loop with a stopping condition that evaluates to false
while (true === false){
  console.log(secondMessage)
};

Observação: para sair de um loop infinito em um exercício, atualize a página e corrija o código do(s) seu(s) loop(s).

Instruções
Checkpoint 1 Passed
1 .
Gostaríamos de um programa para simular parte do processo de assar bolos. Dependendo da receita, um número diferente de xícaras de açúcar é necessário. Crie a variável cupsOfSugarNeedede atribua a ela um valor numérico de sua escolha.

As xícaras de açúcar devem ser adicionadas à massa uma de cada vez. Declare a variável cupsAddede atribua a ela o valor 0.

Ponto de verificação 2 aprovado
2 .
Gostamos de doces, então queremos adicionar pelo menos uma xícara de açúcar à massa, mesmo que o valor de cupsOfSugarNeededseja 0.

Crie um do...whileloop que incremente cupsAddedem um enquanto cupsAddedfor menor que cupsOfSugarNeeded.

Para nos ajudar a visualizar a saída em cada iteração do loop, adicione console.logdentro do do...whilebloco e registre o valor de cupsAdded.