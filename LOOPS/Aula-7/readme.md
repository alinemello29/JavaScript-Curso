O Loop While

Você está indo muito bem! Vamos lhe ensinar sobre um tipo diferente de loop: o whileloop . Para começar, vamos converter um forloop em um whileloop:

// A for loop that prints 1, 2, and 3
for (let counterOne = 1; counterOne < 4; counterOne++){
  console.log(counterOne);
}

// A while loop that prints 1, 2, and 3
let counterTwo = 1;
while (counterTwo < 4) {
  console.log(counterTwo);
  counterTwo++;
}

Vamos analisar o que está acontecendo com nossa whilesintaxe de loop:

A counterTwovariável é declarada antes do loop. Podemos acessá-la dentro do nosso whileloop, já que ela está no escopo global.
Começamos nosso loop com a palavra-chave whileseguida por nossa condição de parada, ou condição de teste . Isso será avaliado antes de cada rodada do loop. Enquanto a condição for avaliada como true, o bloco continuará a ser executado. Uma vez que for avaliada como , falseo loop será interrompido.
Em seguida, temos o bloco de código do nosso loop que imprime counterTwono console e incrementa counterTwo.
O que aconteceria se não incrementássemos counterTwodentro do nosso bloco? Se não incluíssemos isso, counterTwosempre teria seu valor inicial, 1. Isso significaria que a condição de teste counterTwo < 4sempre avaliaria truee nosso loop nunca pararia de rodar! Lembre-se, isso é chamado de loop infinito e é algo que sempre queremos evitar . Loops infinitos podem ocupar todo o poder de processamento do seu computador, potencialmente congelando seu computador.

Então você pode estar se perguntando quando usar um whileloop! A sintaxe de um whileloop é ideal quando não sabemos com antecedência quantas vezes o loop deve ser executado. Pense em comer como um whileloop: quando você começa a dar mordidas, você não sabe o número exato que precisará para ficar satisfeito. Em vez disso, você comerá porque whileestá com fome. Em situações em que queremos que um loop seja executado um número indeterminado de vezes, whileos loops são a melhor escolha.

Instruções
Checkpoint 1 Passed
1 .
Abaixo do cardsarray, declare uma variável, currentCard, com a letpalavra-chave, mas não atribua um valor a ela.

Ponto de verificação 2 aprovado
2 .
Crie um whileloop com uma condição que verifica se o currentCardnão tem esse valor 'spade'.

Dentro do bloco do seu whileloop, adicione a seguinte linha de código:

currentCard = cards[Math.floor(Math.random() * 4)];

Math.floor(Math.random() * 4)nos dará um número aleatório de 0a 3. Usaremos esse número para indexar o cardsarray e atribuir o valor de currentCarda um elemento aleatório daquele array.

Se você notar o botão Executar girando continuamente ou uma mensagem “Conexão perdida com o Codecademy” em um exercício, você pode ter um loop infinito! Se a condição de parada para nosso loop nunca for atendida, criaremos um loop infinito que impede nosso programa de executar qualquer outra coisa. Para sair de um loop infinito em um exercício, atualize a página — então corrija o código para seu loop.

Ponto de verificação 3 aprovado
3 .
Incrível! Seu loop está em execução, mas você não consegue perceber porque ele não produz nada. Vamos adicionar uma console.log()declaração ao nosso whilebloco. Dentro do bloco, depois de atribuir currentCardum novo valor, faça log currentCardno console.

Para se divertir, você pode executar seu código algumas vezes e ver como a saída muda!