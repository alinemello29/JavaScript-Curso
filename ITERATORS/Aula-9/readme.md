ITERADORES
Análise
<1 minuto
Ótimo trabalho ao limpar a lição sobre iteradores ! Você aprendeu vários métodos úteis nesta lição, bem como como usar a documentação JavaScript da Mozilla Developer Network para descobrir e entender métodos adicionais. Vamos revisar!

.forEach()é usado para executar o mesmo código em todos os elementos de uma matriz, mas não altera a matriz e retorna undefined.
.map()executa o mesmo código em cada elemento de uma matriz e retorna uma nova matriz com os elementos atualizados.
.filter()verifica cada elemento em uma matriz para ver se ele atende a determinados critérios e retorna uma nova matriz com os elementos que retornam verdadeiros para os critérios.
.findIndex()retorna o índice do primeiro elemento de um array que satisfaz uma condição na função de retorno de chamada. Ele retorna -1se nenhum dos elementos no array satisfaz a condição.
.reduce()itera por uma matriz, pega os valores dos elementos e retorna um único valor.
Todos os métodos iteradores recebem uma função de retorno de chamada, que pode ser uma função predefinida, uma expressão de função ou uma função de seta.
Você pode visitar a Mozilla Developer Network para saber mais sobre métodos iteradores (e todas as outras partes do JavaScript!).
Instruções
Se você quer se desafiar:

Defina uma função de retorno de chamada antes de usá-la em um iterador.
Encadeie dois métodos de iteração no mesmo array.
Use os argumentos opcionais em um iterador para incluir o índice ou o array inteiro. (Confira a página de métodos de iteração de array do MDN para mais informações)
Use .reduce()para pegar uma matriz de várias camadas e retornar uma matriz de camada única do zero.