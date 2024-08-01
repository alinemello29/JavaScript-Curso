FUNÇÕES DE ORDEM SUPERIOR
Funções como Parâmetros

Como você sabe, um parâmetro é um espaço reservado para os dados que são passados ​​para uma função. Como as funções podem se comportar como qualquer outro tipo de dado em JavaScript, pode não ser surpresa para você saber que as funções podem aceitar outras funções como parâmetros. Uma função de ordem superior é uma função que aceita funções como parâmetros, retorna uma função ou ambos! Chamamos funções que são passadas como parâmetros de funções de retorno de chamada . As funções de retorno de chamada são invocadas durante a execução da função de ordem superior.

Quando invocamos uma função de ordem superior e passamos outra função como argumento, não invocamos a função argumento. Invocá-la avaliaria a passagem do valor de retorno dessa chamada de função. Com funções de retorno de chamada, passamos a função em si digitando o nome da função sem os parênteses:

const higherOrderFunc = param => {
  param();
  return `I just invoked ${param.name} as a callback function!`
}
 
const anotherFunc = () => {
  return 'I\'m being invoked by the higher-order function!';
}

higherOrderFunc(anotherFunc);

Escrevemos uma função de ordem superior higherOrderFuncque aceita um único parâmetro, param. Dentro do corpo, paramé invocado usando parênteses. E, finalmente, uma string é retornada, nos dizendo o nome da função de retorno de chamada que foi passada.

Abaixo da função de ordem superior, temos outra função apropriadamente chamada anotherFunc. Esta função aspira ser chamada dentro da função de ordem superior.

Por fim, invocamos higherOrderFunc(), passando anotherFunccomo seu argumento, realizando assim seu sonho de ser chamado pela função de ordem superior.

higherOrderFunc(() => {
  for (let i = 0; i <= 10; i++){
    console.log(i);
  }
});

Neste exemplo, invocamos higherOrderFunc()uma função anônima (uma função sem nome) que conta até 10. Funções anônimas também podem ser argumentos!

Vamos praticar a escrita de funções de ordem superior.

Instruções
Checkpoint 1 Passed
1 .
Aqui temos uma função, addTwo(), que adiciona 2 a tudo o que é passado para ela. Abaixo disso, criamos o que será uma função de ordem superior, checkConsistentOutput(). O propósito da função de ordem superior será verificar o trabalho de addTwo(). Vamos começar!

Para começar, dentro do corpo de checkConsistentOutput(), declare duas variáveis: checkAe checkB:

checkAarmazena a soma valmais 2.
checkBarmazena a invocação do retorno de funcchamada, com valcomo argumento.
Ponto de verificação 2 aprovado
2 .
Em seguida, abaixo das variáveis, escreva uma instrução condicional que verifica se o valor de checkAé igual ao valor checkB. Se verdadeiro, retorna o resultado da função de retorno de chamada. Se falso, retorna a string 'inconsistent results'.

Ponto de verificação 3 aprovado
3 .
Por fim, usando console.log(), registre a invocação de checkConsistentOutput()com dois argumentos: a addTwo()função e qualquer número.

