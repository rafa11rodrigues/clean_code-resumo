## Capítulo 3 - Funções

Funções devem ser pequenas. Se a lógica da função estiver muito grande e complexa, extraia para outras funções, de modo que todo o processo seja uma historinha.

Funções devem ter apenas 1 ou 2 níveis de aninhamento. Em geral, blocos if, else, while e afins devem ter só uma linha contendo a chamada para uma outra função (o que ajuda a manter 1 ou 2 níveis de aninhamento).

Uma função deve fazer só uma coisa (e fazer bem). Fazer uma só coisa significa uma sequência de pequenos passos que estão 1 nível de abstração abaixo do nome da função.
Quando não der mais pra extrair funções sem que a nova função seja apenas a mesma sequência de instruções mas com um nome diferente, aí sim a função está fazendo só uma coisa.
Ou ainda, quando não der pra separar a função em seções (inicialização, checar condições, executar, limpar...), então a função está fazendo só uma coisa

Funções devem ser lidas de cima pra baixo, como se fossem vários parágrafos de uma narrativa. Pensar nisso ajuda a fazer funções pequenas com apenas 1 nível de abstração, que fazem apenas 1 coisa.

Usar switch (ou if/else) pra fazer operações diferentes de acordo com um tipo é problemático, pois o código precisa ser alterado se novos tipos surgirem e pode haver novas operações com a mesma estrutura.
Nesses casos, polimorfismo ajuda: esconder o switch em um factory que cria diferentes instâncias de acordo com o tipo, e cada instância implementa a sua operação.

Use nomes descritivos, mesmo que sejam longos (é melhor um nome longo e descritivo do que nome curto que não diz nada sobre o que a função faz).
Quanto menor a função, mais fácil de escolher um bom nome.

Use o menor número de argumentos possível em uma função, pois restringe o conceito de o que a função faz e facilita os testes (quanto mais argumentos, mais possibilidade de combinações de valores pra testar).
Funções com mais de 3 argumentos precisam de uma justificativa muito boa pra serem usadas.
Sempre que possível, refatore as funções pra usar apenas um argumento.

Passar flags como argumentos é ruim, pois isso significa que a função faz duas coisas (um caminho pra quando a flag é verdadeira e outro pra quando é falsa).

Não faça funções com efeitos colaterais. Se nome da função diz que ela vai fazer X, se proponha a fazer apenas X. Se precisar fazer mais alguma coisa, informe no nome da função.

Evite argumentos de saída (ex: passar referência de um objeto que será modificado na função). Refatore para que o comportamento seja um método dentro da classe do objeto.

Separe ação de consulta (command query separation). Ou a função realiza algo ou ela responde uma pergunta, mas nunca os dois ao mesmo tempo.

Lance exceções em vez de retornar códigos de erro, pois isso dá liberdade pra tratar o erro em outro momento, separando da lógica principal.

Isole o caminho feliz do tratamento da exceção. Se necessário, crie uma função que executa o caminho feliz e outra que trata a exceção:
```
try {
    happyPath();
} catch (Exception e) {
    handleException(e);
}
```
Funções devem fazer só uma coisa, e tratar erros é uma coisa.

Evite duplicações. Use todos os recursos existentes (funções, classes...) pra isolar partes repetidas.

