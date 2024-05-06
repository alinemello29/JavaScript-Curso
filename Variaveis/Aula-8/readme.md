VARIÁVEIS
Interpolação de strings

Na versão ES6 do JavaScript, podemos inserir ou interpolar variáveis ​​em strings usando literais de modelo . Confira o exemplo a seguir, onde um modelo literal é usado para registrar strings juntas:

const myPet = 'armadillo';
console.log(`I own a pet ${myPet}.`);
// Output: I own a pet armadillo.

Notar que:

um literal de modelo é envolvido por crases `(essa tecla geralmente está localizada na parte superior do teclado, à esquerda da 1tecla).
Dentro do literal do modelo, você verá um espaço reservado, ${myPet}. O valor de myPeté inserido no literal do modelo.
Quando interpolamos `I own a pet ${myPet}.`, a saída que imprimimos é a string:'I own a pet armadillo.'
Um dos maiores benefícios de usar literais de modelo é a legibilidade do código. Usando literais de modelo, você pode saber mais facilmente qual será a nova string. Você também não precisa se preocupar em escapar de aspas duplas ou simples.

Instruções
Ponto de verificação 1 Envio
1 .
Crie uma variável chamada myNamee atribua seu nome a ela.

Ponto de verificação 2 aprovado
2 .
Crie uma variável chamada myCitye atribua a ela o nome da sua cidade favorita.

Ponto de verificação 3 aprovado
3 .
Use um único modelo literal para interpolar suas variáveis ​​na frase abaixo. Use console.log()para imprimir sua frase no console no seguinte formato:

My name is NAME. My favorite city is CITY.

Substitua NAMEe CITYna string acima interpolando os valores salvos em myNamee myCity.