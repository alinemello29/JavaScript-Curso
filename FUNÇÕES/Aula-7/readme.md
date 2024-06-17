Funções auxiliares

Também podemos usar o valor de retorno de uma função dentro de outra função. Essas funções chamadas dentro de outra função são frequentemente chamadas de funções auxiliares . Como cada função executa uma tarefa específica, nosso código fica mais fácil de ler e depurar, se necessário.

Se quiséssemos definir uma função que converta a temperatura de Celsius para Fahrenheit, poderíamos escrever duas funções como:

function multiplyByNineFifths(number) {
  return number * (9/5);
};

function getFahrenheit(celsius) {
  return multiplyByNineFifths(celsius) + 32;
};

getFahrenheit(15); // Returns 59

No exemplo acima:

getFahrenheit()é chamado e 15passado como um argumento.
O bloco de código dentro de getFahrenheit()chama multiplyByNineFifths()e passa 15como argumento.
multiplyByNineFifths()leva o argumento de 15para o numberparâmetro.
O bloco de código dentro da multiplyByNineFifths()função multiplica 15por (9/5), que é avaliado como 27.
27é retornado para a chamada de função em getFahrenheit().
getFahrenheit()continua a ser executado. Ele adiciona 32a 27, que é avaliado como 59.
Finalmente, 59é retornado para a chamada de função getFahrenheit(15).
Podemos usar funções para separar pequenos pedaços de lógica ou tarefas e usá-las quando necessário. Escrever funções auxiliares pode ajudar a realizar tarefas grandes e difíceis e dividi-las em tarefas menores e mais gerenciáveis.

Instruções
Checkpoint 1 Passed
1 .
No exercício anterior, criamos uma função para encontrar a quantidade de monitores necessários para um escritório. Agora vamos escrever outra função que usa a monitorCountfunção para descobrir o preço.

Abaixo, monitorCountcrie uma declaração de função chamada costOfMonitorsque tenha dois parâmetros, o primeiro parâmetro é rowse o segundo parâmetro é columns. Deixe o corpo da função vazio por enquanto.

Ponto de verificação 2 aprovado
2 .
É hora de adicionar algum código ao corpo da função costOfMonitorspara calcular o custo total.

Adicione uma returninstrução que retorne o valor da chamada monitorCount(rows, columns)multiplicado por 200.

Ponto de verificação 3 aprovado
3 .
Devemos economizar o custo em uma variável.

Declare uma variável nomeada totalCostusando a constpalavra-chave. Atribua ao totalCostvalor da chamada costOfMonitors()com os argumentos 5e 4respectivamente.

Ponto de verificação 4 aprovado
4 .
Para verificar se a função funcionou corretamente, faça login totalCostno console.