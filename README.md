Práctica del curso de git, gitHub y Sourcetree


Preguntas:

>
-¿Qué comando utilizaste en el paso 11? ¿Por qué? 

***Rpta:***

`$ git reset HEAD^`

Por que este hace que lo que esta en el HEAD anterior (HEAD^) se copie, se copie al HEAD actual y al Stagin Area, maneniendose en el Working Directory (es un `git reset --mixed HEAD^`) no se coloca el `mixed` por que es por default.

>-¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué? 

***Rpta:***

`git commit -a -m "👷<0001f3ff>  Rehacemos el ultimo commit que acabamos de deshacer"`

Utilece este comando por que me permite agregat al `stagin area` y hacer el commit a la vez, para pasarlo al `HEAD`



>-El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?

***Rpta:***

No, no causo conflicto, Salio `Already up-to-date` y es poque todo los cambios que hay en `master`, `styled` lo tiene.


>-El merge del paso 19, ¿Causó algún conflicto? ¿Por qué? 

***Rpta:***

Si, causo un conflicto, por que fue modificado el mismo archivo y en las mismas lineas.


Comandos realizados:

```git
git checkout styled
git merge htmlify
```

>-El merge del paso 21, ¿Causó algún conflicto? ¿Por qué? 

***Rpta:***

No, no causo ningun conflicto, por que practicamente solo actualizamos el master que estaba en una version anterior y se añadieron los nuevos cambios.

>-¿Qué comando o comandos utilizaste en el paso 25? 

***Rpta:***

`git log --graph --decorate --pretty=oneline`


>-El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?

***Rpta:***

Se uso el comando `git merge --no-ff title` , estando en master.

No porque tanto la rama `master` como la rama `title` tienen commit avanzados y estos de alguna forma tienen que combinarse.


>-¿Qué comando o comandos utilizaste en el paso 27?

***Rpta:***

git reset HEAD~1


>-¿Qué comando o comandos utilizaste en el paso 28?

***Rpta:***

git checkout -- git-nuestro.md


>-¿Qué comando o comandos utilizaste en el paso 29?

***Rpta:***

git branch -D title


>-¿Qué comando o comandos utilizaste en el paso 30?

***Rpta:***

$ git reflog
Luego vi el SHA donde hizimos el commit, en mi caso 6b3c2d3
$ git reset --hard 6b3c2d3


>-¿Qué comando o comandos usaste en el paso 32?

***Rpta:***

$ git reflog
Luego vi el SHA donde se creo el poema, en mi caso 039d9ff
$ git reset --hard 039d9ff

>-¿Qué comando o comandos usaste en el punto 33?

***Rpta:***

$ git reflog
Luego vi el SHA donde pusimos el titulo, en mi caso d0a1d16
$ git reset --hard d0a1d16



