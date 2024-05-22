DECLARAÇÕES CONDICIONAIS
Declarações If...Else

No exercício anterior, usamos uma ifinstrução que verificava uma condição para decidir se executaríamos ou não um bloco de código. Em muitos casos, teremos código que queremos executar se nossa condição for avaliada como false.

Se quisermos adicionar algum comportamento padrão à ifinstrução, podemos adicionar uma elseinstrução para executar um bloco de código quando a condição for avaliada como false. Dê uma olhada na inclusão de uma elsedeclaração:

if (false) {
  console.log('The code in this block will not run.');
} else {
  console.log('But the code in this block will!');
}

// Prints: But the code in this block will!

Uma elsedeclaração deve ser emparelhada com uma ifdeclaração e, juntas, elas são chamadas de if...elsedeclaração.

No exemplo acima, a elseafirmação:

Usa a elsepalavra-chave após o bloco de código de uma ifinstrução.
Possui um bloco de código envolvido por um conjunto de chaves {}.
O código dentro do elsebloco de código da instrução será executado quando a ifcondição da instrução for avaliada como false.
if...else as declarações nos permitem automatizar soluções para perguntas do tipo sim ou não, também conhecidas como decisões binárias .

Instruções
Checkpoint 1 Passed
1 .
Adicione uma elseinstrução à instrução existente if. Dentro do bloco de código da else instrução, console.log()a string'Time to wait for a sale.'