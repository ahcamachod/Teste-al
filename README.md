# Teste-al

# Git Hub

Content Track, rastrear versoes do codigo, 
To know exactly where the code messed up
what, when, where, how it changed?

Always when a Lab is made, we can save the status, save in both the computer and the Github.
Used to synchronize work
Collaborative work, wiki

when at the Desktop, Repository local, (folder)
when @ Github, remote repository: remote

4 MAIN COMMANDS

# 1. git init initializa o git =  Cria pasta
pasta objects armazena todas as modificaçoes 

$ cat .git/HEAD
ref: refs/heads/master
Branch inicial, branch Master

# 2. git status
$ git status
On branch master

Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)
$ git log
commit b5d0f8321369c7fe96d2984898a8ebac1b613fc8 (HEAD -> master)
Author: Alvaro Camacho <camacho_al@hotmail.com>
Date:   Mon Feb 17 17:30:52 2020 -0300

    last change

commit acfde3b480520ffbe76c18df52f977cd1dbf00ae
Author: Alvaro Camacho <camacho_al@hotmail.com>
Date:   Mon Feb 17 17:25:42 2020 -0300

    primeiro commit ok

commit 7957eaa6284c6047d9d8743a83324ba95f591baa
Author: Alvaro Camacho <camacho_al@hotmail.com>
Date:   Mon Feb 17 17:22:17 2020 -0300

    Este sera o primeiro commit, qualquer mensagem

Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)
$

No commits yet #(nao esta comprometido, nao rastreia)

Untracked files: #(nao rastreia)
  (use "git add <file>..." to include in what will be committed)
        arquivo.txt
        arquivo2.txt
        arquivo3.txt
        casa.txt
        example_file2

nothing added to commit but untracked files present (use "git add" to track)

# 3. git add (PRONTOS PARA SEREM MODIFICADOS) **CHECKPOINT**
$ git add arquivo.txt
warning: LF will be replaced by CRLF in arquivo.txt.
The file will have its original line endings in your working directory

Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)
# $ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   arquivo.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        arquivo2.txt
        arquivo3.txt
        casa.txt
        example_file2
  # git commit **(abre editor de texto que chama VIM)**
  How to exit aperta esc + : q! # para sair sem salvar or :qw para sair salvando
  
  Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)
$ git commit
Aborting commit due to empty commit message.

Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)
$ git commit -m "Este sera o primeiro commit, qualquer mensagem"
[master (root-commit) 7957eaa] Este sera o primeiro commit, qualquer mensagem
 1 file changed, 5 insertions(+)
 create mode 100644 arquivo.txt

Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)
$ git status
On branch master
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        arquivo2.txt
        arquivo3.txt
        casa.txt
        example_file2

nothing added to commit but untracked files present (use "git add" to track)

Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)

# 5. git log (todas as vezes que deu commit)

Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)
$ git log
commit 7957eaa6284c6047d9d8743a83324ba95f591baa (HEAD -> master)
Author: Alvaro Camacho <camacho_al@hotmail.com>
Date:   Mon Feb 17 17:22:17 2020 -0300

    Este sera o primeiro commit, qualquer mensagem
    
#### EXECUCAO DOS COMANDOS GIT

Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)
$

Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)
$ mkdir test

Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)
$ mv arquivo2.txt test/

Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)

# exemplo status
$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   example_file2

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    arquivo2.txt

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        arquivo3.txt
        casa.txt
        test/


Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)
$ ls test
arquivo2.txt

Alvaro Camacho@DESKTOP-677B14I MINGW64 ~/Desktop/pasta_exemplo (master)
$
