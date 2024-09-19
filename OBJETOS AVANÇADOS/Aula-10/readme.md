OBJETOS AVANÇADOS
Métodos de Objetos Integrados
13 minutos
Nos exercícios anteriores, criamos instâncias de objetos que têm seus próprios métodos . Mas também podemos aproveitar os métodos internos para Objetos!

Por exemplo, temos acesso a métodos de instância de objeto como: .hasOwnProperty(), .valueOf(), e muitos mais! Pratique suas habilidades de leitura de documentação e confira: Documentação de instância de objeto do MDN .

Também há métodos úteis de classe Object como Object.assign(), Object.entries(), e Object.keys()apenas para citar alguns. Para uma lista abrangente, navegue: Documentação de instância de objeto do MDN .

Vamos nos familiarizar com alguns desses métodos e sua documentação.

Observação: você verá erros ao longo deste exercício, mas no final eles serão corrigidos!

Instruções
Checkpoint 1 Passed
1 .
Em main.js há um objeto, robot. Gostaríamos de pegar os nomes de propriedade, também conhecidos como chaves, e salvar as chaves em um array que é atribuído a robotKeys. No entanto, há algo faltando na chamada do método.

Descubra o que precisamos incluir lendo a documentação do MDNObject.keys() .

Ponto de verificação 2 aprovado
2 .
Object.entries()também retornará um array, mas o array conterá mais arrays que têm tanto a chave quanto o valor das propriedades em um objeto.

Declare uma constvariável chamada robotEntriese atribua a ela as entradas de robotchamando Object.entries().

Para saber como usar Object.entries(), leia a documentação no MDN .

Ponto de verificação 3 aprovado
3 .
Agora, e se quisermos outro objeto que tenha as propriedades de, robotmas com algumas propriedades adicionais. Object.assign()Parece um ótimo método para usar, mas, como nos exemplos anteriores, devemos verificar a documentação do Object.assign() no MDN .

Declare uma constvariável chamada newRobot. newRobotserá um novo objeto que tem todas as propriedades de robote as propriedades no seguinte objeto: {laserBlaster: true, voiceRecognition: true}. Certifique-se de que você não está alterando o robotobjeto!