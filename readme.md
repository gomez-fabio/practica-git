**- ¿Qué comando utilizaste en el paso 11? ¿Por qué?**
```git reset --hard HEAD~1``. Me permite moverme en el grafo un paso atras ***(~1)***, con el modificador ***--hard*** cambio el ***working copy***.

**- ¿Qué comando o comandos utilizaste en el paso 12? ¿Por qué?**
  Localice el ***hash*** abreviado del ***commit*** que acababa de deshacer con ```git reflog``` y luego ```git reset --hard <hash>``` (el hash abreviado del ***commit***), 
  que de nuevo mueve los punteros de ***rama*** y ***head*** a ese ***commit*** identificado por el ***hash***, y con el modificador ***--hard*** cambio el contenido del ***working copy***.

**- El merge del paso 13, ¿Causó algún conflicto? ¿Por qué?**
  No causa ningún conflicto, ya que los ***commits*** están en la misma ***lista***, no en ***ramas*** diferentes. Desde el ***commit*** en el que estoy ya tengo el contenido del otro nodo.

**- El merge del paso 19, ¿Causó algún conflicto? ¿Por qué?**
  Si que creó un ***conflicto***, tengo el fichero en dos ***ramas*** paralelas con modificaciones en las mismas lineas.

**- El merge del paso 21, ¿Causó algún conflicto? ¿Por qué?**
  No, son ***commits*** en una ***lista***, es tan solo avanzar ***punteros***.

**- ¿Qué comando o comandos utilizaste en el paso 25?**
  ```git log --graph --decorate```

**- El merge del paso 26, ¿Podría ser fast forward? ¿Por qué?**
  Si, porque solo tendría que avanzar los ***punteros*** en la ***lista*** desde ***master*** al ***commit*** de title, y ni tendría que hacer un nuevo ***commit***.

**- ¿Qué comando o comandos utilizaste en el paso 27?**
  ```git reset HEAD~1```

**- ¿Qué comando o comandos utilizaste en el paso 28?**
  ```git checkout -- git-nuestro.md ```

**- ¿Qué comando o comandos utilizaste en el paso 29?**
  ```git branch -D title```

**- ¿Qué comando o comandos utilizaste en el paso 30?**
  ```git reflog``` para consultar el ***hash*** del ***commit***, ```git reset <hash>``` para ir al ***commit*** del ***merge***, como tenia cambios por "commitear", ```git add git-nuestro.md``` y luego ```git commit -m "paso 30". ```¨:

**- ¿Qué comando o comandos usaste en el paso 32?**
  ```git reflog ```para consultar el ***hash*** del ***commit*** y ```git checkout <hash>```

**- ¿Qué comando o comandos usaste en el punto 33?**
  ```git reflog``` para consultar el ***hash*** del ***commit*** ````git checkout <hash>````
