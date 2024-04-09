Comentários

A programação costuma ser altamente colaborativa. Além disso, nosso próprio código pode rapidamente se tornar difícil de entender quando voltamos a ele — às vezes, apenas uma hora depois! Por esses motivos, geralmente é útil deixar anotações em nosso código para outros desenvolvedores ou para nós mesmos.

À medida que escrevemos JavaScript, podemos escrever comentários em nosso código que o computador irá ignorar enquanto nosso programa for executado. Esses comentários existem apenas para leitores humanos.

Os comentários podem explicar o que o código está fazendo, deixar instruções para os desenvolvedores que usam o código ou adicionar quaisquer outras anotações úteis.

Existem dois tipos de comentários de código em JavaScript:

Um comentário de uma única linha comentará uma única linha e será indicado por duas barras //antes dela.
// Prints 5 to the console
console.log(5);

Você também pode usar um comentário de linha única para comentar após uma linha de código:

console.log(5);  // Prints 5 

Um comentário de várias linhas comentará várias linhas e será indicado com /*para iniciar e */finalizar o comentário.
/*
This is all commented 
console.log(10);
None of this is going to run!
console.log(99);
*/

Você também pode usar esta sintaxe para comentar algo no meio de uma linha de código:

console.log(/*IGNORED!*/ 5);  // Still just prints 5 

Instruções
Ponto de verificação 1 ativado
1 .
Vamos praticar a adição de alguns comentários ao código.

À direita, fornecemos o início do livro Catch-22 , de Joseph Heller.

Na linha 1, escreva um comentário de uma única linha que diga Opening line.