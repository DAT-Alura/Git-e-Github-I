# Para Saber Mais

## Git Status

Ao executar o comando git status, recebemos algumas informações que talvez não estejam tão claras, principalmente quando nos deparamos com termos como HEAD, working tree, index, etc.

Apenas para esclarecer um pouco, visto que entenderemos melhor o funcionamento do Git durante o treinamento, seguem algumas definições interessantes:

HEAD: Estado atual do nosso código, ou seja, onde o Git nos colocou
Working tree: Local onde os arquivos realmente estão sendo armazenados e editados
index: Local onde o Git armazena o que será commitado, ou seja, o local entre a working tree e o repositório Git em si.
Além disso, os possíveis estados dos nossos arquivos são explicados com detalhes neste link: <https://git-scm.com/book/pt-br/v2/Fundamentos-de-Git-Recording-Changes-to-the-Repository>. O texto do link está em inglês.

Acredite, embora pareça confuso agora, durante o treinamento tudo fará muito mais sentido! :-D

## Git Log

Conforme vimos no último vídeo, podemos visualizar o histórico de alterações em nosso projeto de forma muito fácil, através do comando git log.

Apesar de ser fácil, este comando é muito poderoso. Execute git log --help e veja algumas das opções possíveis. Para alguns exemplos mais fáceis de entender, você pode pesquisar sobre git log ou dar uma olhada neste link: <https://devhints.io/git-log>.

## Quando Comittar

Devemos gerar um commit sempre que a nossa base de código está em um estado do qual gostaríamos de nos lembrar. Nunca devemos ter commits de códigos que não funcionam, mas também não é interessante deixar para commitar apenas no final de uma feature.

Essa pode ser uma discussão sem fim e cada empresa ou equipe pode seguir uma estratégia diferente. Estude sobre o assunto, entenda o que faz mais sentido para você e sua equipe e seja feliz! :-D

## GitHub

No último vídeo, nós conhecemos (bem por alto) um dos serviços mais famosos e utilizados por pessoas que desenvolvem software: o GitHub.

Com o GitHub, podemos ter repositórios remotos públicos e privados gratuitos para armazenar e compartilhar o código dos nossos projetos.

O GitHub fornece muitas outras funcionalidades bem legais. Explore-as, brinque com elas, e em outros cursos aqui na Alura nós vamos falar mais sobre esse assunto.

## Ramificações (Branches)

Branches ("ramos") são utilizados para desenvolver funcionalidades isoladas umas das outras. A branch master é a branch "padrão" quando você cria um repositório.

É interessante separar o desenvolvimento de funcionalidades em branches diferentes, para que as mudanças no código para uma não influencie no funcionamento de outra.

Nesta aula, entenderemos melhor como trabalhar com estes ramos, mas é muito importante que você entenda seu propósito.

Em outros treinamentos aqui na Alura, falaremos mais sobre estratégias para organizar suas branches, então não precisa se preocupar tanto com isso agora! ;-)

## Conflitos com rebase

Vimos como é simples resolver conflitos identificados pelo Git ao tentar realizar o merge.

Agora, gere um conflito e, ao invés de utilizar o merge, utilize o rebase para atualizar o master:

- Vá para a branch titulo
- Commite algo
- Vá para a branch master, commite uma alteração na mesma linha
- Execute git rebase titulo

Veja a saída do Git e utilize as informações que ela te der para, após corrigir o conflito, continuar o rebase.

Boa sorte! ;-)
