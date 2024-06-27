ESCOPO
Poluição do Escopo

Pode parecer uma ótima ideia tornar suas variáveis ​​sempre acessíveis, mas ter muitas variáveis ​​globais pode causar problemas em um programa.

Quando você declara variáveis ​​globais, elas vão para o namespace global . O namespace global permite que as variáveis ​​sejam acessíveis de qualquer lugar do programa. Essas variáveis ​​permanecem lá até o programa terminar, o que significa que nosso namespace global pode ser preenchido muito rapidamente.

A poluição do escopo ocorre quando temos muitas variáveis ​​globais no namespace global ou quando reutilizamos variáveis ​​em diferentes escopos. A poluição de escopo torna difícil acompanhar nossas diferentes variáveis ​​e nos prepara para possíveis acidentes. Por exemplo, variáveis ​​com escopo global podem colidir com outras variáveis ​​com escopo mais local, causando comportamento inesperado em nosso código.

Vejamos um exemplo de poluição de escopo na prática para sabermos como evitá-la:

let num = 50;

const logNum = () => {
  num = 100; // Take note of this line of code
  console.log(num);
};

logNum(); // Prints 100
console.log(num); // Prints 100

Você notará:

Temos uma variável num.
Dentro do corpo da função logNum(), queremos declarar uma nova variável, mas esquecemos de usar a letpalavra-chave.
Quando ligamos logNum(), numele é reatribuído para 100.
A reatribuição interna logNum()afeta a variável global num.
Mesmo que a reatribuição seja permitida e não recebamos um erro, se decidirmos usar nummais tarde, usaremos, sem saber, o novo valor de num.
Embora seja importante saber o que é o escopo global, é uma prática recomendada não definir variáveis ​​no escopo global.

Instruções
Checkpoint 1 Passed
1 .
Vamos ver o que acontece se criarmos uma variável que sobrescreva uma variável global.

Dentro da callMyNightSky()função, na primeira linha do corpo da função, atribua a variável starscomo 'Sirius'tal:

stars = 'Sirius';

Ponto de verificação 2 aprovado
2 .
Fora da função, na console.log()instrução atual, adicione outra console.log()instrução para registrar starsno console.

Você notará que a variável global starsfoi reatribuída para 'Sirius'. Em outras palavras, alteramos o valor da starsvariável global, mas não é fácil ler exatamente o que aconteceu. Esta é uma má prática na manutenção do código e pode impactar nosso programa de maneiras que não pretendemos.