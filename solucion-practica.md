En el repositorio, deberá existir un archivo readme.md con las respuestas a las siguientes preguntas:
- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
- El merge del paso 13, ¿Causó algún conﬂicto? ¿Por qué?
- El merge del paso 19, ¿Causó algún conﬂicto? ¿Por qué?
- El merge del paso 21, ¿Causó algún conﬂicto? ¿Por qué?
- ¿Qué comando o comandos utilizaste en el paso 25?
- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
- ¿Qué comando o comandos utilizaste en el paso 27?
- ¿Qué comando o comandos utilizaste en el paso 28?
- ¿Qué comando o comandos utilizaste en el paso 29?
- ¿Qué comando o comandos utilizaste en el paso 30?
- ¿Qué comando o comandos usaste en el paso 32?
- ¿Qué comando o comandos usaste en el punto 33?

Los pasos a ejecutar son los siguientes (los pasos en negrita indican que hay una pregunta
asociada):
1) Crear un repositorio en GitHub y clónalo en tu equipo
2) Crear un archivo git-nuestro.md con el contenido:

Git nuestro
Git nuestro que estas en los repos
Comprimidos sean tus commits
Venga a nosotros tu log
En el local como en el remote
Danos hoy nuestro pull de cada día
Perdona nuestros conflictos
Como también perdonamos los de otros geeks
No nos dejes caer en detached HEAD
y líbranos de SVN
git commit --amend

3) Añadir git-nuestro.md al staging área -> git add

4) Mover lo que hay en el staging area al repositorio -> git commit

5) Crear una rama llamada “styled” -> git Branch styled ( sobre el commit 45038ffdb70cdc45a17926cf27a9594933103b9 / detached head)

6) Listar las ramas que hay en el repositorio -> git branch
* (HEAD detached at 45038ff)
  NewBranch
  main
  styled

7) Moverse a la rama “styled” -> git checkout styled -> Switched to branch 'styled'

8) Comprobar que se está en la rama correcta -> git Branch

9) Modiﬁcar en el archivo git-nuestro.md: -> nano git_nuestro.md

*Git* nuestro que estás en los repos
Comprimidos sean tus *commits*
Venga a nosotros tu *log*
En el local como en el *remote*
Danos hoy nuestro *pull* de cada día
Perdona nuestros *conflictos*

Como también perdonamos los de otros geeks
No nos dejes caer en *detached HEAD*
y líbranos de *SVN*
`git commit --amend`

10) Añadir los cambios al staging area y luego pasarlos al repositorio ->git add + git commit -m " Hago 1er Update del archivo"

11)**Deshacer el último commit (perdiendo los cambios realizados en el working copy) -> git reset --hard HEAD~1**

12)**Rehacer el último commit (el que acabamos de deshacer) -> git reflog + git reset --hard <numero_commit>**

13)**Hacer un merge con ‘main’ (styled absorbe a main) -> git merge main (debemos estar en styled - git checkout styled)**

14) Volver a la rama main -> git checkouot main

15) Crear una nueva rama llamada “htmlify” -> git Branch htmlify

16) Cambiar a la rama htmlify -> git checkout htmlify / git switch

17) Modiﬁcar en el archivo git-nuestro.md: nano git-nuestro.md 

<p><em>Git</em> nuestro que estas en los repos<br />
Comprimidos sean tus <em>commits</em><br />
Venga a nosotros tu <em>log</em><br />
En el local como en el <em>remote</em><br />
Danos hoy nuestro <em>pull</em> de cada día<br />
Perdona nuestros <em>conflictos</em><br />
Como también perdonamos los de otros geeks<br />
No nos dejes caer en <em>detached HEAD</em><br />
y líbranos de <em>SVN</em><br />
<code>git commit --amend</code></p>

18) Hacer un commit -> git add + git commit -m "Hago 2do Update del Archivo"

