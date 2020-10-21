## Capítulo 2 - Nomes Significativos

O nome de uma variável, função ou classe deve responder: por que existe, o que faz e como usar. Se foi necessário colocar um comentário explicando isso, então o nome não revela a intenção.

Evite usar abreviações, nomes comuns a ambientes e o prefixo "list" se o elemento não for uma lista.

Nomes diferentes devem significar coisas diferentes, então cuidado com prefixos e sufixos inúteis.

Use nomes pronunciáveis em vez de siglas e abreviações, eles facilitam a comunicação entre os desenvolvedores.

Use nomes fáceis de serem pesquisados de acordo com o escopo. Se um nome pode ser visto em vários lugares, é interessante ter um nome um pouco mais longo.

Evite códigos, mapas mentais, piadas internas. Já temos muito trabalho em codificar regras de negócio e elementos da linguagem de programação, então pra quê criar mais coisas pra ficar pensando no que significam?

Nomes de classes devem ser nomes ou adjuntos adnominais, métodos devem ser verbos ou adjuntos adverbiais.

Use um mesmo nome para um mesmo significado (ex: ou só fetch, ou só get, ou só retrieve, se usar cada hora um nome diferente pode confundir).
Não use o mesmo nome para contextos diferentes.

Quem vai ler seu código serão outros programadores, então nomes que indicam assuntos técnicos são interessantes (jobQueue, accountVisitor - padrão de projeto Visitor), pois são conceitos que "todos" entendem.
Quando faltar um bom nome técnico, use nomes de domínio, assim é possível tirar dúvida com os analistas ao ler um código escrito por outra pessoa.

Use nomes adequados ao contexto. Às vezes vários nomes curtos dentro de um contexto fazem sentido, mas em um outro pode ser necessário adicionar um prefixo para indicar o contexto.
Por exemplo, campos de endereço em uma classe Endereço podem ser apenas logradouro, bairro, mas fora da classe pode ser necessário colocar enderecoLogradouro.

Um método pode receber um contexto e um significado mais visível se for quebrado em pequenas partes, ou até mesmo criando uma classe para envolver a lógica do método original.
Mas cuidado pra não adicionar mais contexto do que o necessário, pois um nome curto (entendível) é melhor que um nome comprido.

