OBJETOS
Métodos
10 minutos
Quando os dados armazenados em um objeto são uma função, chamamos isso de método . Uma propriedade é o que um objeto tem, enquanto um método é o que um objeto faz.

Os métodos de objeto parecem familiares? Isso porque você os tem usado o tempo todo! Por exemplo, consoleé um objeto JavaScript global e .log()é um método naquele objeto. Mathtambém é um objeto JavaScript global e .floor()é um método nele.

Podemos incluir métodos em nossos literais de objeto criando pares chave-valor comuns, separados por dois pontos. A chave serve como o nome do nosso método, enquanto o valor é uma expressão de função anônima.

const alienShip = {
  invade: function () { 
    console.log('Hello! We have come to dominate your planet. Instead of Earth, it shall be called New Xaculon.')
  }
};

Com a nova sintaxe de método introduzida no ES6, podemos omitir os dois pontos e a functionpalavra-chave.

const alienShip = {
  invade () { 
    console.log('Hello! We have come to dominate your planet. Instead of Earth, it shall be called New Xaculon.')
  }
};

Os métodos de objeto são invocados anexando o nome do objeto com o operador ponto seguido pelo nome do método e parênteses:

alienShip.invade(); // Prints 'Hello! We have come to dominate your planet. Instead of Earth, it shall be called New Xaculon.'

Instruções
Checkpoint 1 Passed
1 .
Abaixo da retreatMessagevariável no editor de código, crie um alienShipobjeto. Ele deve conter um método retreat()que irá console.log()o retreatMessage.

Ponto de verificação 2 aprovado
2 .
Adicione outro método ao seu literal de objeto. Este método, takeOff(), deve ser console.log()a string 'Spim... Borp... Glix... Blastoff!'.

Ponto de verificação 3 aprovado
3 .
Invoque seus dois métodos: primeiro .retreat()e depois .takeOff().