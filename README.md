# Git :pushpin:



Para usar repositórios Git basta aprender como funcionam os comandos presentes nas secções seguintes (E um terminal, pode ser Bash on Ubuntu on Windows, linux ou MacOS).
Se não tens um terminal linux, começa a tratar disso:

>
> - Windows :
>   
> Instalar Bash on Windows - https://msdn.microsoft.com/en-us/commandline/wsl/install-win10 ou https://www.windowscentral.com/how-install-bash-shell-command-line-windows-10
>  
> - Linux or MacOS
> 
> (segue para o passo seguinte)
  
    
 ### Instalar Git no terminal?
 
 ________________


 Verifica se ja tens Git instalado no teu terminal: ```git --version``` 
 
  > - Unix/Linux
  >
  > **@terminal:~$** ``` sudo apt-get install git ```
  >
  > - MacOS (brew)
  >
  > **@terminal:~$** ```brew install git ```
 

# Como funciona?     :information_source:

  Para começar, tens que fazer o link entre repositórios, Local e Cloud ***(1x only)***.
  -------------


- 1º `git clone <endereço do repositório no Github>` - Cria uma pasta clone na tua directoria

- 2º `git remote add origin <endereço do repositório no Github>` - Cria uma ligação entre o teu repositório local e o repositório no Github

- 3º `git fetch` - Adiciona as flags dos branchs existentes no repositório - Usa isto se já existir alguma coisa no respositório e além disso com mais do que um ramo

> **Note:**
> Só tens de fazer estes passos desta secção uma única vez por repositório. 


 Agora já podes começar a dar tudo no git! ( Entra dentro do repositorio: ``$ cd nome_do_repositorio``  )
-------------
- 4º `git status` - Dá-te a informação sobre os ficheiros e pastas existentes no repositório local
> **Note:**
>  -  4.1º - `git tree` - mostra-te o workflow , mas pr'a isso tens que instalar a feature : https://stackoverflow.com/questions/1064361/unable-to-show-a-git-tree-in-terminal


 Adicionar ficheiros e pastas ao teu repositório
-------------
- 5º `git add nomedoficheiro` - Adicionar um ficheiro ou uma pasta ( mas não adiciona o que está dentro da pasta)

> **Note:**
> - 5.1º `git add .` - Adiciona tudo
> - 5.2º `git add nomedapasta/*` - Adiciona pasta com ficheiros dentro
> - 5.3º `git add -u` - Adiciona todos os ficheiros modificados e eliminados

- 6º `git commit -m 'escreve o teu update'` - comentário de status

- 7º `git push origin` - usa origin no caso de estares no branch master. Na situação de não estares no branch certo, verifica com um git status ou git tree


 Actualizar o teu repositório
 -------------

- 8º `git pull`
> **Note** 
> - Se quiseres cagar naquilo que fizeste e queres **MESMO** o que está em cloud faz primeiro: `git checkout --` ou `git stash` (**mais seguro** - guarda o *commit* localmente e podes aceder-lo com  `git checkout <id do commit stashed>`)
> - Se quiseres juntar os códigos ( local vs cloud) , vais ter que resolver alguns conflitos. Entra dentro dos ficheiros e apaga aquilo que não queres (implentações mais antigas, por exemplo!) e volta a fazer push! - [**Acabaste de resolver/fazer um merge!**](http://gph.is/29qxLq2)  - `>>>> HEAD` será o identifcador da tua versão (no teu PC).  





[Feito !](https://github.com/bmalbusca/)
=========




Merge, Branch e Rebase (Em breve)
 -------------
 #### Trabalha num lado separado para tudo correr bem (Branches!)
 
 - 1º `git branch <nome do branch>` - Cria um ramo a partir do *node* actual

- 2º `git checkout <nome do branch usado>` - Muda a HEAD para o *branch* criado anteriormente. Neste momento estas a trabalhar no *branch* que criaste.

> **Note** 
> - Na primeira vez que tentares fazer *push* vais ter que usar  `--set-upstream origin <new-branch>` ou `-u origin <new-branch>` 


 ________________
 Para aprenderes mais um pouco sobre git vê : [github-tutorial](http://product.hubspot.com/blog/git-and-github-tutorial-for-beginners) e/ou  [git-guide]( http://rogerdudler.github.io/git-guide/)
. Explora também : [Vim](http://www.openvim.com) , [Tmux](http://www.hamvocke.com/blog/a-quick-and-easy-guide-to-tmux/) , [Sublime](https://www.sublimetext.com). 

- [Vim and Tmux config here! (link)](https://github.com/bmalbusca/Vim_config_files)
- [Git stats : git-quick-stats (link)](https://lukasmestan.com/git-quick-stats/) 

By Bmalbusca 

 
 
