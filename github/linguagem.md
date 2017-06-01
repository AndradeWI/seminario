# Linguagem
### [Git](https://git-scm.com/) - https://git-scm.com/

## COMANDOS BASICOS GITHUB

1. git init
Cria um diretório oculto (.git) com todas as configurações necessárias.
1. git status
Analisa e informa as condições dos arquivos locais em relação aos arquivos salvos remotamente no git, exibindo os arquivos com alteração que precisão ser adicionados ao cabeçalho e commitados, posteriormente.
1. git branch
Informa o branch (linha de desenvolvimento) em que os arquivos estão sendo manipulados.
1. git clone https://github.com/rusemberg/hello-world.git
Clona os arquivos salvos no git remotamente e salvam no disco local. Esse comando também já gera um “git remote”, sincronizando os arquivos salvos no disco com os salvos remotamente.
1. git add “nome_do_arquivo.arq”
Adiciona o arquivo alterado no cabeçalho .git para ser executado o commite e enviado o arquivo para git remoto.
1. git commit -m “Mensagem para ser enviada junto ao arquivo, identificando-o dos demais”
Salva, localmente, os arquivos que foram adicionados no cabeçalho através do “git add”.
1. git pull
Verifica se os arquivos salvos remotamente sofreram alguma alteração.
1. git push
Envia as alterações realizadas nos arquivos remotamente, realizando as alterações necessárias nos arquivos salvos no diretório remoto.
1. git config --global user.email “you@example.com”
Comando para configurar o email que o github irá utilizar quando for realizar um PUSH e não identificar o email automaticamente
1. git config --global user.name "Rusemberg"
Configura o nome do usuário github quando for realizado um comando “git push”
1. git config –list
Lista configurações
1. git commit -a –m “mensagem”
Adiciona os arquivos no Staging Area e já realiza o commit dos mesmos.
1. git diff
Informa, de forma detalhada, as alterações realizadas nos arquivos que estejam na Working Diectory.
1. git diff --staged
Informa, de forma detalhada, as alterações realizadas nos arquivos que estejam na Staging Area.
1. git log
Retorna um log de todos os comitês realizados no seu projeto, no seu diretório.
1. git log –p (git log + git diff)
Retorna um log de todos os comitês realizados no seu projeto, no seu diretório, informando ainda os diff’s de cada commit. Para sair da tela de log, deve –se digitar a letra “q”.
1. gitk
Abre o visualizador de relatório de alterações do git (Interface do Git).
1. git commit –amend –m “mensagem que foi inserida no commit que deseja editar (edicao)” 
Realiza edição de um commit que foi realizado anteriormente.
1. git reset HEAD <nome do arquivo>

Retira o arquivo do Staging Area.
1. git checkout -- <nome do arquivo>

Descarta as alterações feitas no arquivo, revertendo ao estado originaal do ultimo commit realizado no respectivo arquivo.
1. git rm <nome do arquivo> Remove o arquivo.

1. git tag –a v1.0 –m “mensagem da tag”
Cria uma tag anotada do ultimo commit realizado, permitindo que o usuário possa retornar a uma verão anterior para fazer consulta ou restaurar a respectiva versão, por exemplo.
1. git tag
Lista todas as tag’s criadas do projeto ou diretório.
1. git tag –a v0.0 <chave do commit que deseja versionar> -m “mensagem”
Cria uma tag anotada de um commit especifico.

1. git show <nome da tag>
Mostra detalhes de uma tag.

1. git checkout <nome da tag(versão) que deseja retornar>
Retornar os arquivos e o diretório ou projeto para o estado da versão em questão. Troca a verão do sistema para a tag especifica.
1. git checkout máster
Retornar ao ultimo estado do sistema.

1. git tag –d <nome da tag que deseja deletar>
Deleta a tag especificada.

1. git branch <nome do branch que deseja criar>
Cria um novo branch (uma nova linha de desencolvimento)

1. git checkout <nome do branch>
Transfere os arquivos do diretório para o branch informado, onde poderão ser realizadas as alterações necessárias.

1. git checkout –b <nome do branch>
Cria um novo branch e já transfere os arquivos do diretório para o novo branch criado.

1. git merge <nome do branch que deseja atualizar as alterações no branch que esta atualmente>
Atualiza as alterações realizadas em um branch especifico com o branch atual.

1. git branch –d <nome do branch>
Deleta o branch especificado.

## Trabalhando com Controle de Versão e Branch’s de Testes
1. realiza um git checkout <nome do branch de teste que deseja trabalhar>;

1. faz as modificações que deseja, que são necessárias no desenvolvimento;

1. realiza os git add <nome do arquivo>;

1. realiza o respectivo commit para salvar as alterações localmente;

1. para salvar as alterações no branch master, deve-se então fazer um “git checkout master”;

1. realizar o “git merge <nome do branch de teste que deseja atualizar com o master>;

1. realizar o “git pull”;
1. realizar o “git push”;

## Considerações Gerais
Git é um Sistema de Controle de Versão Distribuído que foi desenvolvido pelo Linus Torvalds para ajudar no desenvolvimento do Kernel do Linux.

Controle de Versão
É um sistema que gerencia, que registra todas as alterações que foram feitas em um arquivo ou em um conjunto de arquivos, permitindo que o usuário possa recuperar versões especificas quando houver necessidade. Permite também que várias pessoas possam trabalhar em um projeto, de forma organizada e mais segura. O git não é um sistema de controle de verão centralizado, ele é distribuído, ou seja, a cópia de cada versão que esta sendo desenvolvida estará em todas as estações de trabalho, além do repositório.
Estágios de trabalho no Git
Working Directory: antes de realizar “git add”;
Staging Area (Sala de espera): após realizar “git add” e antes de realizar “git commit”;
Git Directory: após realizar o “git commit”.
Cenários
Uma única estação de trabalho:

.gitignore: arquivo que tem especificações de arquivos e/ou diretórios que deseja que o git ignore quando for realizar as atualizações, verificar as mudanças ocorridas, ou seja, que o git deve ignorar o monitoramento..

## TUTORIAS 
https://guides.github.com/activities/hello-world/
https://gist.github.com/leocomelli/2545add34e4fec21ec16
https://www.youtube.com/watch?v=WVLhm1AMeYE&index=1&list=PLuN4DpjKVR1omeTtjvJRGU1_J8MsFN-fv (Vídeos aulas de curso básico de git)


