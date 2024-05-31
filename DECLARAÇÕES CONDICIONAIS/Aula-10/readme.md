DECLARAÇÕES CONDICIONAIS
A palavra-chave switch

else if declarações são uma ótima ferramenta se precisarmos verificar múltiplas condições. Na programação, muitas vezes precisamos verificar vários valores e lidar com cada um deles de maneira diferente. Por exemplo:

let groceryItem = 'papaya';

if (groceryItem === 'tomato') {
  console.log('Tomatoes are $0.49');
} else if (groceryItem === 'papaya'){
  console.log('Papayas are $1.29');
} else {
  console.log('Invalid item');
}

No código acima, temos uma série de condições verificando um valor que corresponda a uma groceryItemvariável. Nosso código funciona bem, mas imagine se precisássemos verificar 100 valores diferentes! Ter que escrever tantas else ifdeclarações parece uma dor!

Uma switchinstrução fornece uma sintaxe alternativa que é mais fácil de ler e escrever. Uma switchdeclaração é assim:

let groceryItem = 'papaya';

switch (groceryItem) {
  case 'tomato':
    console.log('Tomatoes are $0.49');
    break;
  case 'lime':
    console.log('Limes are $1.49');
    break;
  case 'papaya':
    console.log('Papayas are $1.29');
    break;
  default:
    console.log('Invalid item');
    break;
}

// Prints 'Papayas are $1.29'

A switchpalavra-chave inicia a instrução e é seguida por ( ... ), que contém o valor que cada uma caseirá comparar. No exemplo, o valor ou expressão da switchinstrução é groceryItem.
Dentro do bloco { ... }, existem vários cases. A casepalavra-chave verifica se a expressão corresponde ao valor especificado que vem depois dela. O valor após o primeiro caseé 'tomato'. Se o valor de groceryItemequaled 'tomato', isso caseseria console.log()executado.
O valor de groceryItemé 'papaya', então a terceira caseexecução Papayas are $1.29é registrada no console.
A breakpalavra-chave diz ao computador para sair do bloco e não executar mais nenhum código ou verificar quaisquer outros casos dentro do bloco de código. Observação: sem breakpalavras-chave, o primeiro caso correspondente será executado, mas o mesmo acontecerá com todos os casos subsequentes, independentemente de corresponderem ou não — incluindo o padrão. Esse comportamento é diferente das instruções if/ elsecondicionais que executam apenas um bloco de código.
No final de cada switchdeclaração, há uma defaultdeclaração. Se nenhum dos cases for verdadeiro, o código na defaultinstrução será executado.
Instruções
Checkpoint 1 Passed
1 .
Vamos escrever um switchcomunicado para decidir qual medalha conceder a um atleta.

athleteFinalPositionjá está definido no topo de main.js . Portanto, comece escrevendo uma switchdeclaração tendo athleteFinalPositioncomo expressão.

Ponto de verificação 2 aprovado
2 .
Dentro da switchdeclaração, adicione três cases:

A primeira caseverifica o valor'first place'
Se o valor da expressão corresponder ao valor de caseentão console.log()a string'You get the gold medal!'
O segundo caseverifica o valor'second place'
Se o valor da expressão corresponder ao valor de caseentão console.log()a string'You get the silver medal!'
O terceiro caseverifica o valor'third place'
Se o valor da expressão corresponder ao valor de caseentão console.log()a string'You get the bronze medal!'
Lembre-se de adicionar um breakapós cada um console.log().

Ponto de verificação 3 aprovado
3 .
Agora, adicione uma defaultinstrução no final do switchque usa console.log()para print 'No medal awarded.'.

Se athleteFinalPositionnão for igual a nenhum valor de nosso cases, a string 'No medal awarded.'será registrada no console.

Lembre-se de adicionar a breakpalavra-chave no final do defaultcaso.