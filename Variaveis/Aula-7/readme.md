VARIÁVEIS
Concatenação de Strings com Variáveis

Nos exercícios anteriores, atribuímos strings às variáveis . Agora, vamos ver como conectar ou concatenar strings em variáveis.

O +operador pode ser usado para combinar dois valores de string mesmo se esses valores estiverem sendo armazenados em variáveis:

let myPet = 'armadillo';
console.log('I own a pet ' + myPet + '.'); 
// Output: 'I own a pet armadillo.'

No exemplo acima, atribuímos o valor 'armadillo'à myPetvariável. Na segunda linha, o +operador é usado para combinar três strings: 'I own a pet', o valor salvo em myPet, e '.'. Registramos o resultado dessa concatenação no console como:

I own a pet armadillo.

Instruções
Ponto de verificação 1 Envio
1 .
Crie uma variável chamada favoriteAnimale defina-a igual ao seu animal favorito.

Ponto de verificação 2 aprovado
2 .
Use console.log()para imprimir 'My favorite animal: ANIMAL'no console. Use a concatenação de strings para que ela ANIMALseja substituída pelo valor em sua favoriteAnimalvariável.