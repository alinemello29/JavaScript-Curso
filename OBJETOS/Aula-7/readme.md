OBJETOS
Objetos aninhados
17 minutos
No código do aplicativo, os objetos geralmente são aninhados: um objeto pode ter outro objeto como propriedade, que por sua vez pode ter uma propriedade que é uma matriz de ainda mais objetos!

Em nosso spaceshipobjeto, queremos um crewobjeto. Isso conterá todos os membros da tripulação que fazem trabalho importante na nave. Cada um desses crewmembros são objetos em si. Eles têm propriedades como name, e degree, e cada um tem métodos exclusivos com base em suas funções. Também podemos aninhar outros objetos no spaceshipcomo a telescopeou aninhar detalhes sobre os computadores da nave espacial dentro de um nanoelectronicsobjeto pai.

const spaceship = {
     telescope: {
        yearBuilt: 2018,
        model: '91031-XLT',
        focalLength: 2032 
     },
    crew: {
        captain: { 
            name: 'Sandra', 
            degree: 'Computer Engineering', 
            encourageTeam() { console.log('We got this!') } 
         }
    },
    engine: {
        model: 'Nimbus2000'
     },
     nanoelectronics: {
         computer: {
            terabytes: 100,
            monitors: 'HD'
         },
        'back-up': {
           battery: 'Lithium',
           terabytes: 50
         }
    }
}; 

Podemos encadear operadores para acessar propriedades aninhadas. Teremos que prestar atenção em qual operador faz sentido usar em cada camada. Pode ser útil fingir que você é o computador e avaliar cada expressão da esquerda para a direita para que cada operação comece a parecer um pouco mais gerenciável.

spaceship.nanoelectronics['back-up'].battery; // Returns 'Lithium'

No código anterior:

Primeiro, o computador avalia spaceship.nanoelectronics, o que resulta em um objeto contendo os objetos back-upe computer.
Acessamos o back-upobjeto anexando ['back-up'].
O back-upobjeto possui uma batterypropriedade, acessada com .batterya qual retorna o valor ali armazenado:'Lithium'
Instruções
Checkpoint 1 Passed
1 .
Crie uma variável capFavee atribua a captaincomida favorita de 's (o elemento no índice 0 do 'favorite foods'array dela) a ela. Certifique-se de usar a notação de colchetes e pontos para obter o valor da comida por meio de acesso aninhado (não copie apenas o valor para a variável!)

Ponto de verificação 2 aprovado
2 .
No momento, a passengerspropriedade tem um valor de null. Em vez disso, atribua como seu valor um array de objetos. Esses objetos devem representar os spaceshippassageiros do como objetos individuais. Crie pelo menos um objeto passageiro no array que tenha pelo menos um par chave-valor nele.

Ponto de verificação 3 aprovado
3 .
Crie uma variável firstPassengere atribua o primeiro passageiro como seu valor (o elemento no índice 0 do spaceship.passengersarray que você acabou de fazer). Certifique-se de usar a notação de colchetes e pontos para obter o objeto passageiro por meio de acesso aninhado (não copie apenas o objeto para a variável!)