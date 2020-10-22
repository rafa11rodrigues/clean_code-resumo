## Capítulo 4 - Comentários

Quando você escrever um comentário no código, sinta sua falta de capacidade de se expressar.

Comentários podem ser colocados longe do elemento referenciado (podem ter outras variáveis no meio) e podem não ser atualizados se o código mudar, de modo que ele se torne obsoleto e incoerente com o código atual.
Somente o código expressa o que realmente está acontecendo, então se sentir a necessidade de colocar um comentário, pense em refatorar o código.

Em algumas situações pode ser interessante colocar um comentário, mas no geral o melhor comentário é aquele que você não precisa escrever.
* colocar referências de licenças e copyrights no cabeçalho
* uma breve descrição do que um método retorna (mas ainda é melhor refatorar o nome do método) ou de uma expressão regular (mas ainda dá pra encapsular)
* explicar decisões de projeto
* esclarecer métodos e argumentos de terceiros, tomando muito cuidado pra explicar corretamente
* Avisar sobre operações perigosas
* TODO - lembrar que algo deve ser feito depois, mas deve ser checado com regularidade pra eliminar o que puder
* JavaDoc - ajuda quando o projeto será usado por terceiros, mas pode ser tão enganoso quanto qualquer outro comentário

Se for fazer um comentário, gaste tempo fazendo um comentário que valha a pena. Se o comentário fizer a pessoa olhar outro lugar, então o comentário é inútil.

Alguns comentários são redundantes e só poluem o código. Quase sempre o comentário pode ser substituído por uma refatoração de código.

Em vez de usar comentários para marcar final de funções, gaste tempo refatorando as funções para serem menores.

Não coloque informações muito grandes nem informações irrelevantes. Se for necessário ter um comentário, ele deve ser simples e estar muito bem conectado a um trecho de código.

### Resumo do resumo:

Se sentir que precisa de comentário pra explicar seu código, gaste tempo refatorando. Só então, depois que não tiver como melhorar a legibilidade e ainda tem algo faltando, aí sim gaste tempo pensando em um comentário simples e direto.

