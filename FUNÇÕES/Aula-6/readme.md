Retornar

Quando uma função é chamada, o computador percorre o código da função e avalia o resultado. Por padrão, o valor resultante é undefined.

function rectangleArea(width, height) {
  let area = width * height;
}
console.log(rectangleArea(5, 7)) // Prints undefined

No exemplo de código, definimos nossa função para calcular o parâmetro areaae . Então é invocado com os argumentos e . Mas quando fomos imprimir os resultados obtivemos . Escrevemos nossa função errada? Não! Na verdade, a função funcionou bem e o computador calculou a área como , mas não a capturamos. Então, como podemos fazer isso? Com a palavra-chave !widthheightrectangleArea()57undefined35return

usando a palavra-chave return em uma função
Para retornar informações da chamada de função, usamos uma instrução return . Para criar uma instrução de retorno, usamos a returnpalavra-chave seguida do valor que desejamos retornar. Como vimos acima, se o valor for omitido, undefinedserá retornado.

Quando uma returninstrução é usada no corpo de uma função, a execução da função é interrompida e o código que a segue não será executado. Veja o exemplo abaixo:

function rectangleArea(width, height) {
  if (width < 0 || height < 0) {
    return 'You need positive integers to calculate area!';
  }
  return width * height;
}

Se um argumento para widthou heightfor menor que 0, então rectangleArea()retornará 'You need positive integers to calculate area!'. A segunda instrução return width * heightnão será executada.

A returnpalavra-chave é poderosa porque permite que funções produzam uma saída. Podemos então salvar a saída em uma variável para uso posterior.

Instruções
Checkpoint 1 Passed
1 .
Imagine se precisássemos solicitar monitores para todos em um escritório e esse escritório estivesse convenientemente organizado em formato de grade. Poderíamos usar uma função para nos ajudar a calcular o número de monitores necessários!

Declare uma função monitorCount()que possui dois parâmetros. O primeiro parâmetro é rowse o segundo parâmetro é columns.

Ponto de verificação 2 aprovado
2 .
Vamos calcular o número de monitores multiplicando rowse columnsretornando o valor.

No corpo da função que você acabou de escrever, use a returnpalavra-chave para retornar rows * columns.

Ponto de verificação 3 aprovado
3 .
Agora que a função está definida, podemos calcular o número de monitores necessários. Digamos que o escritório tenha 5 linhas e 4 colunas.

Declare uma variável nomeada numOfMonitorsusando a constpalavra-chave e atribua numOfMonitorso valor da invocação monitorCount()com os argumentos 5e 4.

Ponto de verificação 4 aprovado
4 .
Para verificar se a função funcionou corretamente, faça login numOfMonitorsno console.