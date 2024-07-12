MATRIZES
Matrizes e Funções

Ao longo da lição, abordamos arrays sendo mutáveis, ou alteráveis. Bem, o que acontece se tentarmos alterar um array dentro de uma função? O array mantém a alteração após a chamada da função ou ela é delimitada para dentro da função?

Dê uma olhada no exemplo a seguir, onde chamamos .push()um array dentro de uma função. Lembre-se, o .push()método muta, ou altera, um array:

const flowers = ['peony', 'daffodil', 'marigold'];

function addFlower(arr) {
  arr.push('lily');
}

addFlower(flowers);

console.log(flowers); // Output: ['peony', 'daffodil', 'marigold', 'lily']

Vamos rever o que aconteceu no exemplo:

A flowersmatriz que tem 3 elementos.
A função addFlower()possui um parâmetro de arruso .push()para adicionar um 'lily'elemento arr.
Chamamos addFlower()com um argumento flowersque executará o código dentro dele addFlower.
Verificamos o valor de flowerse agora ele inclui o 'lily'elemento! O array foi mutado!
Então, quando você passa um array para uma função, se o array for mutado dentro da função, essa mudança será mantida fora da função também. Você também pode ver esse conceito explicado como passagem por referência, já que o que estamos realmente passando para a função é uma referência para onde a variável memory está armazenada e alterando a memória.

Instruções
Ponto de verificação 1 aprovado
1 .
Em main.js , existe um array concept. Existe também uma função changeArrque atribuirá o elemento no índice 3de um array a 'MUTATED'. A função changeArrfoi chamada com um argumento de concept.

Abaixo da chamada de função, acesse concepto console para verificar se essa reatribuição alterou a matriz.

Ponto de verificação 2 aprovado
2 .
Vamos verificar o que acontece se modificarmos um array usando um método integrado dentro de uma função.

Na console.log()instrução, defina outra função chamada removeElementque receba um parâmetro de newArr. Dentro do corpo da função, .pop()chame newArr.

Ponto de verificação 3 aprovado
3 .
Chamada removeElement()com um argumento de concept.

Ponto de verificação 4 aprovado
4 .
Depois de chamar removeElement(concept), verifique o valor conceptregistrando-o no console.

Observe que em ambos os casos, a alteração na matriz foi mantida fora da função!