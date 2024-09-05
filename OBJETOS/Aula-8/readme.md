OBJETOS
Passar por referência
15 minutos
Objetos são passados ​​por referência . Isso significa que quando passamos uma variável atribuída a um objeto em uma função como um argumento, o computador interpreta o nome do parâmetro como apontando para o espaço na memória que contém esse objeto. Como resultado, funções que alteram propriedades do objeto na verdade mutam o objeto permanentemente (mesmo quando o objeto é atribuído a uma constvariável).

const spaceship = {
  homePlanet : 'Earth',
  color : 'silver'
};
 
let paintIt = obj => {
  obj.color = 'glorious gold'
};
 
paintIt(spaceship);
 
spaceship.color // Returns 'glorious gold'
 

Nossa função paintIt()alterou permanentemente a cor do nosso spaceshipobjeto. No entanto, a reatribuição da spaceshipvariável não funcionaria da mesma forma:

let spaceship = {
  homePlanet : 'Earth',
  color : 'red'
};
let tryReassignment = obj => {
  obj = {
    identified : false, 
    'transport type' : 'flying'
  }
  console.log(obj) // Prints {'identified': false, 'transport type': 'flying'}
 
};
tryReassignment(spaceship) // The attempt at reassignment does not work.
spaceship // Still returns {homePlanet : 'Earth', color : 'red'};
 
spaceship = {
  identified : false, 
  'transport type': 'flying'
}; // Regular reassignment still works.

Vejamos o que aconteceu no exemplo de código:

Declaramos esse spaceshipobjeto com let. Isso nos permitiu reatribuí-lo a um novo objeto com propriedades identifiede 'transport type'sem problemas.
Quando tentamos a mesma coisa usando uma função projetada para reatribuir o objeto passado a ela, a reatribuição não funcionou (embora a chamada console.log()ao objeto tenha produzido o resultado esperado).
Quando passamos spaceshippara essa função, objtornou-se uma referência ao local de memória do spaceshipobjeto, mas não à spaceshipvariável. Isso ocorre porque o objparâmetro da tryReassignment()função é uma variável por si só. O corpo de tryReassignment()não tem conhecimento algum da spaceshipvariável!
Quando fizemos a reatribuição no corpo de tryReassignment(), a objvariável passou a se referir ao local de memória do objeto {'identified' : false, 'transport type' : 'flying'}, enquanto a spaceshipvariável permaneceu completamente inalterada em relação ao seu valor anterior.
Instruções
Checkpoint 1 Passed
1 .
Escreva uma função greenEnergy()que tenha um objeto como parâmetro e defina 'Fuel Type'a propriedade desse objeto como 'avocado oil'.

Ponto de verificação 2 aprovado
2 .
Escreva uma função remotelyDisable()que tenha um objeto como parâmetro e defina (ou reatribua) a disabledpropriedade desse objeto como true.

Ponto de verificação 3 aprovado
3 .
Chame suas duas funções com o spaceshipobjeto no editor de código e, em seguida, console.log()o spaceshipobjeto para confirmar se essas propriedades foram alteradas/adicionadas.