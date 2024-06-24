ESCOPO
Blocos e Escopo

Antes de falarmos mais sobre escopo, primeiro precisamos falar sobre blocos .

Já vimos blocos usados ​​antes em funções e if instruções . Um bloco é o código encontrado dentro de um conjunto de chaves {}. Os blocos nos ajudam a agrupar uma ou mais instruções e servem como um importante marcador estrutural para nosso código.

Um bloco de código poderia ser uma função, assim:

const logSkyColor = () => {
  let color = 'blue'; 
  console.log(color); // blue 
}

Observe que o corpo da função é na verdade um bloco de código.

Observe o bloco em uma ifdeclaração:

if (dusk) {
  let color = 'pink';
  console.log(color); // pink
}

Nos próximos exercícios, veremos como os blocos definem o escopo das variáveis .

Instruções
Checkpoint 1 Passed
1 .
No topo de main.js , declare uma constvariável chamada cityset equal to 'New York City'. Esta variável existirá fora do bloco.

Ponto de verificação 2 aprovado
2 .
Abaixo da cityvariável, escreva uma função chamada logCitySkyline.

Ponto de verificação 3 aprovado
3 .
Dentro do corpo da função logCitySkyline(), escreva outra variável usando letnomeado skyscrapere defina-a igual a 'Empire State Building'.

Ponto de verificação 4 aprovado
4 .
Dentro da função, inclua uma instrução de retorno como esta:

return 'The stars over the ' + skyscraper + ' in ' + city;

Ponto de verificação 5 aprovado
5 .
Abaixo da logCitySkyline()função, use console.log()para registrar o valor de logCitySkyline()no console.

Você notará que a logCitySkyline()função é capaz de acessar ambas as variáveis ​​sem problemas. No próximo exercício consideraremos por que seria preferível ter uma variável fora de um bloco e a outra dentro de um bloco.