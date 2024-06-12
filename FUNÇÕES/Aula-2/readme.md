Declarações de Função

Em JavaScript, existem muitas maneiras de criar uma função . Uma maneira de criar uma função é usando uma declaração de função . Assim como uma declaração de variável vincula um valor a um nome de variável, uma declaração de função vincula uma função a um nome ou identificador . Dê uma olhada na anatomia de uma declaração de função abaixo:

Uma declaração de função consiste em:

A functionpalavra-chave.
O nome da função, ou seu identificador, seguido de parênteses.
Um corpo de função, ou o bloco de instruções necessárias para executar uma tarefa específica, entre colchetes da função, { }.
Uma declaração de função é uma função vinculada a um identificador ou nome. No próximo exercício veremos como executar o código dentro do corpo da função.

Também devemos estar cientes do recurso de elevação em JavaScript, que permite acesso às declarações de funções antes de serem definidas.

Veja um exemplo de içamento:

greetWorld(); // Output: Hello, World!

function greetWorld() {
  console.log('Hello, World!');
}

Observe como hoisting pode greetWorld()ser chamado antes da greetWorld()função ser definida! Como o içamento não é considerado uma boa prática, queremos apenas que você esteja ciente desse recurso.

Se você quiser ler mais sobre içamento, verifique a documentação do MDN sobre içamento .

Instruções
Checkpoint 1 Passed

Vamos criar uma função que imprima um lembrete no console. Usando uma declaração de função, crie uma função chamada getReminder().

Ponto de verificação 2 aprovado

No corpo da função getReminder(), registre o seguinte lembrete no console:'Water the plants.'

Ponto de verificação 3 aprovado

Vamos criar outra função que imprima uma frase útil de viagem em espanhol no console.

Usando uma declaração de função, crie uma função chamada greetInSpanish().

Ponto de verificação 4 aprovado

Adicione código ao corpo da função de greetInSpanish():

No corpo da função console.log()a seguinte frase em espanhol para o console:'Buenas tardes.'