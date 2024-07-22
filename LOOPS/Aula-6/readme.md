Loops aninhados

Quando temos um loop rodando dentro de outro loop, chamamos isso de nested loop . Um uso para um nested forloop é comparar os elementos em dois arrays . Para cada rodada do forloop externo, o loop interno forrodará completamente.

Vejamos um exemplo de um forloop aninhado:

const myArray = [6, 19, 20];
const yourArray = [19, 81, 2];
for (let i = 0; i < myArray.length; i++) {
  for (let j = 0; j < yourArray.length; j++) {
    if (myArray[i] === yourArray[j]) {
      console.log('Both arrays have the number: ' + yourArray[j]);
    }
  }
}

Vamos pensar sobre o que está acontecendo no loop aninhado em nosso exemplo. Para cada elemento no array de loop externo, myArray, o loop interno será executado em sua totalidade comparando o elemento atual do array externo, myArray[i], a cada elemento no array interno, yourArray[j]. Quando ele encontra uma correspondência, ele imprime uma string no console.

Agora é sua vez de escrever um loop aninhado!

Observação: para sair de um loop infinito em um exercício, atualize a página e corrija o código do(s) seu(s) loop(s).

Instruções
Checkpoint 1 Passed
1 .
Imagine que você é um programador figurão para uma plataforma de mídia social! Você foi encarregado de construir um protótipo para um programa de seguidores mútuos. Você precisará de dois arrays de “amigos” de dois usuários simulados para que possa extrair os nomes dos seguidores que existem em ambas as listas. Crie uma variável chamada bobsFollowerse defina-a como igual a um array com quatro strings representando os nomes dos amigos de Bob.

Ponto de verificação 2 aprovado
2 .
Crie uma variável chamada tinasFollowerse defina-a como igual a um array com três strings representando os nomes dos amigos de Tina. Faça exatamente dois deles iguais a dois dos amigos no bobsFollowersarray.

Ponto de verificação 3 aprovado
3 .
Crie uma terceira variável chamada mutualFollowerse defina-a como uma matriz vazia.

Ponto de verificação 4 aprovado
4 .
Crie um loop aninhado que itere bobsFollowerscomo o array para o loop externo e tinasFollowerscomo o array para o loop interno. Se o elemento atual do loop externo for o mesmo que o elemento atual do loop interno, empurre esse elemento para o mutualFollowersarray