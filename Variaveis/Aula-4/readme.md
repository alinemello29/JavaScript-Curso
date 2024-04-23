VARIÁVEIS
Crie uma variável: const

A constpalavra-chave também foi introduzida no ES6 e é uma abreviação da palavra constante. Assim como com vare letvocê pode armazenar qualquer valor em uma constvariável. A maneira como você declara uma constvariável e atribui um valor a ela segue a mesma estrutura de lete var. Dê uma olhada no seguinte exemplo:

const myName = 'Gilberto';
console.log(myName); // Output: Gilberto

No entanto, uma constvariável não pode ser reatribuída porque é constante . Se você tentar reatribuir uma constvariável, obterá um arquivo TypeError.

Variáveis ​​constantes devem receber um valor quando declaradas. Se você tentar declarar uma constvariável sem valor, obterá um arquivo SyntaxError.

Se você estiver tentando decidir entre qual palavra-chave usar letou const, pense se precisará reatribuir a variável mais tarde. Se você precisar reatribuir a variável use let, caso contrário, use const.

Instruções
Ponto de verificação 1 Envio
1 .
Crie uma variável constante chamada entreee defina-a como igual à string 'Enchiladas'.


Ponto de verificação 2 aprovado
2 .
Apenas para verificar se você salvou o valor de 'Enchiladas'to entree, registre o valor de entreeno console.


Ponto de verificação 3 aprovado
3 .
Ótimo, vamos ver o que acontece se você tentar reatribuir uma variável constante.

Cole o seguinte código na parte inferior do seu programa.

entree = 'Tacos'

Este código gera o seguinte erro quando você executa seu código:

TypeError: Assignment to constant variable.
Depois de passar por esse ponto de verificação, se quiser ver outra peculiaridade constem ação, abra a dica!