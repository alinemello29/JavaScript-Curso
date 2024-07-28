Muitas vezes não temos consciência do número de suposições que fazemos quando nos comunicamos em nossas línguas nativas. Se disséssemos para você “contar até três”, esperaríamos que você dissesse os números “um”, “dois” e “três”. Presumimos que você saberia começar com “um” e terminar com “três”. Com a programação, precisamos ser mais explícitos com nossas instruções para o computador. Veja como podemos dizer ao computador para “contar até três”:

for (let i = 1; i <= 3; i++) {
  console.log(i);
}

Quando falamos com outros humanos, compartilhamos um vocabulário que fornece maneiras rápidas de comunicar conceitos complicados. Quando dizemos a palavra “assar”, ela nos lembra de uma subrotina familiar — pré-aquecer um forno, colocar algo em um forno por um determinado período de tempo e, finalmente, removê-lo. Isso nos permite abstrair muitos detalhes e comunicar conceitos-chave de forma mais concisa. Em vez de listar todos esses detalhes, podemos dizer: “Nós assamos um bolo” e ainda transmitir todo esse significado a você.

Nesta lição, aprenderemos como usar “abstração” na programação escrevendo funções . Além de nos permitir reutilizar nosso código, as funções ajudam a criar programas claros e legíveis. Se você encontrar countToThree()em um programa, poderá adivinhar rapidamente o que a função faz sem ter que parar e ler o corpo da função.

Também aprenderemos sobre uma maneira de adicionar outro nível de abstração à nossa programação: funções de ordem superior . Funções de ordem superior são funções que aceitam outras funções como argumentos e/ou retornam funções como saída. Isso nos permite construir abstrações sobre outras abstrações, assim como “Nós organizamos uma festa de aniversário” é uma abstração que pode ser construída sobre a abstração “Nós fizemos um bolo”.