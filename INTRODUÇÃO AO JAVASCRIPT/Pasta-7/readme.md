Métodos

Lembre-se de que métodos são ações que podemos realizar. Os tipos de dados têm acesso a métodos específicos que nos permitem lidar com instâncias desse tipo de dados. JavaScript fornece vários métodos de string.

Chamamos ou usamos esses métodos anexando uma instância com:

um ponto (o operador ponto)
o nome do método
abrindo e fechando parênteses
Por exemplo 'example string'.methodName().

Essa sintaxe parece um pouco familiar? Quando usamos console.log()estamos chamando o .log()método no consoleobjeto. Vamos ver console.log()alguns métodos de string reais em ação!

console.log('hello'.toUpperCase()); // Prints 'HELLO'
console.log('Hey'.startsWith('H')); // Prints true

Vejamos cada uma das linhas acima:

Na primeira linha, o .toUpperCase()método é chamado na string instance 'hello'. O resultado é registrado no console. Este método retorna uma string em letras maiúsculas: 'HELLO'.
Na segunda linha, o .startsWith()método é chamado na string instance 'Hey'. Este método também aceita o caractere 'H'como entrada, ou argumento , entre parênteses. Como a string 'Hey'começa com a letra 'H', o método retorna o booleano true.
Você pode encontrar uma lista de métodos de string integrados na documentação do JavaScript . Os desenvolvedores usam a documentação como ferramenta de referência. Ele descreve palavras-chave, métodos e sintaxe do JavaScript.

Instruções
Ponto de verificação 1 ativado
1 .
Use o .toUpperCase()método para registrar a string 'Codecademy'no console em letras maiúsculas.

Na segunda console.log()instrução em app.js , temos uma string ' Remove whitespace 'que possui espaços antes e depois das palavras 'Remove whitespace'.

Se navegarmos na documentação de strings JavaScript , encontraremos vários métodos de string integrados, cada um atingindo um objetivo diferente. O único método que parece ideal para nós é .trim().

Use o método para remover o espaço em branco no início e no final da string na segunda console.log()instrução.