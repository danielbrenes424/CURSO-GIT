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


## Guaradado
git checkout -- <archivo> file returns to its original state
git reset <archivo> file is removed from commit but your edits are retained
git reset --hash move the project to the past at a certain point
git restore (restore everything from the last commit)

### logs

git log --graph
git log --graph --pretty=oneline (just oneline)
optimize logs
git log --graph --decorate --all --oneline

### Alias

include alias
git config --global alias.tlog "log --graph --decorate --all --oneline"

just call git tlog

### gitignore
en el .gitignore colocar **/file para ignorar archivos si es hidden colocar .file
- posterior generar git status para identificar sino lo esta leyendo actualmente


### git diff
change identification of files where i can see all the changes that i madre

### desplazamiento
HEAD pointer allow to go back in time on commits but you are not in any branch

Estado Detached: El HEAD apunta directamente a un commit (HEAD -> e2b544a). Si haces cambios aquí y haces un commit, esos cambios "flotarán" en el vacío y podrías perderlos al moverte

Always Safe mode
git checkout <hash del commit>
git checkout <main> for going back to the main branch that we are working on

if you like to work on there must create a branch
git checkout -b fix-version-antigua

### git reset

git reset --hard atras o adelante con el hash
comeback
git flog

git reflog
976c8d0 (HEAD -> main, rescue-docs) HEAD@{0}: merge rescue-docs: Fast-forward
eb4427c HEAD@{1}: checkout: moving from 976c8d0c874e368caea141008f97af3f955f05a5 to main
976c8d0 (HEAD -> main, rescue-docs) HEAD@{2}: commit: update documentation
eb4427c HEAD@{3}: checkout: moving from e2b544a6925c9c24e401c81225ad8d5794b7fbf8 to eb4427c
e2b544a HEAD@{4}: checkout: moving from main to e2b544a6925c9c24e401c81225ad8d5794b7fbf8
eb4427c HEAD@{5}: commit: all changes
89a4aad HEAD@{6}: commit: add gitignore2
6ad61b8 HEAD@{7}: commit: add gitignore

- git checkout (view in the past)
- git reset (rescribe history)


### git tag

git tag clase_1

commit 976c8d0c874e368caea141008f97af3f955f05a5 (HEAD -> main, tag: clase_1, rescue-docs)
Author: DanielBrenes <dbrenes424@gmail.com>
Date:   Mon May 4 18:14:34 2026 -0600


volvemos git checkout tags/clase_1


###
