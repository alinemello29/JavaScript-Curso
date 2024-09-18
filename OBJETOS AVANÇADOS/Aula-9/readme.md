OBJETOS AVANÇADOS
Atribuição Desestruturada
6 minutos
Frequentemente queremos extrair pares de chave-valor de objetos e salvá-los como variáveis . Tome como exemplo o seguinte objeto:

const vampire = {
  name: 'Dracula',
  residence: 'Transylvania',
  preferences: {
    day: 'stay inside',
    night: 'satisfy appetite'
  }
};

Se quiséssemos extrair a residencepropriedade como uma variável, poderíamos usar o seguinte código:

const residence = vampire.residence; 
console.log(residence); // Prints 'Transylvania' 

No entanto, também podemos tirar vantagem de uma técnica de desestruturação chamada atribuição desestruturada para economizar alguns toques de tecla. Na atribuição desestruturada, criamos uma variável com o nome da chave de um objeto que é envolvida por chaves { }e atribuímos a ela o objeto. Dê uma olhada no exemplo abaixo:

const { residence } = vampire; 
console.log(residence); // Prints 'Transylvania'

Olhe novamente para as vampirepropriedades do objeto no primeiro exemplo de código. Então, no exemplo acima, declaramos uma nova variável residenceque extrai o valor da residencepropriedade de vampire. Quando registramos o valor de residenceno console, 'Transylvania'é impresso.

Podemos até usar atribuição desestruturada para obter propriedades aninhadas de um objeto:

const { day } = vampire.preferences; 
console.log(day); // Prints 'stay inside'

Instruções
Checkpoint 1 Passed
1 .
Use a atribuição desestruturada para criar uma constvariável functionalitychamada functionality.robot

Se precisar de um lembrete sobre como usar a tarefa desestruturada, revise o exemplo na narrativa ou verifique a dica.

Ponto de verificação 2 aprovado
2 .
Como functionalityé uma referência, robot.functionalitypodemos chamar os métodos disponíveis robot.functionalitysimplesmente por meio de functionality.

Aproveite este atalho e chame o .beep()método em functionality.