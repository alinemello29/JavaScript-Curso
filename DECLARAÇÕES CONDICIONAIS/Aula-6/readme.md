DECLARAÇÕES CONDICIONAIS
Verdadeiramente e falsamente

Vamos considerar como os tipos de dados não booleanos , como strings ou números, são avaliados quando verificados dentro de uma condição.

Às vezes, você desejará verificar se uma variável existe e não necessariamente desejará que ela seja igual a um valor específico - você apenas verificará se um valor foi atribuído à variável.

Aqui está um exemplo:

let myVariable = 'I Exist!';

if (myVariable) {
   console.log(myVariable)
} else {
   console.log('The variable does not exist.')
}

O bloco de código na ifinstrução será executado porque myVariabletem um valor verdadeiro ; mesmo que o valor de myVariablenão seja explicitamente o valor true, quando usado em um contexto booleano ou condicional, ele é avaliado como trueporque foi atribuído um valor não falso.

Então, quais valores são falsos - ou avaliados falsequando verificados como uma condição? A lista de valores falsos inclui:

0
Strings vazias como ""ou''
nullque representam quando não há valor algum
undefinedque representam quando uma variável declarada não possui um valor
NaNou não é um número
Aqui está um exemplo com números:

let numberOfApples = 0;

if (numberOfApples){
   console.log('Let us eat apples!');
} else {
   console.log('No apples left!');
}

// Prints 'No apples left!'

A condição é avaliada como falseporque o valor de numberOfApplesé 0. Como 0é um valor falso, o bloco de código na elseinstrução será executado.

Instruções
Checkpoint 1 Passed
1 .
Mude o valor de wordCountpara que seja verdadeiro. Este valor ainda deve ser um número.

Depois de fazer essa alteração e executar seu código, você 'Great! You've started your work!'deve efetuar login no console.

Ponto de verificação 2 aprovado
2 .
Altere o valor de favoritePhrasepara que ainda seja uma string, mas falsa.

Depois de fazer essa alteração e executar seu código, você 'This string is definitely empty.'deve efetuar login no console.