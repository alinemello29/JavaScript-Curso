INTRODUÇÃO AO JAVASCRIPT
Objetos integrados

Além disso console, existem outros objetos incorporados ao JavaScript . No futuro, você construirá seus próprios objetos , mas por enquanto esses objetos “integrados” estão cheios de funcionalidades úteis.

Por exemplo, se você quiser realizar operações matemáticas mais complexas do que aritméticas, o JavaScript possui o objeto integrado Math.

O melhor dos objetos é que eles possuem métodos! Vamos chamar o .random()método do objeto integrado Math:

console.log(Math.random()); // Prints a random number between 0 and 1

No exemplo acima, chamamos o .random()método anexando o nome do objeto com o operador ponto, o nome do método e os parênteses de abertura e fechamento. Este método retorna um número aleatório entre 0 (inclusivo) e 1 (exclusivo).

Para gerar um número aleatório entre 0 e 50, poderíamos multiplicar esse resultado por 50, assim:

Math.random() * 50;

O exemplo acima provavelmente será avaliado como decimal. Para garantir que a resposta seja um número inteiro, podemos aproveitar outro Mathmétodo útil chamado Math.floor().

Math.floor()pega um número decimal e arredonda para o número inteiro mais próximo. Você pode usar Math.floor()para arredondar um número aleatório como este:

Math.floor(Math.random() * 50);

Nesse caso:

Math.random()gera um número aleatório entre 0 e 1.
Em seguida, multiplicamos esse número por 50, então agora temos um número entre 0 e 50.
Em seguida, Math.floor()arredonda o número para o número inteiro mais próximo.
Se você quisesse ver o número impresso no terminal, ainda precisaria usar uma console.log()instrução:

console.log(Math.floor(Math.random() * 50)); // Prints a random whole number between 0 and 50

Para ver todas as propriedades e métodos do Mathobjeto, dê uma olhada na documentação aqui .

Instruções
Ponto de verificação 1 Envio
1 .
Dentro de a console.log(), crie um número aleatório com Math.random()e multiplique-o por 100.


Preso? Obtenha uma dica
Ponto de verificação 2 aprovado
2 .
Agora, use Math.floor()para tornar a saída um número inteiro.

Dentro do que console.log()você escreveu na última etapa, coloque o Math.random() * 100código existente entre parênteses Math.floor().


Preso? Obtenha uma dica
Ponto de verificação 3 aprovado
3 .
Encontre um método no objeto JavaScriptMath que retorne o menor número inteiro maior ou igual a um número decimal.

Use este método com o número 43.8. Registre a resposta no console.


Preso? Obtenha uma dica
Ponto de verificação 4 aprovado
4 .
Use a documentação do JavaScript para encontrar um método no objeto integrado Numberque verifique se um número é um número inteiro.

Coloque o número 2017entre parênteses do método e use console.log()para imprimir o resultado.