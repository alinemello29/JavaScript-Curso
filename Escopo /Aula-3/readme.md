ESCOPO
Âmbito global

Escopo é o contexto no qual nossas variáveis ​​são declaradas. Pensamos no escopo em relação aos blocos porque variáveis ​​podem existir fora ou dentro desses blocos.

No escopo global , as variáveis ​​são declaradas fora dos blocos. Essas variáveis ​​são chamadas de variáveis ​​globais . Como as variáveis ​​globais não estão vinculadas a um bloco, elas podem ser acessadas por qualquer código do programa, incluindo código em blocos.

Vejamos um exemplo de escopo global:

const color = 'blue';

const returnSkyColor = () => {
  return color; // blue 
};

console.log(returnSkyColor()); // blue

Mesmo que a colorvariável seja definida fora do bloco, ela pode ser acessada no bloco funcional, dando-lhe escopo global.
Por sua vez, colorpode ser acessado dentro do returnSkyColorbloco funcional.
Vamos trabalhar com variáveis ​​globais para ver como os dados podem ser acessíveis de qualquer lugar dentro de um programa.

Instruções
Checkpoint 1 Passed
1 .
No topo de main.js , escreva três variáveis ​​globais:

Nomeie a primeira variável satellitee defina-a igual a 'The Moon'.
Nomeie a segunda variável galaxye defina-a igual a 'The Milky Way'.
Nomeie a terceira variável starse defina-a igual a 'North Star'.
Ponto de verificação 2 aprovado
2 .
Abaixo das variáveis ​​criadas na etapa anterior, escreva uma função chamada callMyNightSky. Dentro da função, inclua uma instrução de retorno como esta:

return 'Night Sky: ' + satellite + ', ' + stars + ', and ' + galaxy;

Ponto de verificação 3 aprovado
3 .
Abaixo da callMyNightSky()função, use console.log()para registrar o valor de callMyNightSky()no console.

Você notará que o bloco de função callMyNightSky()é capaz de acessar livremente as variáveis ​​globais, pois as variáveis ​​estão disponíveis para todas as linhas de código do arquivo.

