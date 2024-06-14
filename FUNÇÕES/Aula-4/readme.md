Parâmetros e argumentos

Até agora, as funções que criamos executam uma tarefa sem entrada. No entanto, algumas funções podem receber entradas e usá-las para executar uma tarefa. Ao declarar uma função, podemos especificar seus parâmetros . Os parâmetros permitem que as funções aceitem entradas e executem uma tarefa usando as entradas. Usamos parâmetros como espaços reservados para informações que serão passadas para a função quando ela for chamada.

Vamos observar como especificar parâmetros em nossa declaração de função:

Sintaxe JavaScript para declarar uma função com parâmetros
No diagrama acima, calculateArea()calcula a área de um retângulo, com base em duas entradas, widthe height. Os parâmetros são especificados entre parênteses como widthe heighte dentro do corpo da função, eles agem como variáveis ​​regulares. widthe heightatuam como espaços reservados para valores que serão multiplicados juntos.

Ao chamar uma função que possui parâmetros, especificamos os valores entre parênteses que seguem o nome da função. Os valores que são passados ​​para a função quando ela é chamada são chamados de argumentos . Os argumentos podem ser passados ​​para a função como valores ou variáveis.

Sintaxe JavaScript para invocar uma função com argumentos como valores
Na chamada de função acima, o número 10é passado como widthe 6é passado como height. Observe que a ordem na qual os argumentos são passados ​​e atribuídos segue a ordem em que os parâmetros são declarados.

Sintaxe JavaScript para invocar uma função com argumentos como variáveis
As variáveis rectWidth​​e rectHeightsão inicializadas com os valores de altura e largura de um retângulo antes de serem usadas na chamada de função.

Ao usar parâmetros, calculateArea()pode ser reutilizado para calcular a área de qualquer retângulo! Funções são uma ferramenta poderosa em programação de computadores, então vamos praticar a criação e chamada de funções com parâmetros.

Instruções
Checkpoint 1 Passed
1 .
A sayThanks()função funciona bem, mas vamos adicionar o nome do cliente na mensagem.

Adicione um parâmetro chamado nameà declaração da função para sayThanks().

Ponto de verificação 2 aprovado
2 .
Com namecomo parâmetro, pode ser usado como uma variável no corpo da função de sayThanks().

Usando namea concatenação de strings, altere a mensagem de agradecimento para o seguinte:

'Thank you for your purchase '+ name + '! We appreciate your business.'

Copie e cole a mensagem acima em seu código.

Ponto de verificação 3 aprovado
3 .
Um cliente chamado Cole acabou de comprar algo em sua loja online. Ligue sayThanks()e passe 'Cole'como argumento para enviar a Cole uma mensagem de agradecimento personalizada.