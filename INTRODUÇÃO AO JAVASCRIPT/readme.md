Introdução ao JavaScript
JavaScript é uma linguagem de programação amplamente utilizada para o desenvolvimento web. Com ele, você pode criar páginas web interativas, adicionar animações, manipular o DOM (Document Object Model) e muito mais. JavaScript é executado no navegador, o que significa que você pode ver os resultados de seu código instantaneamente.

O Que é JavaScript?
JavaScript é uma linguagem de programação interpretada, leve e orientada a objetos. Foi inicialmente desenvolvida por Brendan Eich na Netscape como uma maneira de adicionar scripts às páginas web. Hoje, é uma das três principais tecnologias da web, junto com HTML e CSS.

Primeiro Exemplo de JavaScript
Vamos começar com um simples exemplo de código JavaScript. Este exemplo exibirá uma mensagem "Hello, World!" na tela do navegador.

Exemplo:
html
Copiar código
<!DOCTYPE html>
<html>
<head>
    <title>Meu Primeiro Script</title>
</head>
<body>
    <h1>Olá, Mundo!</h1>
    <script>
        document.write("Hello, World!");
    </script>
</body>
</html>
Explicação:
<script>: A tag <script> é usada para incluir código JavaScript no HTML.
document.write("Hello, World!");: Este comando escreve "Hello, World!" diretamente no documento HTML.
Fundamentos do JavaScript
Variáveis
Em JavaScript, você pode armazenar dados em variáveis. Existem três maneiras principais de declarar variáveis:

var: Declarar uma variável que tem escopo de função.
let: Declarar uma variável com escopo de bloco.
const: Declarar uma variável cujo valor não pode ser alterado.
javascript
Copiar código
var nome = "Aline";
let idade = 25;
const cidade = "São Paulo";
Tipos de Dados
JavaScript possui vários tipos de dados, incluindo:

String (cadeia de caracteres): "Hello"
Number (número): 42, 3.14
Boolean (booleano): true, false
Array (vetor): [1, 2, 3]
Object (objeto): { nome: "Aline", idade: 25 }
Operadores
JavaScript suporta diversos operadores para realizar operações com variáveis e valores:

Aritméticos: +, -, *, /, %
Comparação: ==, ===, !=, !==, >, <, >=, <=
Lógicos: &&, ||, !
Funções
Funções são blocos de código reutilizáveis que executam uma tarefa específica. Você pode definir uma função e chamá-la quando necessário.

javascript
Copiar código
function saudacao(nome) {
    return "Olá, " + nome + "!";
}

console.log(saudacao("Aline"));
Manipulação do DOM
Uma das principais utilizações do JavaScript é a manipulação do DOM, permitindo que você altere dinamicamente o conteúdo e o estilo da página web.

javascript
Copiar código
document.getElementById("meuElemento").innerHTML = "Texto atualizado!";
Conclusão
JavaScript é uma linguagem poderosa que adiciona interatividade e dinamismo às páginas web. Com os conceitos básicos apresentados aqui, você pode começar a explorar e criar seus próprios scripts para melhorar suas habilidades e projetos web.
