OBJETOS AVANÇADOS
A palavra-chave this
12 minutos
Objetos são coleções de dados e funcionalidades relacionadas. Armazenamos essa funcionalidade em métodos em nossos objetos:

const goat = {
  dietType: 'herbivore',
  makeSound() {
    console.log('baaa');
  }
};

Em nosso goatobjeto temos um .makeSound()método. Podemos invocar o .makeSound()método em goat.

goat.makeSound(); // Prints baaa

Legal, temos um goatobjeto que pode imprimir baaano console. Tudo parece estar funcionando bem. E se quiséssemos adicionar um novo método ao nosso goatobjeto chamado .diet()que imprima o goat's dietType?

const goat = {
  dietType: 'herbivore',
  makeSound() {
    console.log('baaa');
  },
  diet() {
    console.log(dietType);
  }
};
goat.diet(); 
// Output will be "ReferenceError: dietType is not defined"

Isso é estranho, por que dietTypenão é definido mesmo sendo uma propriedade de goat? Isso porque dentro do escopo do .diet()método, não temos acesso automático a outras propriedades do goatobjeto.

É aqui que a thispalavra-chave vem ao resgate. Se mudarmos o .diet()método para usar o this, .diet()funciona! :

const goat = {
  dietType: 'herbivore',
  makeSound() {
    console.log('baaa');
  },
  diet() {
    console.log(this.dietType);
  }
};

goat.diet(); 
// Output: herbivore

A thispalavra-chave faz referência ao objeto chamador que fornece acesso às propriedades do objeto chamador. No exemplo acima, o objeto chamador é goate usando thisestamos acessando o goatobjeto em si, e então a dietTypepropriedade de goatusando notação de ponto de propriedade.

Vamos nos familiarizar com o uso da thispalavra-chave em um método.

Instruções
Checkpoint 1 Passed
1 .
Vamos criar um novo objeto para praticar o uso de this.

Em main.js há um objeto robot, adicione uma propriedade de modele atribua a ele um valor de '1E78V2'. Adicione outra propriedade energyLevele atribua a ele um valor de 100.

Ponto de verificação 2 aprovado
2 .
Dentro do robotobjeto, adicione um método chamado provideInfo. Dentro do corpo de provideInfo(), retorne a seguinte string usando interpolação:

I am MODEL and my current energy level is ENERGYLEVEL.  

Substitua 'MODEL' e 'ENERGYLEVEL' pelas propriedades modele do objeto chamador energyLevel. Lembre-se, para obter acesso às propriedades do objeto chamador dentro de um método, você tem que usar a thispalavra-chave!

Ponto de verificação 3 aprovado
3 .
Agora para verificar .provideInfo()se tem acesso às propriedades internas de robot. Registre o resultado da chamada do .provideInfo()método robotno console.