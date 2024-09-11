OBJETOS AVANÇADOS
Privacidade
6 minutos
Acessar e atualizar propriedades é fundamental ao trabalhar com objetos . No entanto, há casos em que não queremos que outro código simplesmente acesse e atualize as propriedades de um objeto. Ao discutir privacidade em objetos, definimos isso como a ideia de que apenas certas propriedades devem ser mutáveis ​​ou capazes de mudar de valor.

Certas linguagens têm privacidade incorporada para objetos, mas JavaScript não tem esse recurso. Em vez disso, os desenvolvedores de JavaScript seguem convenções de nomenclatura que sinalizam para outros desenvolvedores como interagir com uma propriedade. Uma convenção comum é colocar um sublinhado _antes do nome de uma propriedade para significar que a propriedade não deve ser alterada. Aqui está um exemplo de uso _para prefixar uma propriedade.

const bankAccount = {
  _amount: 1000
}

No exemplo acima, o _amountnão se destina a ser manipulado diretamente.

Mesmo assim, ainda é possível reatribuir _amount:

bankAccount._amount = 1000000;

Em exercícios posteriores, abordaremos o uso de métodos chamados getters e setters . Ambos os métodos são usados ​​para respeitar a intenção de propriedades prefixadas, ou iniciadas, com _. Getters podem retornar o valor de propriedades internas e setters podem reatribuir valores de propriedade com segurança. Por enquanto, vamos ver o que acontece se pudermos alterar propriedades que não têm setters ou getters.

Instruções
Checkpoint 1 Passed
1 .
Abaixo do robotobjeto, reatribua a _energyLevelpropriedade para 'high'.

Ponto de verificação 2 aprovado
2 .
Agora dê uma olhada no novo rechargemétodo em robot. .recharge()irá adicionar 30a _energyLevel.

O que vai acontecer agora que _energyLevelnão é um número?

Ligue .recharge()para robotsaber mais.

Observe que uma string funky é impressa no console! Isso é conhecido como um efeito colateral da coerção de tipo. Não precisa se preocupar com o que isso significa por enquanto, mas é importante entender que você pode causar efeitos colaterais indesejados ao mutar objetos e suas propriedades.