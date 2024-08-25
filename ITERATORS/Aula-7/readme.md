ITERADORES
Documentação do Iterador
12 minutos
Existem muitos métodos de array integrados adicionais , uma lista completa dos quais está na página Métodos de iteração de array do MDN .

A documentação de cada método contém várias seções:

Uma breve definição.
Um bloco com a sintaxe correta para usar o método.
Uma lista de parâmetros que o método aceita ou requer.
O valor de retorno da função.
Uma descrição estendida.
Exemplos de uso do método.
Outras informações adicionais.
Nas instruções abaixo, há alguns erros no código. Use a documentação de um método dado para determinar o erro ou preencha um espaço em branco para fazer o código rodar corretamente.

Instruções
Checkpoint 1 Passed
1 .
No editor de código, há um array chamado words. Queremos criar um novo array de palavras interessantes. A primeira coisa que queremos fazer é verificar se há palavras com menos de 6caracteres de comprimento. Há algo faltando na words.some()chamada do método. Corrija esse método para que trueseja impresso no console.

Para mais informações, navegue pela documentação do MDN em.some() .

Ponto de verificação 2 aprovado
2 .
O .some()método retornou true, o que significa que há algumas palavras no array que são menores que seis caracteres. Use o .filter()método para salvar quaisquer palavras maiores que 5caracteres em uma nova variável chamada interestingWords, declarada com const.

Usamos isso .filter()em um exercício anterior, mas, para mais informações, navegue pela documentação do MDN em.filter() .

Ponto de verificação 3 aprovado
3 .
Na última linha do main.js , há este código:

// console.log(interestingWords.every(word =>        ));

Complete o código entre parênteses para verificar se cada elemento tem mais de 5 caracteres.

Certifique-se de descomentar (excluir o //antes) a última linha do programa antes de executar o código.

Para mais informações, navegue pela documentação do MDN em.every() .