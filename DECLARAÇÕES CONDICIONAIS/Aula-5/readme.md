DECLARAÇÕES CONDICIONAIS
Operadores lógicos

Trabalhar com condicionais significa que usaremos booleanos trueou falsevalores. Em JavaScript, existem operadores que trabalham com valores booleanos conhecidos como operadores lógicos . Podemos usar operadores lógicos para adicionar lógica mais sofisticada às nossas condicionais. Existem três operadores lógicos:

o operador e&& ( )
o operador ou ( ||)
o operador not , também conhecido como operador bang ( !)
Quando usamos o &&operador, estamos verificando se duas coisas são true:

if (stopLight === 'green' && pedestrians === 0) {
  console.log('Go!');
} else {
  console.log('Stop');
}

Ao usar o &&operador, ambas as condições devem ser avaliadas como truepara que toda a condição seja avaliada truee executada. Caso contrário, se qualquer uma das condições for false, a &&condição será avaliada como falsee o elsebloco será executado.

Se nos importamos apenas com o fato de qualquer uma das condições ser true, podemos usar o ||operador:

if (day === 'Saturday' || day === 'Sunday') {
  console.log('Enjoy the weekend!');
} else {
  console.log('Do some work.');
}

Ao usar o ||operador, apenas uma das condições deve ser avaliada como truepara que a instrução geral seja avaliada como true. No exemplo de código acima, se um day === 'Saturday'ou day === 'Sunday'for avaliado como truea ifcondição será avaliada como truee seu bloco de código será executado. Se a primeira condição em uma ||instrução for avaliada como true, a segunda condição nem mesmo será verificada. Somente se day === 'Saturday'for avaliado como falseserá day === 'Sunday'avaliado. O código na elseinstrução acima será executado somente se ambas as comparações forem avaliadas como false.

O ! operador not inverte ou nega o valor de um booleano:

let excited = true;
console.log(!excited); // Prints false

let sleepy = false;
console.log(!sleepy); // Prints true

Essencialmente, o !operador pegará um truevalor e transmitirá de volta falseou pegará um falsevalor e transmitirá de volta true.

Operadores lógicos são frequentemente usados ​​em instruções condicionais para adicionar outra camada de lógica ao nosso código.

Instruções
Checkpoint 1 Passed
1 .
Em main.js existem duas variáveis mood​​e tirednessLevel.

Vamos criar uma if...elseinstrução que verifique se moodé 'sleepy'e tirednessLevelé maior que 8.

Se ambas as condições forem avaliadas como true, então console.log()a string 'time to sleep'. Caso contrário, deveríamos console.log() 'not bed time yet'.

Depois de pressionar “Executar”, brinque com o ||operador e o !operador! O que acontece se você negar o valor de toda a instrução with !e mudar para ||em vez de &&?

