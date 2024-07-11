MATRIZES
Mais métodos de matriz

Existem muito mais métodos de array do que apenas .push()and .pop(). Você pode ler sobre esses métodos de array na entrada do Documentos para JavaScript Arrays .

.pop()e .push()mutar o array no qual eles são chamados. No entanto, há momentos em que não queremos mutar o array original e podemos usar métodos de array não mutantes. Certifique-se de verificar a Docs para entender o comportamento do método que você está usando.

Alguns métodos de arrays disponíveis para desenvolvedores JavaScript incluem: .join(), .slice(), .splice(), .shift(), .unshift()e .concat()entre muitos outros. O uso desses métodos integrados facilita a execução de algumas tarefas comuns ao trabalhar com arrays.

Abaixo, exploraremos alguns métodos que ainda não aprendemos. Usaremos esses métodos para editar uma lista de compras. Conforme você conclui as etapas, pode consultar o Codecademy Docs para saber o que cada método faz!

Instruções
Ponto de verificação 1 aprovado
1 .
Use o .shift()método para remover o primeiro item do array groceryList.

Registre o novo groceryListno console.

Leia sobre isso .shift()em Documentos .

Ponto de verificação 2 aprovado
2 .
No código adicionado na etapa 1, use o .unshift()método para adicionar 'popcorn'ao início da sua lista de compras.

Depois de ligar .unshift(), groceryListfaça login groceryListno console.

Talvez você queira excluir a console.log()declaração da etapa anterior.

Leia sobre isso .unshift()em Documentos .

Ponto de verificação 3 aprovado
3 .
Você está com pressa, então decide pedir a um amigo para ajudá-lo com suas compras de supermercado. Você quer que ele pegue o 'bananas', 'coffee beans', e 'brown rice'.

No código que você adicionou na etapa 2, use .slice()para fornecer ao seu amigo uma lista dessas três coisas.

Registre esta parte da lista no console. Ao contrário dos dois pontos de verificação anteriores, você deve executar essas duas etapas em uma linha.

Leia sobre isso .slice()em Documentos .

Ponto de verificação 4 aprovado
4 .
Depois de chamar .slice(), groceryListregistre a lista de compras no console mais uma vez.

Observe que o groceryListarray ainda contém os mesmos itens que tinha no Passo 2. Isso significa .slice()que não é mutante! Você pode confirmar isso no link do passo anterior.

Ponto de verificação 5 aprovado
5 .
Vamos encontrar o índice de um elemento específico groceryListusando .indexOf().

Chame .indexOf()para groceryListencontrar o índice do elemento 'pasta'e salvar o valor retornado em uma constvariável chamada pastaIndex.

Em seguida, faça login pastaIndexno console. (Você pode remover as outras console.log()instruções para organizar o terminal.)

Leia sobre isso .indexOf()em Documentos