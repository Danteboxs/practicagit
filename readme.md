- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
  git reset --hard HEAD~1 vuele al commit anterior, dejando los ficheros como estaban en ese commit

- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
  git reset --hard HEAD@{1} vuelve al commit justo antes del desecho en el anterior.
  
- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?
  git merge master, no hay conflicto ya que la rama esta por detras la actual, no hay conflictos.
  
- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?
  git checkout styled, git merge htmlify. Hay conflictos por que se ha tocado en las dos ramas el mismo fichero en la/s misma/s linea

- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?
  git checkout master, git merge styled, no hay conflicto se actualiza correctamente por que en la rama master no se habia tocado el fichero.
  
- ¿Qué comando o comandos utilizaste en el paso 25?
  git log --graph --decorate --pretty=oneline.
  git config --global alias.pintar 'log --graph --decorate --pretty=oneline'
  git pintar
  
- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
  Git merge title --no-ff, si podria se fast ya que se moveria el puntero correctamente y no se perderian cambios.
  creo que mejor no fast por que queda constancia, depende de caso dejar constancia en nuevo commit o no del mergeo.
  
- ¿Qué comando o comandos utilizaste en el paso 27?
  git reset HEAD~1, vuelve justo al anterior y quedan los cambios pendientes.

- ¿Qué comando o comandos utilizaste en el paso 28?
  git checkout -- git-nuestro.md, descarta los cambios del fichero.

- ¿Qué comando o comandos utilizaste en el paso 29?
  git branch –D title
  
- ¿Qué comando o comandos utilizaste en el paso 30?
  git reflog y busco el commit donde se hizo el merge por ejemplo, hago un git checkout HEAD@{5} y luego creo la rama git branch title

- ¿Qué comando o comandos usaste en el paso 32?
  git checkout HEAD@{25}, es mi primer commit.

- ¿Qué comando o comandos usaste en el punto 33?
  git checkout 35d3849, me he ido al commit donde creaba el titulo, a partir de ahi he creado un rama nueva, git branch titulo, luego me he ido al master y hecho un
  git merge titulo