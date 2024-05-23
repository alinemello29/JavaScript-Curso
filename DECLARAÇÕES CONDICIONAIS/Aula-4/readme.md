DECLARAÇÕES CONDICIONAIS
Operadores de comparação

Ao escrever instruções condicionais, às vezes precisamos usar diferentes tipos de operadores para comparar valores. Esses operadores são chamados de operadores de comparação .

Aqui está uma lista de alguns operadores de comparação úteis e sua sintaxe:

Menor que:<
Maior que:>
Menos que ou igual a:<=
Melhor que ou igual a:>=
É igual a:===
Não é igual a:!==
Os operadores de comparação comparam o valor à esquerda com o valor à direita. Por exemplo:

10 < 12 // Evaluates to true

Pode ser útil pensar nas afirmações de comparação como perguntas. Quando a resposta é “sim”, a afirmação é avaliada como true, e quando a resposta é “não”, a afirmação é avaliada como false. O código acima estaria perguntando: 10 é menor que 12? Sim! Então 10 < 12avalia como true.

Também podemos usar operadores de comparação em diferentes tipos de dados, como strings:

'apples' === 'oranges' // false

No exemplo acima, estamos usando o operador de identidade ( ===) para verificar se a string 'apples'é igual à string 'oranges'. Como as duas strings não são iguais, a instrução de comparação é avaliada como false.

Todas as declarações de comparação são avaliadas como trueou falsee são compostas por:

Dois valores que serão comparados.
Um operador que separa os valores e os compara adequadamente ( >, <, <=, >=, ===, !==).
Vamos praticar o uso desses operadores de comparação!

Instruções
Checkpoint 1 Passed
1 .
Usando let, crie uma variável chamada hungerLevele defina-a igual a 7.

Ponto de verificação 2 aprovado
2 .
Escreva uma if...elsedeclaração usando um operador de comparação. A condição deve verificar se hungerLevelé maior que 7. Nesse caso, a instrução condicional deve registrar, 'Time to eat!'. Caso contrário, ele deverá registrar 'We can eat later!'.

Depois de pressionar executar, brinque com a condição ajustando a comparação hungerLevelusando diferentes operadores, como <=, >=, >e <.