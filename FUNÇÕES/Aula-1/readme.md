FUNÇÕES
O que são funções?

Ao aprender como calcular a área de um retângulo pela primeira vez, há uma sequência de etapas para calcular a resposta correta:

Meça a largura do retângulo.
Meça a altura do retângulo.
Multiplique a largura e a altura do retângulo.
Com prática, você pode calcular a área do retângulo sem ser instruído sempre com essas três etapas.

Podemos calcular a área de um retângulo com o seguinte código:

const width = 10;
const height = 6;
const area =  width * height;
console.log(area); // Output: 60

Imagine ser solicitado a calcular a área de três retângulos diferentes:

// Area of the first rectangle
const width1 = 10;
const height1 = 6;
const area1 =  width1 * height1;

// Area of the second rectangle
const width2 = 4;
const height2 = 9;
const area2 =  width2 * height2;

// Area of the third rectangle
const width3 = 10;
const height3 = 10;
const area3 =  width3 * height3;

Na programação, costumamos usar código para executar uma tarefa específica várias vezes. Em vez de reescrever o mesmo código, podemos agrupar um bloco de código e associá-lo a uma tarefa, e então podemos reutilizar esse bloco de código sempre que precisarmos executar a tarefa novamente. Conseguimos isso criando uma função . Uma função é um bloco de código reutilizável que agrupa uma sequência de instruções para executar uma tarefa específica.

Nesta lição, você aprenderá como criar e usar funções e como elas podem ser usadas para criar um código mais claro e conciso.

Instruções
Dê uma olhada no GIF fornecido. Ele mostra uma função chamada addOneSide, adicionando um lado adicional a diferentes entradas de forma. Observe como existe apenas uma função, representada pela caixa, que é usada para transformar formas individuais (entradas) em novas formas (saídas).