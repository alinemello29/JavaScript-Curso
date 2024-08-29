OBJETOS
Criando Literais de Objetos
6 minutos
Objetos podem ser atribuídos a variáveis ​​como qualquer tipo JavaScript. Usamos chaves, {}, para designar um literal de objeto :

let spaceship = {}; // spaceship is an empty object

Preenchemos um objeto com dados não ordenados. Esses dados são organizados em pares chave-valor . Uma chave é como um nome de variável que aponta para um local na memória que contém um valor.


O valor de uma chave pode ser de qualquer tipo de dado na linguagem, incluindo funções ou outros objetos.

Criamos um par chave-valor escrevendo o nome da chave, ou identificador , seguido por dois pontos e então o valor. Separamos cada par chave-valor em um literal de objeto com uma vírgula ( ,). Chaves são strings, mas quando temos uma chave que não tem nenhum caractere especial, JavaScript nos permite omitir as aspas:


// An object literal with two key-value pairs
let spaceship = {
  'Fuel Type': 'diesel',
  color: 'silver'
};

O spaceshipobjeto tem duas propriedades Fuel Typee color. 'Fuel Type'tem aspas porque contém um caractere de espaço.

Vamos fazer alguns objetos!

Instruções
Checkpoint 1 Passed
1 .
O que spaceshiptemos até agora parece bom, mas, infelizmente, não é muito rápido em viagens hiperespaciais devido a ter uma fonte de combustível inferior. Crie um novo objeto de nave espacial nomeado fasterShipcom o mesmo colorque spaceshipmas com um Fuel Typeigual a 'Turbo Fuel'.