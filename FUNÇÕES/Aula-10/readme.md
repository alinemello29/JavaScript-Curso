FUNÇÕES
Funções concisas da seta corporal

JavaScript também fornece várias maneiras de refatorar a sintaxe da função de seta . A forma mais condensada da função é conhecida como corpo conciso . Exploraremos algumas dessas técnicas abaixo:

Funções que usam apenas um único parâmetro não precisam que esse parâmetro esteja entre parênteses. No entanto, se uma função tiver zero ou vários parâmetros, serão necessários parênteses.

mostrando como os parâmetros das funções de seta diferem para diferentes quantidades de parâmetros
Um corpo de função composto por um bloco de linha única não precisa de chaves. Sem as chaves, tudo o que essa linha avaliar será retornado automaticamente. O conteúdo do bloco deve seguir imediatamente a seta =>e a returnpalavra-chave pode ser removida. Isso é conhecido como retorno implícito .

comparando funções de seta de linha única e multilinha
Então, se tivermos uma função:

const squareNum = (num) => {
  return num * num;
};

Podemos refatorar a função para:

const squareNum = num => num * num;

Observe as seguintes alterações:

Os parênteses num foram removidos, pois possui um único parâmetro.
As chaves { }foram removidas porque a função consiste em um bloco de linha única.
A returnpalavra-chave foi removida porque a função consiste em um bloco de linha única.
Instruções
Checkpoint 1 Passed
1 .
Vamos refatorar plantNeedsWater()para ser um corpo conciso. Observe que já convertemos a instrução if/ elseem um operador ternário para fazer o código caber em uma linha.