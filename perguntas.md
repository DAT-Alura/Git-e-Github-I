# Perguntas

## Aula 1

1 - Agora que nós já entendemos para que serve um VCS (Version Control System), ou sistema de controle de versões, podemos dar continuidade com este treinamento, mas só para garantir...

Quais das afirmações a seguir sobre o Git estão corretas?

- Funciona apenas quando estivermos online
- __Nos deixa organizar o trabalho em equipe, mantendo as alterações nos arquivos em um servidor específico para isso__

> Alternativa correta! O Git permite que a gente armazene as modificações feitas em cada arquivo em um servidor próprio para isso. Toda a gestão de alterações é feita pelo Git e nós só precisamos nos preocupar em criar código que funciona, e não em quem alterou o que antes.

- __Permite armazenamento e acesso a um histórico de modificações__

> Alternativa correta! Cada alteração que você faz fica gravada em um histórico, podendo ser visualizada e restaurada a qualquer instante.

2 - Já entendemos o motivo para utilizar o Git. Começamos também a entender como o Git funciona. Sabemos que o Git faz a gestão de repositórios, e cada pessoa na equipe pode ter o seu repositório.

Como fazemos para o Git passar a enxergar determinada pasta como um repositório e a observar as mudanças em seus arquivos?

- __Através do comando git init__

> Alternativa correta! O git init inicializa um repositório no diretório em que o comando for executado. A partir deste comando, o Git poderá gerenciar as modificações realizadas nos arquivos.

- Através do comando git repository init
- Através do comando git init-repository

## Aula 2

1 - Para que o Git saiba quem está realizando as alterações, ele precisa de algumas configurações. Na primeira vez que você tentar realizar um commit em uma máquina, ele pedirá que você o configure.

Como podemos definir o nome da pessoa que executa commits no repositório local atual?

- git config --local username "Nome da pessoa"
- __git config --local user.name "Nome da pessoa"__

> Alternativa correta! Assim todos os commits executados neste repositório serão atribuídos à pessoa com nome Nome da pessoa. Para mais detalhes e outras configurações possíveis (até algumas mais avançadas), você pode conferir este link: <https://git-scm.com/book/en/v2/Customizing-Git-Git-Configuration>.

- git config --global user.name "Nome da pessoa"
