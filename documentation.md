## Globales

- configuracion git

git config --global user.name "DanielBrenes"
git config --global user.email "dbrenes424@gmail.com"

Ya estaba configurado

## Inicializar git

git init (create a .git hidden)

## Branch

photograph
git status

# add files to git
git add FILENAME ex

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
	new file:   hellogit.py

Untracked files:
  (use "git add <file>..." to include in what will be committed)
	documentation.md


# pass status local to photograph
git commit

git commit -m "nuevos archivos"
[main (root-commit) e2b544a] nuevos archivos
 2 files changed, 14 insertions(+)
 create mode 100644 documentation.md
 create mode 100644 hellogit.py


## once created the commit
git status
On branch main
nothing to commit, working tree clean

## logs de git

git log
commit e2b544a6925c9c24e401c81225ad8d5794b7fbf8 (HEAD -> main)
Author: DanielBrenes <dbrenes424@gmail.com>
Date:   Mon May 4 10:39:59 2026 -0600


## inclusion del segundo fichero 
git commit -m "nuevos archivos 2"
[main eb1e631] nuevos archivos 2
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 hellogit2.py



