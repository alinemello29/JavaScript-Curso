ESCOPO
Pratique um bom escopo

Dados os desafios com variáveis ​​globais e poluição do escopo, devemos seguir as melhores práticas para definir o escopo de nossas variáveis ​​da forma mais precisa possível usando escopo de bloco.

Definir o escopo de suas variáveis ​​melhorará muito seu código de várias maneiras:

Isso tornará seu código mais legível, pois os blocos organizarão seu código em seções discretas.
Isso torna seu código mais compreensível, pois esclarece quais variáveis ​​estão associadas a diferentes partes do programa, em vez de ter que controlá-las linha após linha!
É mais fácil manter seu código, pois ele será modular.
Isso economizará memória em seu código porque ele deixará de existir após a execução do bloco.
Aqui está outro exemplo de como funciona o escopo do bloco, conforme definido dentro de um ifbloco:

const logSkyColor = () => {
  const dusk = true;
  let color = 'blue'; 
  if (dusk) {
    let color = 'pink';
    console.log(color); // Prints "pink"
  }
  console.log(color); // Prints "blue"
};

console.log(color); // throws a ReferenceError

Aqui você notará:

Criamos uma variável colordentro da logSkyColor()função.
Após a ifinstrução, definimos um novo bloco de código com {}colchetes. Aqui atribuímos um novo valor à variável colorse a ifafirmação for verdadeira.
Dentro do ifbloco, a colorvariável contém o valor 'pink', embora fora do ifbloco, no corpo da função, a colorvariável contém o valor 'blue'.
Na última linha, tentamos imprimir o valor colorfora da ifinstrução e da definição de logSkyColor(). Isso gerará um ReferenceErrordado que colorsó existe no escopo desses dois blocos — nunca é definido no escopo global.
Embora usemos escopo de bloco, ainda poluímos nosso namespace reutilizando o mesmo nome de variável duas vezes. Uma prática melhor seria renomear a variável dentro do bloco.
O escopo do bloco é uma ferramenta poderosa em JavaScript, pois nos permite definir variáveis ​​com precisão e não poluir o namespace global. Se uma variável não precisa existir fora de um bloco – ela não deveria existir!

Instruções
Checkpoint 1 Passed
1 .
Dentro do corpo da função logVisibleLightWaves(), abaixo da regionvariável e antes da console.log()instrução fornecida, crie uma ifinstrução que verifique se regioné o 'The Arctic'.

Ponto de verificação 2 aprovado
2 .
Dentro do ifbloco, defina uma nova letvariável lightWavese defina-a igual a 'Northern Lights'.

Ponto de verificação 3 aprovado
3 .
Abaixo da variável no ifbloco, use console.log()para registrar o valor da variável do bloco dentro do ifbloco.

Execute seu código e observe a saída. Dentro do ifbloco console.log(lightWaves)registra o valor Northern Lightsno console. Fora do ifbloco, mas ainda dentro da função, a mesma instrução é registrada Moonlightno console.