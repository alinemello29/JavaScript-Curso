DECLARAÇÕES CONDICIONAIS
Tarefa Verdadeira e Falsa

Avaliações verdadeiras e falsas abrem um mundo de possibilidades taquigráficas!

Digamos que você tenha um site e queira usar o nome de usuário de um usuário para fazer uma saudação personalizada. Às vezes, o usuário não possui conta, tornando a usernamevariável falsa. O código abaixo verifica se usernameestá definido e atribui uma string padrão caso não esteja:

let username = '';
let defaultName;

if (username) {
  defaultName = username;
} else {
  defaultName = 'Stranger';
}

console.log(defaultName); // Prints: Stranger

Se você combinar seu conhecimento de operadores lógicos , poderá usar uma abreviação para o código acima. Em uma condição booleana, o JavaScript atribui o valor verdadeiro a uma variável se você usar o ||operador em sua atribuição:

let username = '';
let defaultName = username || 'Stranger';

console.log(defaultName); // Prints: Stranger

Como as instruções|| or verificam primeiro a condição do lado esquerdo, será atribuído à variável o valor real de se for verdadeira e será atribuído o valor de se for falsa. Este conceito também é conhecido como avaliação de curto-circuito .defaultNameusername'Stranger'username

Instruções
Checkpoint 1 Passed
1 .
Vamos usar a avaliação de curto-circuito para atribuir um valor a writingUtensil. Não edite toolainda, retornaremos toolna próxima etapa.

Atribua ao writingUtensilvalor de toole se toolfor falso, atribua um valor padrão de 'pen'.

Ponto de verificação 2 aprovado
2 .
Observe o texto 'The pen is mightier than the sword'registrado no console. O que significa que o valor de writingUtensilé 'pen'.

E se reatribuíssemos o valor de toolto 'marker'. Vamos ver o que acontece com o valor de writingUtensil.