OBJETOS AVANÇADOS
Funções de fábrica
11 minutos
Até agora, criamos objetos individualmente, mas há momentos em que queremos criar muitas instâncias de um objeto rapidamente. É aqui que entram as funções de fábrica . Uma fábrica do mundo real fabrica várias cópias de um item rapidamente e em grande escala. Uma função de fábrica é uma função que retorna um objeto e pode ser reutilizada para criar várias instâncias de objeto. As funções de fábrica também podem ter parâmetros que nos permitem personalizar o objeto que é retornado.

Digamos que quiséssemos criar um objeto para representar monstros em JavaScript. Existem muitos tipos diferentes de monstros e poderíamos fazer cada monstro individualmente, mas também podemos usar uma função de fábrica para facilitar nossas vidas. Para atingir esse plano diabólico de criar vários objetos de monstros, podemos usar uma função de fábrica que tenha parâmetros:

const monsterFactory = (name, age, energySource, catchPhrase) => {
  return { 
    name: name,
    age: age, 
    energySource: energySource,
    scare() {
      console.log(catchPhrase);
    } 
  }
};

Na monsterFactoryfunção acima, ela tem quatro parâmetros e retorna um objeto que tem as propriedades: name, age, energySource, e scare(). Para fazer um objeto que representa um monstro específico como um fantasma, podemos chamar monsterFactorycom os argumentos necessários e atribuir o valor de retorno a uma variável:

const ghost = monsterFactory('Ghouly', 251, 'ectoplasm', 'BOO!');
ghost.scare(); // 'BOO!'

Agora temos um ghostobjeto como resultado da chamada monsterFactory()com os argumentos necessários. Com monsterFactoryo in place, não precisamos criar um literal de objeto toda vez que precisamos de um novo monstro. Em vez disso, podemos invocar a monsterFactoryfunção com os argumentos necessários paradominar o mundofaça um monstro para nós!

Instruções
Checkpoint 1 Passed
1 .
Em vez de criar robôs individuais como temos feito, vamos criar uma função de fábrica para criar robôs como quisermos!

Crie uma função de fábrica chamada robotFactoryque tenha dois parâmetros modele mobile. Faça a função retornar um objeto. No objeto, adicione uma chave de modelcom o valor do modelparâmetro. Adicione outra propriedade que tenha uma chave de mobilecom um valor do mobileparâmetro.

Em seguida, adicione um método chamado beepsem um parâmetro que registrará 'Beep Boop'no console.

Ponto de verificação 2 aprovado
2 .
Use sua função de fábrica declarando uma constvariável chamada tinCan. Atribua ao tinCanvalor de chamando robotFactorycom o primeiro argumento de 'P-500'e o segundo argumento de true.

Ponto de verificação 3 aprovado
3 .
Vamos agora verificar o que tinCanpode fazer! Ligue .beep()para tinCan.

Você deve ver 'Beep Boop'impresso no console, o que significa que a função de fábrica produziu um objeto robô! Brinque com tinCanpara verificar as outras propriedades!