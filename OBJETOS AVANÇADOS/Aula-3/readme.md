OBJETOS AVANÇADOS
Funções de seta e isto
6 minutos
Vimos no exercício anterior que para um método, o objeto de chamada é o objeto ao qual o método pertence. Se usarmos a thispalavra-chave em um método, então o valor de thisé o objeto de chamada. No entanto, fica um pouco mais complicado quando começamos a usar funções de seta para métodos . Dê uma olhada no exemplo abaixo:

const goat = {
  dietType: 'herbivore',
  makeSound() {
    console.log('baaa');
  },
  diet: () => {
    console.log(this.dietType);
  }
};

goat.diet(); // Prints undefined

No comentário, você pode ver que goat.diet()would log undefined. Então o que aconteceu? Observe que o .diet()método é definido usando uma arrow function.

As funções de seta inerentemente vinculam , ou amarram, um valor já definido thisà função em si que NÃO é o objeto de chamada. No trecho de código acima, o valor de thisé o objeto global , ou um objeto que existe no escopo global, que não tem uma dietTypepropriedade e, portanto, retorna undefined.

Para ler mais sobre as funções de seta ou o objeto global, confira a documentação do MDN sobre o objeto global e as funções de seta .

A principal lição do exemplo acima é evitar usar funções de seta ao usar thisem um método!

Instruções
Checkpoint 1 Passed
1 .
Atualmente, o .checkEnergy()método não está produzindo a saída correta porque está usando a sintaxe da função de seta.

Refatore, ou altere, o método para usar uma expressão de função. Você pode escrever a função usando o formato longo ou curto.

Após refatorar o método, observe que ele .checkEnergy()tem acesso às outras propriedades internas do robotobjeto.