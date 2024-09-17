OBJETOS AVANÇADOS
Valor da Propriedade Abreviado
3 minutos
O ES6 introduziu alguns novos atalhos para atribuir propriedades a variáveis, conhecidos como desestruturação .

No exercício anterior, criamos uma função de fábrica que nos ajudou a criar objetos . Tivemos que atribuir a cada propriedade uma chave e um valor, mesmo que o nome da chave fosse o mesmo que o nome do parâmetro que atribuímos a ela. Para nos lembrar, aqui está uma versão truncada da função de fábrica:

const monsterFactory = (name, age) => {
  return { 
    name: name,
    age: age
  }
};

Imagine se tivéssemos que incluir mais propriedades, esse processo se tornaria rapidamente tedioso! Mas podemos usar uma técnica de desestruturação, chamada property value shorthand , para economizar alguns toques de tecla. O exemplo abaixo funciona exatamente como o exemplo acima:

const monsterFactory = (name, age) => {
  return { 
    name,
    age 
  }
};

Observe que não precisamos nos repetir para atribuições de propriedades!

Instruções
Checkpoint 1 Passed
1 .
Use a abreviação do valor da propriedade e refatore a função de fábrica em main.js