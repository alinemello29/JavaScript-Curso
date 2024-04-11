Concatenação de Strings

Operadores não servem apenas para números! Quando um +operador é usado em duas strings, ele anexa a string direita à string esquerda:

console.log('hi' + 'ya'); // Prints 'hiya'
console.log('wo' + 'ah'); // Prints 'woah'
console.log('I love to ' + 'code.')
// Prints 'I love to code.'

Este processo de anexar uma string a outra é chamado de concatenação . Observe que no terceiro exemplo tivemos que incluir um espaço no final da primeira string. O computador unirá as cordas exatamente, então precisávamos incluir o espaço que queríamos entre as duas cordas.

console.log('front ' + 'space'); 
// Prints 'front space'
console.log('back' + ' space'); 
// Prints 'back space'
console.log('no' + 'space'); 
// Prints 'nospace'
console.log('middle' + ' ' + 'space'); 
// Prints 'middle space'

Assim como na matemática normal, podemos combinar ou encadear nossas operações para obter um resultado final:

console.log('One' + ', ' + 'two' + ', ' + 'three!'); 
// Prints 'One, two, three!'

Instruções
Ponto de verificação 1 ativado
1 .
Dentro de uma console.log()instrução, concatene as duas strings 'Hello'e 'World'.

Nota: Você deve concatenar as duas strings exatamente (sem introduzir caracteres adicionais).


Preso? Obtenha uma dica
A instrução da etapa do ponto de verificação 2 fica indisponível até que as etapas anteriores sejam concluídas
2 .
Deixamos o espaço da última vez. Crie uma segunda console.log()instrução na qual você concatena as strings 'Hello'e 'World', mas desta vez certifique-se de incluir também um espaço ( ' ') entre as duas palavras.