19)**Hacer un merge de “htmlify” en “styled” (styled absorbe a htmlify) -> git merge htmlify (verificar estar en la rama styled(git Branch + git checkout)**

20) Si hay conﬂictos, deberemos resolverlos quedándonos con el contenido de la rama “styled”. -> nano git-nuestro.md (modificamos) + git add + git commit + git merge

21)**Desde “main”, hacer un merge con “styled” -> ir a main y hacer un merge (git checkout main + git merge styled)**
 
22) Crear una rama “title” y cambiarse a esa rama -> git Branch y git checkout

23) Añadir un título (a tu gusto) al archivo git-nuestro.md y hacer un commit.-> nano + git add + git commit - m "Agrego titulo a nuestro archivo"

#***El Padre Git: Una Oración Geek por la Paz del Repositorio***
24) Volver a la rama main -> git checkout main

25)**Dibujar el diagrama -> git log --graph --decorate --pretty=oneline**

26)**Hacer un merge “no fast-forward” de “title” en “main” (main absorbe a title) -> git merge --no-ff tittle**

27)**Deshacer el merge (sin perder los cambios del working copy)-> git log --graph + git reset --hard<numero_commit>**

28)**Descartar los cambios-> git reflog -> git reset --hard<numero_commit>**

29)**Eliminar la rama “title”-> git branch -d tittle (desde main o donde se haya hecho merge) o git Branch -D directamente(forzado)**

30)**Rehacer el merge que hemos deshecho-> desde reflog-> ya hecho en paso 28**

En el
repositorio, deberá existir un archivo readme.md con las respuestas a las siguientes preguntas:
- ¿Qué comando utilizaste en el paso 11? ¿Por qué?
- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?
- El merge del paso 13, ¿Causó algún conﬂicto? ¿Por qué?
- El merge del paso 19, ¿Causó algún conﬂicto? ¿Por qué?
- El merge del paso 21, ¿Causó algún conﬂicto? ¿Por qué?
- ¿Qué comando o comandos utilizaste en el paso 25?
- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?
- ¿Qué comando o comandos utilizaste en el paso 27?
- ¿Qué comando o comandos utilizaste en el paso 28?
- ¿Qué comando o comandos utilizaste en el paso 29?
- ¿Qué comando o comandos utilizaste en el paso 30?
- ¿Qué comando o comandos usaste en el paso 32?
- ¿Qué comando o comandos usaste en el punto 33?

Los pasos a ejecutar son los siguientes (los pasos en negrita indican que hay una pregunta
asociada):
1) Crear un repositorio en GitHub y clónalo en tu equipo
2) Crear un archivo git-nuestro.md con el contenido:

Git nuestro
Git nuestro que estas en los repos
Comprimidos sean tus commits
Venga a nosotros tu log
En el local como en el remote
Danos hoy nuestro pull de cada día
Perdona nuestros conflictos
Como también perdonamos los de otros geeks
No nos dejes caer en detached HEAD
y líbranos de SVN
git commit --amend

3) Añadir git-nuestro.md al staging área -> git add

4) Mover lo que hay en el staging area al repositorio -> git commit

5) Crear una rama llamada “styled” -> git Branch styled ( sobre el commit 45038ffdb70cdc45a17926cf27a9594933103b9 / detached head)

6) Listar las ramas que hay en el repositorio -> git branch
* (HEAD detached at 45038ff)
  NewBranch
  main
  styled

7) Moverse a la rama “styled” -> git checkout styled -> Switched to branch 'styled'

8) Comprobar que se está en la rama correcta -> git Branch

9) Modiﬁcar en el archivo git-nuestro.md: -> nano git_nuestro.md

*Git* nuestro que estás en los repos
Comprimidos sean tus *commits*
Venga a nosotros tu *log*
En el local como en el *remote*
Danos hoy nuestro *pull* de cada día
Perdona nuestros *conflictos*

