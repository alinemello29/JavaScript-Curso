FUNÇÕES DE ORDEM SUPERIOR
Funções como Dados

As funções JavaScript se comportam como qualquer outro tipo de dado na linguagem; podemos atribuir funções a variáveis ​​e reatribuí-las a novas variáveis.

Abaixo, temos um nome de função irritantemente longo que prejudica a legibilidade de qualquer código em que é usado. Nota: Se a sintaxe da função abaixo parecer estranha, reveja o exercício de funções de seta para atualizar seu conhecimento sobre a notação de seta do ES6.

const announceThatIAmDoingImportantWork = () => {
    console.log("I’m doing very important work!");
};

Vamos fingir que essa função faz um trabalho importante e precisa ser chamada repetidamente. Para renomear essa função sem sacrificar o código-fonte, podemos reatribuir a função a uma variável com um nome curto adequado:

const busy = announceThatIAmDoingImportantWork;

busy(); // This function call barely takes any space!

busyé uma variável que contém uma referência à nossa função original. Se pudéssemos procurar o endereço na memória de busye o endereço na memória de announceThatIAmDoingImportantWorkeles apontariam para o mesmo lugar. Nossa nova busy()função pode ser invocada com parênteses como se esse fosse o nome que originalmente demos à nossa função.

Observe como atribuímos announceThatIAmDoingImportantWorksem parênteses como o valor para a busyvariável. Queremos atribuir o valor da função em si, não o valor que ela retorna quando invocada.

Em JavaScript, funções são objetos de primeira classe . Isso significa que, como outros objetos que você encontrou, funções JavaScript podem ter propriedades e métodos .

Como funções são um tipo de objeto, elas têm propriedades como .lengthe .name, e métodos como .toString(). Você pode ver mais sobre os métodos e propriedades de funções na documentação .

Funções são especiais porque podemos invocá-las, mas ainda podemos tratá-las como qualquer outro tipo de dado. Vamos praticar um pouco fazendo isso!

Instruções
Checkpoint 1 Passed
1 .
Definimos uma função com um nome muito longo: checkThatTwoPlusTwoEqualsFourAMillionTimes(). Essa função demora muito para ser executada. Ela verifica se 2 + 2 = 4, mas faz isso um milhão de vezes (só para ter certeza)!

Usando const, declare uma variável de nome mais curto, isTwoPlusTwoque será mais fácil de trabalhar. Atribua checkThatTwoPlusTwoEqualsFourAMillionTimescomo seu valor.

Ponto de verificação 2 aprovado
2 .
Invoque sua isTwoPlusTwo()função.

Ponto de verificação 3 aprovado
3 .
Hmmm, se esquecemos o nome original da nossa função. Existe uma maneira de descobrirmos?

Use isTwoPlusTwoa console.log()propriedade nameda função que atribuímos a isTwoPlusTwo.