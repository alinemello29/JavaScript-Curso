OBJETOS AVANÇADOS
Levantadores
14 minutos
Junto com métodos getter , também podemos criar métodos setter que reatribuem valores de propriedades existentes dentro de um objeto. Vamos ver um exemplo de um método setter:

const person = {
  _age: 37,
  set age(newAge){
    if (typeof newAge === 'number'){
      this._age = newAge;
    } else {
      console.log('You must assign a number to age');
    }
  }
};

Observe que no exemplo acima:

Podemos verificar qual valor está sendo atribuído a this._age.
Quando usamos o método setter, apenas valores que são números serão reatribuídosthis._age
Há diferentes saídas dependendo de quais valores são usados ​​para reatribuir this._age.
Então use o método setter:

person.age = 40;
console.log(person._age); // Logs: 40
person.age = '40'; // Logs: You must assign a number to age

Métodos setter como agenão precisam ser chamados com um conjunto de parênteses. Sintaticamente, parece que estamos reatribuindo o valor de uma propriedade.

Assim como os métodos getter, há vantagens semelhantes em usar métodos setter que incluem verificar a entrada, executar ações em propriedades e exibir uma intenção clara de como o objeto deve ser usado. No entanto, mesmo com um método setter, ainda é possível reatribuir propriedades diretamente. Por exemplo, no exemplo acima, ainda podemos definir ._agediretamente:

person._age = 'forty-five'
console.log(person._age); // Prints forty-five

Instruções
Checkpoint 1 Passed
1 .
Atualmente, robothá um método getter para, numOfSensorsmas nenhum método setter! E se precisarmos adicionar ou remover alguns sensores? Vamos consertar esse problema.

Adicione um método setter nomeado numOfSensorsusando a setpalavra-chave. Forneça um parâmetro de num. Deixe o corpo da função vazio por enquanto.

Ponto de verificação 2 aprovado
2 .
Há algumas coisas que devemos fazer no método setter:

Adicione uma verificação para ver se numé um número usando o typeofoperador.
numtambém deve ser maior ou igual a 0.
Se ambas as condições forem atendidas, reatribua this._numOfSensorspara num.
Ponto de verificação 3 aprovado
3 .
Agora adicione um elseque registre 'Pass in a number that is greater than or equal to 0'no console.

Ponto de verificação 4 aprovado
4 .
Use o numOfSensorsmétodo setter robotpara atribuir _numOfSensorsa 100.

Ponto de verificação 5 aprovado
5 .
Para verificar se o método setter funcionou, console.log() robot.numOfSensors.