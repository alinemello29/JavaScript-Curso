ESCOPO
Escopo do bloco

O próximo contexto que abordaremos é o escopo do bloco . Quando uma variável é definida dentro de um bloco, ela só é acessível ao código entre chaves {}. Dizemos que a variável tem escopo de bloco porque só é acessível às linhas de código desse bloco.

Variáveis ​​declaradas com escopo de bloco são conhecidas como variáveis ​​locais porque estão disponíveis apenas para o código que faz parte do mesmo bloco.

O escopo do bloco funciona assim:

const logSkyColor = () => {
  let color = 'blue'; 
  console.log(color); // Prints "blue"
};

logSkyColor(); // Prints "blue"
console.log(color); // throws a ReferenceError

Você notará:

Definimos uma função logSkyColor().
Dentro da função, a colorvariável só está disponível entre chaves da função.
Se tentarmos registrar a mesma variável fora da função, ela lançará um ReferenceError.
Instruções
Checkpoint 1 Passed
1 .
Em main.js , defina uma função logVisibleLightWaves().

Ponto de verificação 2 aprovado
2 .
Dentro da logVisibleLightWaves()função, usando const, crie uma variável lightWavese defina-a igual a 'Moonlight'.

Ponto de verificação 3 aprovado
3 .
Dentro da logVisibleLightWaves()função, abaixo da lightWavesvariável, adicione uma console.log()instrução que registrará o valor da lightWavesvariável quando a função for executada.

Ponto de verificação 4 aprovado
4 .
Chame a logVisibleLightWaves()função de fora da função.

Ponto de verificação 5 aprovado
5 .
Abaixo da chamada de função, registre o valor de lightWavesno console de fora da função.

Você notará que ele registra a ReferenceErrorjá que a variável está vinculada ao escopo do bloco da função!