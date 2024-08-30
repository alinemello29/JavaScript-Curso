OBJETOS
Acessando Propriedades
5 minutos
Há duas maneiras de acessarmos a propriedade de um objeto. Vamos explorar a primeira maneira — notação de ponto, ..

Você usou a notação de ponto para acessar as propriedades e métodos de objetos internos e instâncias de dados:

'hello'.length; // Returns 5

Com a notação de ponto de propriedade, escrevemos o nome do objeto, seguido pelo operador ponto e então o nome da propriedade (chave):

let spaceship = {
  homePlanet: 'Earth',
  color: 'silver'
};
spaceship.homePlanet; // Returns 'Earth',
spaceship.color; // Returns 'silver',


Se tentarmos acessar uma propriedade que não existe naquele objeto, undefinedserá retornado.

spaceship.favoriteIcecream; // Returns undefined

Vamos praticar mais um pouco usando a notação de ponto em um objeto!

Instruções
Checkpoint 1 Passed
1 .
Vamos usar o operador ponto para acessar o valor de numCrewdo spaceshipobjeto no editor de código. Crie uma variável crewCounte atribua a propriedade spaceship's numCrewa ela.

Ponto de verificação 2 aprovado
2 .
Novamente usando o operador ponto, crie uma variável planetArraye atribua a propriedade spaceship's flightPatha ela.