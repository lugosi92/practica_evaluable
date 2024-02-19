### 1.**Directorios y Ficheros (Crear repositorio)**
- `echo "Contenido del archivo" > archivo.txt` → Añade texto y lo crea
- `touch archivo.txt`       # Crea un documento
- `mkdir carpeta`        # Crea un directorio
- `git init`               # Inicia un repositorio


**Validar repositorios**
- `git status`             # Estado actual del repositorio
`git add .`              # Agrega todos los archivos modificados
`git status`           # Estado actual del repositorio
`git commit -m "Comentario"`  # Confirma los cambios realizados en los archivos (HEAD, apunta al último commit)

**Versiones creadas**
`git log --oneline  `    # Muestra el historial de commits de manera resumida
`git log`                # Más extenso
`git show `              # Ver cambio en todos los commits
`git show idCommit `     # Muestra un commit concreto


**Comparar cambios**
`git diff`               # Compara el área de working y el commit que llamamos HEAD.
`git diff HEAD~1 HEAD`   # Diferencia entre varios commits indicando los apuntadores
`git diff id HEAD`       # Consultar la diferencia entre varios commits

**Repositorio remoto**
`git remote add origin http://github.com/GemaBT/Hola-Mundo.git`
`git push` 
`git remote -v`

**Crear copia con checkout**
`git init`
`git remote add origin <nombre-repositorio-remoto>`
`git fetch origin master`
`git checkout origin/master`

**Revertir resetear commits**
`git reset --hard HEAD~1`    # Resetea el estado de tu directorio de trabajo y el área de preparación al estado del último commit de la rama en la que te encuentras
`git revert HEAD`            # Para revertir el último commit en Git

**Conectar con Git Hub**
`git remote add origin https://github.com/lugosi92/practica_evaluable.git`
`git push -u origin master`
`git push origin master`    # Sincronizar con el repositorio remoto
`git push -u origin master`  # La rama como local actual
`git pull origin main`      # Actualizar rama


**Crear rama y cambiar a ella**
`git branch`               # Consultar ramas
`git branch mirama`
`git checkout mirama`      # Puede ser con directorios, ficheros, etc.
`git checkout -b`          # Para cambiara ella directamente

**Validar**
`git merge mirama`         # Fusionar ramas 
`git branch -d mirama`     # BORRAR RAMAS


**Crear etiqueta**
`git show <nombretiqueta>`
`git tag -a V1 -m "Etiqueta V1"`   # Crea una etiqueta anotada llamada "V1" 
`git show V1`               # Esto mostrará los detalles asociados con la etiqueta "V1"
`git tag`                   # Etiquetas existentes 


**Clonar Repositorio**
`git clone https://github.com/lugosi92/practica_evaluable.git practica_evaluable_2`


**Provocar conflicto**

**Clonar Repositoiro**
`git clone <url repositorio remoto>`

**Cambiar a rama 2**
`git branch pruebas2`
`git checkout pruebas`

**Crear LÍNEA 1 en archivo creado**
`echo "Creo archivo en pruebas2" > archivo.txt`

**Crear LÍNEA 2**
`echo "Añado otro texto" >> archivo.txt`

**VALIDAMOS (Añadir a área de trabajo)**
`git add archivo.txt`

**Agregar comentario**
`git commit -m "Creando archivo.txt en la rama pruebas2 "`

**Ver histórico ( ver si se ha creado )**
`git log --oneline`

**Cambiar a MASTER**
`git checkout master`

**Creamos un archivo con el mismo nombre**
`git checkout master`

**Creamos Líneas nuevas**
`echo "Creo archivo.txt en master" > archivo.txt`

**Validamos**
`git commit -m "Creado archivo.txt en master"`
`git log --oneline`

**git merge mirama (desde master)**
`git merge mirama`

• En master fusiono, aparece el conflicto. Dos ramas con el mismo nombre indica que hay conflicto al añadir el archivo.txt. 

**RESOLVER**
Abrir archivo.txt—> borrar las líneas que no queremos 
Validar


**Sincronizar Repositorio**
`git push origin main`

**Etiquetas**
`git tag -a nombre_de_etiqueta -m "Mensaje de la etiqueta"`
`git tg -d <nombre_de_la_etiqueta>`
`git show -nombre_etiqueta-`
`git push origin –tags`   # Manualmente al repositorio



 
