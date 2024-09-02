OBJETOS
Cessão de Propriedade
8 minutos
Uma vez que definimos um objeto, não estamos presos a todas as propriedades que escrevemos. Objetos são mutáveis , o que significa que podemos atualizá-los depois de criá-los!

Podemos usar a notação de ponto, ., ou a notação de colchetes, [], e o operador de atribuição, = para adicionar novos pares de chave-valor a um objeto ou alterar uma propriedade existente.

diagrama mostrando como um objeto seguido por colchetes ([]) com o nome da propriedade como uma string pode ser reatribuído a um novo valor. Essa mesma ideia se aplica para acessar uma propriedade usando notação de ponto que tem o nome do objeto, seguido por um ponto e o nome da propriedade

Uma de duas coisas pode acontecer com a atribuição de propriedade:

Se a propriedade já existir no objeto, qualquer valor que ela continha antes será substituído pelo novo valor atribuído.
Se não houver nenhuma propriedade com esse nome, uma nova propriedade será adicionada ao objeto.
É importante saber que, embora não possamos reatribuir um objeto declarado com const, ainda podemos alterá-lo, o que significa que podemos adicionar novas propriedades e alterar as propriedades que estão lá.

const spaceship = {type: 'shuttle'};
spaceship = {type: 'alien'}; // TypeError: Assignment to constant variable.
spaceship.type = 'alien'; // Changes the value of the type property
spaceship.speed = 'Mach 5'; // Creates a new key of 'speed' with a value of 'Mach 5'

Você pode excluir uma propriedade de um objeto com o deleteoperador.

const spaceship = {
  'Fuel Type': 'Turbo Fuel',
  homePlanet: 'Earth',
  mission: 'Explore the universe' 
};
 
delete spaceship.mission;  // Removes the mission property

Instruções
Checkpoint 1 Passed
1 .
Reatribuir a colorpropriedade do spaceshipobjeto para ter um valor de'glorious gold'

Ponto de verificação 2 aprovado
2 .
Sem alterar as linhas 1 a 6, adicione uma numEnginespropriedade com um valor numérico entre 1 e 10 ao spaceshipobjeto.

Ponto de verificação 3 aprovado
3 .
Use o deleteoperador para remover a 'Secret Mission'propriedade do spaceshipobjeto.