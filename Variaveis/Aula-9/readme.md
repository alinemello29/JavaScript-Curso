VARIÁVEIS
operador typeof

Ao escrever o código, pode ser útil acompanhar os tipos de dados das variáveis ​​no seu programa. Se precisar verificar o tipo de dados do valor de uma variável, você pode usar o typeofoperador.

O typeofoperador verifica o valor à sua direita e retorna , ou devolve, uma string do tipo de dados.

const unknown1 = 'foo';
console.log(typeof unknown1); // Output: string

const unknown2 = 10;
console.log(typeof unknown2); // Output: number

const unknown3 = true; 
console.log(typeof unknown3); // Output: boolean

Vamos analisar o primeiro exemplo. Como o valor unknown1é 'foo', uma string typeof unknown1retornará 'string'.

Instruções
Ponto de verificação 1 Envio
1 .
Use console.log()para imprimir o arquivo typeof newVariable.

Ponto de verificação 2 aprovado
2 .
Ótimo, agora vamos verificar o que acontece se reatribuirmos a variável. Abaixo da console.log()instrução, reatribua newVariablepara 1.

Ponto de verificação 3 aprovado
3 .
Como você atribuiu esse novo valor a newVariable, ele tem um novo tipo! Na linha abaixo da sua reatribuição, use console.log()para imprimir typeof newVariablenovamente.