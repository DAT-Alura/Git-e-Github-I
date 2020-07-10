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

## Aula 3

1 - No último vídeo, nós trabalhamos bastante. Nossa primeira tarefa foi criar um novo repositório, que será utilizado como o nosso "servidor" Git, ou seja, todos os membros da equipe o acessarão para compartilhar suas mudanças.

Como fizemos para definir um repositório Git neste caso?

- __git init --bare__

> Alternativa correta! Com este comando nós criamos um repositório que não terá a working tree, ou seja, não conterá uma cópia dos nossos arquivos. Como o repositório servirá apenas como servidor, para que outros membros da equipe sincronizem seus trabalhos, poupamos espaço de armazenamento desta forma.

- git serve
- git init

2 - Antes de sincronizar as nossas mudanças no código com algum repositório remoto, precisamos antes adicioná-lo ao nosso repositório local.

Como adicionamos esta ligação entre os repositórios?

- git remote nome-repositorio caminho/para/o/repositorio
- git add remote nome-repositorio caminho/para/o/repositorio
- __git remote add nome-repositorio caminho/para/o/repositorio__

> Alternativa correta! Desta forma teremos um link do nosso repositório local com o repositório remoto, que chamamos de nome-repositorio, que está armazenado em caminho/para/o/repositorio.

3 - Além de adicionar repositórios remotos para sincronizar os dados, vimos que o git clone traz um repositório remoto para o nosso computador, criando um repositório local.

Ao alterar os códigos em nosso repositório local, como enviar as alterações para o repositório remoto?

- __git push [repositorio] master__

> Alternativa correta! Desta forma, nós enviamos as alterações em nosso branch master (falaremos mais sobre branches já já) para o repositório remoto. Basta substituir [repositorio] pelo nome que demos ao repositório ao adicioná-lo. Já para trazer os dados que estiverem no repositório remoto, podemos utilizar o git pull [repositorio] master.

- git pull [repositorio] master
- git push master [repositorio]