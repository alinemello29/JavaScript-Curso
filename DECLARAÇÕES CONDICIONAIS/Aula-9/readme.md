DECLARAÇÕES CONDICIONAIS
Declarações Else If

Podemos adicionar mais condições ao nosso if...elsecom uma else ifdeclaração . A else ifdeclaração permite mais de dois resultados possíveis. Você pode adicionar quantas else if instruções desejar para criar condicionais mais complexas!

A else ifdeclaração sempre vem depois da ifdeclaração e antes da elsedeclaração. A else ifdeclaração também requer uma condição. Vamos dar uma olhada na sintaxe:

let stopLight = 'yellow';

if (stopLight === 'red') {
  console.log('Stop!');
} else if (stopLight === 'yellow') {
  console.log('Slow down.');
} else if (stopLight === 'green') {
  console.log('Go!');
} else {
  console.log('Caution, unknown!');
}

As else ifdeclarações permitem que você tenha vários resultados possíveis. if// else ifas elseinstruções são lidas de cima para baixo, então a primeira condição avaliada truede cima para baixo é o bloco que é executado.

No exemplo acima, como stopLight === 'red'avalia falsee stopLight === 'yellow'avalia como true, o código dentro da primeira else ifinstrução é executado. As demais condições não são avaliadas. Se nenhuma das condições fosse avaliada como true, o código na elseinstrução teria sido executado.

Instruções
Checkpoint 1 Passed
1 .
Vamos criar um programa que acompanhe a forma como o ambiente muda com as estações. Escreva uma declaração condicional para fazer isso acontecer!

Em main.js já existe uma if...elsedeclaração em vigor. Vamos adicionar uma else ifinstrução que verifica se seasoné igual a 'winter'.

Dentro do bloco de código da else ifinstrução, adicione a console.log()que imprime a string 'It\'s winter! Everything is covered in snow.'.

Certifique-se de que a estrutura use if, else ife else.

Ponto de verificação 2 aprovado
2 .
Adicione outra else ifinstrução que verifique se seasoné igual a 'fall'.

Dentro do bloco de código da else ifinstrução que você acabou de criar, adicione um console.log()que imprima a string 'It\'s fall! Leaves are falling!'.

Ponto de verificação 3 aprovado
3 .
Adicione uma else ifinstrução final que verifique se seasoné igual a 'summer'.

Dentro do bloco de código da else ifinstrução que você acabou de criar, adicione um console.log()que imprima a string 'It\'s sunny and warm because it\'s summer!'.