Como también perdonamos los de otros geeks
No nos dejes caer en *detached HEAD*
y líbranos de *SVN*
`git commit --amend`

10) Añadir los cambios al staging area y luego pasarlos al repositorio ->git add + git commit -m " Hago 1er Update del archivo"

11)**Deshacer el último commit (perdiendo los cambios realizados en el working copy) -> git reset --hard HEAD~1**

12)**Rehacer el último commit (el que acabamos de deshacer) -> git reflog + git reset --hard <numero_commit>**

13)**Hacer un merge con ‘main’ (styled absorbe a main) -> git merge main (debemos estar en styled - git checkout styled)**

14) Volver a la rama main -> git checkouot main

15) Crear una nueva rama llamada “htmlify” -> git Branch htmlify

16) Cambiar a la rama htmlify -> git checkout htmlify / git switch

17) Modiﬁcar en el archivo git-nuestro.md: nano git-nuestro.md 

<p><em>Git</em> nuestro que estas en los repos<br />
Comprimidos sean tus <em>commits</em><br />
Venga a nosotros tu <em>log</em><br />
En el local como en el <em>remote</em><br />
Danos hoy nuestro <em>pull</em> de cada día<br />
Perdona nuestros <em>conflictos</em><br />
Como también perdonamos los de otros geeks<br />
No nos dejes caer en <em>detached HEAD</em><br />
y líbranos de <em>SVN</em><br />
<code>git commit --amend</code></p>

18) Hacer un commit -> git add + git commit -m "Hago 2do Update del Archivo"

19)**Hacer un merge de “htmlify” en “styled” (styled absorbe a htmlify) -> git merge htmlify (verificar estar en la rama styled(git Branch + git checkout)**

20) Si hay conﬂictos, deberemos resolverlos quedándonos con el contenido de la rama “styled”. -> nano git-nuestro.md (modificamos) + git add + git commit + git merge

21)**Desde “main”, hacer un merge con “styled” -> ir a main y hacer un merge (git checkout main + git merge styled)**
 
22) Crear una rama “title” y cambiarse a esa rama -> git Branch y git checkout

23) Añadir un título (a tu gusto) al archivo git-nuestro.md y hacer un commit.-> nano + git add + git commit - m "Agrego titulo a nuestro archivo"

#***El Padre Git: Una Oración Geek por la Paz del Repositorio***
24) Volver a la rama main -> git checkout main

25)**Dibujar el diagrama -> git log --graph --decorate --pretty=oneline**

26)** Hacer un merge “no fast-forward” de “title” en “main” (main absorbe a title) -> git merge --no-ff tittle **

27)**Deshacer el merge (sin perder los cambios del working copy)-> git log --graph + git reset --hard<numero_commit>**

28)** Descartar los cambios-> git reflog -> git reset --hard<numero_commit> **

29)** Eliminar la rama “title”-> git branch -d tittle (desde main o donde se haya hecho merge) o git Branch -D directamente(forzado)**

30)** Rehacer el merge que hemos deshecho-> desde reflog-> ya hecho en paso 28**

31) Volver a main y eliminar el resto de ramas-> git checkout main -> git Branch + git Branch -d <nombre_rama>

32) **Volver al commit inicial cuando se creó el poema-> git log + git checkout <numero_commit>**

33) **Volver al estado ﬁnal, cuando pusimos título al poema->git log + git checkout <numero_commit>**

34) Crear los siguientes tags:-> git reflog para tener los códigos y git tag uno a uno -> git tag <tag_name> <commit_hash> 
inicial: en el primer commit 
styled: modiﬁcación del paso 10  
htmlify: modiﬁcación del paso 17-18
title: modiﬁcación del paso 30

35) Ir al tag htmlify -> git checkout htmlify (detached head)

36) Vuelve a la rama main-> git checkout main
 
37) Sube a GitHub todas las ramas y todos los tags-> git push --all origin + git push tags
