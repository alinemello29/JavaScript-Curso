OBJETOS
Notação de colchetes
8 minutos
A segunda maneira de acessar o valor de uma chave é usando a notação de colchetes, [ ].

Você usou a notação de colchetes ao indexar uma matriz:

['A', 'B', 'C'][0]; // Returns 'A'

Para usar a notação de colchetes para acessar a propriedade de um objeto, passamos o nome da propriedade (chave) como uma string.


Devemos usar notação de colchetes ao acessar chaves que tenham números, espaços ou caracteres especiais. Sem notação de colchetes nessas situações, nosso código lançaria um erro.

let spaceship = {
  'Fuel Type': 'Turbo Fuel',
  'Active Duty': true,
  homePlanet: 'Earth',
  numCrew: 5
};
spaceship['Active Duty'];   // Returns true
spaceship['Fuel Type'];   // Returns  'Turbo Fuel'
spaceship['numCrew'];   // Returns 5
spaceship['!!!!!!!!!!!!!!!'];   // Returns undefined

Com a notação de colchetes, você também pode usar uma variável dentro dos colchetes para selecionar as chaves de um objeto. Isso pode ser especialmente útil ao trabalhar com funções:

let returnAnyProp = (objectName, propName) => objectName[propName];
 
returnAnyProp(spaceship, 'homePlanet'); // Returns 'Earth'

Se tentássemos escrever nossa returnAnyProp()função com a notação de ponto ( objectName.propName), o computador procuraria uma chave de 'propName'em nosso objeto e não o valor do propNameparâmetro.

Vamos praticar o uso da notação de colchetes para acessar propriedades!

Instruções
Checkpoint 1 Passed
1 .
Vamos usar a notação de colchetes para acessar o valor de 'Active Mission'from do spaceshipobjeto no editor de código. Crie uma variável isActivee atribua a propriedade spaceship's a ela.'Active Mission'

Ponto de verificação 2 aprovado
2 .
Usando a notação de colchetes e a propNamevariável fornecida, console.log()o valor da 'Active Mission'propriedade.