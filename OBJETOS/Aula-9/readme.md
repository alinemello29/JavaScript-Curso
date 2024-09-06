OBJETOS
Looping através de objetos
15 minutos
Loops são ferramentas de programação que repetem um bloco de código até que uma condição seja atendida. Aprendemos como iterar por arrays usando sua indexação numérica, mas os pares chave-valor em objetos não são ordenados! JavaScript nos deu uma solução alternativa para iterar por objetos com a for...insintaxe .

for...inexecutará um determinado bloco de código para cada propriedade em um objeto.

let spaceship = {
  crew: {
    captain: { 
      name: 'Lily', 
      degree: 'Computer Engineering', 
      cheerTeam() { console.log('You got this!') } 
    },
    'chief officer': { 
      name: 'Dan', 
      degree: 'Aerospace Engineering', 
      agree() { console.log('I agree, captain!') } 
    },
    medic: { 
      name: 'Clementine', 
      degree: 'Physics', 
      announce() { console.log(`Jets on!`) } },
    translator: {
      name: 'Shauna', 
      degree: 'Conservation Science', 
      powerFuel() { console.log('The tank is full!') } 
    }
  }
}; 

// for...in
for (let crewMember in spaceship.crew) {
  console.log(`${crewMember}: ${spaceship.crew[crewMember].name}`);
}

Nosso for...inirá iterar por cada elemento do spaceship.crewobjeto. Em cada iteração, a variável crewMemberé definida para uma das spaceship.crewchaves de , permitindo-nos registrar uma lista de papéis e name.

Instruções
Checkpoint 1 Passed
1 .
Usando for...in, itere pelo spaceship.crewobjeto no editor de código e console.log()uma lista de funções e nomes da equipe no seguinte formato: '[crew member's role]: [crew member's name]', por exemplo, 'chief officer: Dan'.

Ponto de verificação 2 aprovado
2 .
Usando for...in, itere pelo spaceship.crewobjeto no editor de código e console.log()uma lista de nomes e graus da tripulação no seguinte formato: '[crew member's name]: [crew member's degree]', ou seja, 'Lily: Computer Engineering'.