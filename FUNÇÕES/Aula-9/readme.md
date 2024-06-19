FUNÇÕES
Funções de seta

ES6 introduziu a sintaxe de função de seta , uma maneira mais curta de escrever funções usando a () =>notação especial “seta gorda”.

As funções de seta eliminam a necessidade de digitar a palavra-chave functionsempre que você precisar criar uma função. Em vez disso, você primeiro inclui os parâmetros dentro de ( )e depois adiciona uma seta =>que aponta para o corpo da função cercado { }assim:

const rectangleArea = (width, height) => {
  let area = width * height;
  return area;
};

É importante estar familiarizado com as diversas maneiras de escrever funções porque você encontrará cada uma delas ao ler outro código JavaScript.

Instruções
Checkpoint 1 Passed
1 .
Mude plantNeedsWater()para usar a sintaxe da função de seta.