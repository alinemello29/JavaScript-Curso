DECLARAÇÕES CONDICIONAIS
Declaração Se

Freqüentemente executamos uma tarefa com base em uma condição. Por exemplo, se o tempo estiver bom hoje, sairemos. Se o despertador tocar, nós o desligaremos. Se estivermos cansados, iremos dormir.

Na programação, também podemos executar uma tarefa baseada em uma condição usando uma ifinstrução:

if (true) {
  console.log('This message will print!'); 
}
// Prints: This message will print!

Observe no exemplo acima, temos uma ifdeclaração. A ifdeclaração é composta por:

A ifpalavra-chave seguida por um conjunto de parênteses ()que é seguido por um bloco de código , ou instrução de bloco , indicado por um conjunto de chaves {}.
Dentro dos parênteses (), é fornecida uma condição avaliada como trueou false.
Se a condição for avaliada como true, o código entre chaves {}será executado ou executado .
Se a condição for avaliada como false, o bloco não será executado.
Vamos fazer uma ifdeclaração.

Instruções
Checkpoint 1 Passed
1 .
Usando a letpalavra-chave, declare uma variável chamada sale. Atribua o valor truea ele.

Ponto de verificação 2 aprovado
2 .
Agora crie uma ifdeclaração. Forneça à ifdeclaração uma condição de sale.

Dentro do bloco de código da ifinstrução, console.log()a string 'Time to buy!'.

Ponto de verificação 3 aprovado
3 .
Observe que o código dentro da ifinstrução foi executado, pois 'Time to buy!'foi registrado no console.

Abaixo da saledeclaração da variável, mas antes da ifinstrução, reatribua salepara false. Execute seu código e observe o que acontece, mudaremos esse comportamento no próximo exercício.