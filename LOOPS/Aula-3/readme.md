O loop For

Em vez de escrever o mesmo código repetidamente, os loops nos permitem dizer aos computadores para repetir um dado bloco de código por conta própria. Uma maneira de dar essas instruções aos computadores é com um forloop .

O loop típico forinclui uma variável iteradora que geralmente aparece em todas as três expressões. A variável iteradora é inicializada, verificada em relação à condição de parada e recebe um novo valor em cada iteração do loop. Variáveis ​​iteradoras podem ter qualquer nome, mas é uma prática recomendada usar um nome de variável descritivo.

Um forloop contém três expressões separadas ;entre parênteses:

uma inicialização inicia o loop e também pode ser usada para declarar a variável do iterador.
uma condição de parada é a condição em relação à qual a variável do iterador é avaliada — se a condição for avaliada como tal, trueo bloco de código será executado e, se for avaliado como tal, falseo código será interrompido.
uma instrução de iteração é usada para atualizar a variável do iterador em cada loop.
A forsintaxe do loop se parece com isto:

for (let counter = 0; counter < 4; counter++) {
  console.log(counter);
}

Neste exemplo, a saída seria a seguinte:

0
1
2
3

Vamos analisar o exemplo:

A inicialização é let counter = 0, então o loop começará a contar em 0.
A condição de parada é counter < 4, o que significa que o loop será executado enquanto a variável do iterador, counter, for menor que 4.
A declaração de iteração é counter++. Isso significa que após cada loop, o valor de counteraumentará em 1. Para a primeira iteração counterserá igual a 0, para a segunda iteração counterserá igual a 1, e assim por diante.
O bloco de código está dentro das chaves, console.log(counter), será executado até que a condição seja avaliada como false. A condição será falsa quando counterfor maior ou igual a 4 — o ponto em que a condição se torna falsa é às vezes chamado de condição de parada .
Este forloop torna possível escrever 0, 1, 2, e 3programaticamente.

Instruções
Checkpoint 1 Passed
1 .
Agora, faça o seu próprio! Crie um programa que faça um loop de 5 a 10 e registre cada número no console.

Ao escrever/alterar loops, há uma chance de que nossa condição de parada não seja atendida e tenhamos um temido loop infinito que essencialmente impede nossa programação de executar qualquer outra coisa! Para sair de um loop infinito em um exercício, atualize a página - então corrija o código para seu loop.