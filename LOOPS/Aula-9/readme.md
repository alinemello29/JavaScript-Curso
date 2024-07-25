A palavra-chave break

Imagine que estamos querendo adotar um cachorro. Planejamos ir ao abrigo todos os dias por um ano e depois desistir. Mas e se encontrarmos o cachorro dos nossos sonhos no dia 65? Não queremos continuar indo ao abrigo pelos próximos 300 dias só porque nosso plano original era ir por um ano inteiro. Em nosso código, quando queremos impedir que um loop continue a ser executado mesmo que a condição de parada original que escrevemos para nosso loop não tenha sido atendida, podemos usar a palavra-chave break.

A breakpalavra-chave permite que os programas “saiam” do loop de dentro do bloco do loop.

Vamos verificar a sintaxe de uma breakpalavra-chave:

for (let i = 0; i < 99; i++) {
  if (i > 2 ) {
     break;
  }
  console.log('Banana.');
}

console.log('Orange you glad I broke out the loop!');

Esta é a saída do código acima:

Banana.
Banana.
Banana.
Orange you glad I broke out the loop!

break podem ser especialmente úteis quando estamos fazendo um loop por grandes estruturas de dados! Com breaks, podemos adicionar condições de teste além da condição de parada e sair do loop quando elas forem atendidas.

Instruções
Checkpoint 1 Passed
1 .
Registre cada elemento rapperArrayem um forloop com a variável iteradora i.

Ponto de verificação 2 aprovado
2 .
Após o forloop, registre a string "And if you don't know, now you know."no console. Nota: como há um caractere de aspas simples, ', em nossa string, podemos usar aspas duplas ao redor da string para garantir que o caractere seja impresso.

Ponto de verificação 3 aprovado
3 .
Adicione um breakbloco dentro do seu loop que sai do loop se o elemento no índice atual no rapperArrayfor 'Notorious B.I.G.'.
Registre o elemento antes de sair do loop.