OBJETOS AVANÇADOS
Pegadores
15 minutos
Getters são métodos que obtêm e retornam as propriedades internas de um objeto. Mas eles podem fazer mais do que apenas recuperar o valor de uma propriedade! Vamos dar uma olhada em um método getter:

const person = {
  _firstName: 'John',
  _lastName: 'Doe',
  get fullName() {
    if (this._firstName && this._lastName){
      return `${this._firstName} ${this._lastName}`;
    } else {
      return 'Missing a first name or a last name.';
    }
  }
}

// To call the getter method: 
person.fullName; // 'John Doe'

Observe que no método getter acima:

Usamos a getpalavra-chave seguida de uma função.
Usamos uma if...elsecondicional para verificar se ambos _firstNamee _lastNameexistem (garantindo que ambos retornem valores verdadeiros) e então retornamos um valor diferente dependendo do resultado.
Podemos acessar as propriedades internas do objeto de chamada usando this. Em fullName, estamos acessando ambos this._firstNamee this._lastName.
Na última linha, chamamos fullName. personEm geral, métodos getter não precisam ser chamados com um conjunto de parênteses. Sintaticamente, parece que estamos acessando uma propriedade.
Agora que vimos a sintaxe, vamos discutir algumas vantagens notáveis ​​de usar métodos getter:

Os getters podem executar uma ação nos dados ao obter uma propriedade.
Getters podem retornar valores diferentes usando condicionais .
Em um getter, podemos acessar as propriedades do objeto de chamada usando this.
A funcionalidade do nosso código é mais fácil de entender para outros desenvolvedores.
Outra coisa a ter em mente ao usar métodos getter (e setter) é que as propriedades não podem compartilhar o mesmo nome que a função getter/setter. Se fizermos isso, chamar o método resultará em um erro de pilha de chamadas infinitas. Uma solução alternativa é adicionar um sublinhado antes do nome da propriedade, como fizemos no exemplo acima.

Ótimo, vamos lá!

Instruções
Checkpoint 1 Passed
1 .
Em robot, crie um método getter nomeado energyLevelusando a getpalavra-chave. Deixe o corpo da função em branco por enquanto.

Ponto de verificação 2 aprovado
2 .
Dentro do método getter, adicione uma ifinstrução para verificar se this._energyLevelé um número usando o typeofoperador. Se essa condição for verdadeira, retorne 'My current energy level is ENERGYLEVEL'. Substitua ENERGYLEVELpelo valor de this._energyLevel.

Certifique-se de retornar a string em vez de registrá-la no console.

Ponto de verificação 3 aprovado
3 .
Se this._energyLevelnão for um número, pode ser que a _energyLevelpropriedade tenha sido alterada. Vamos adicionar uma declaração de retorno padrão para quando tal cenário surgir.

Adicione uma elseinstrução que retorne 'System malfunction: cannot retrieve energy level'.

Ponto de verificação 4 aprovado
4 .
Registre o resultado da chamada do método getter energyLevelno robotconsole.

Observe que o método retornará uma resposta formatada em vez de apenas acessar uma propriedade!