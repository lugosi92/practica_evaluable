### 1.**Directorios y Ficheros (Crear repositorio)**
```bash 
`echo "Contenido del archivo" > archivo.txt` → Añade texto y lo crea
- `touch archivo.txt`       # Crea un documento
- `mkdir carpeta`        # Crea un directorio
- `git init`               # Inicia un repositorio


### 2.**Validar repositorios**
- `git status`             # Estado actual del repositorio
- `git add .`              # Agrega todos los archivos modificados
- `git status`           # Estado actual del repositorio
- `git commit -m "Comentario"`  # Confirma los cambios realizados en los archivos (HEAD, apunta al último commit)

### 3.**Versiones creadas**
- `git log --oneline  `    # Muestra el historial de commits de manera resumida
- `git log`                # Más extenso
- `git show `              # Ver cambio en todos los commits
- `git show idCommit `     # Muestra un commit concreto


### 4.**Comparar cambios**
- `git diff`               # Compara el área de working y el commit que llamamos HEAD.
- `git diff HEAD~1 HEAD`   # Diferencia entre varios commits indicando los apuntadores
- `git diff id HEAD`       # Consultar la diferencia entre varios commits

### 5.**Repositorio remoto**
- `git remote add origin http://github.com/GemaBT/Hola-Mundo.git`
- `git push` 
- `git remote -v`

### 6.**Crear copia con checkout**
- `git init`
- `git remote add origin <nombre-repositorio-remoto>`
- `git fetch origin master`
- `git checkout origin/master`

### 7.**Revertir resetear commits**
- `git reset --hard HEAD~1`    # Resetea el estado de tu directorio de trabajo y el área de preparación al estado del último commit de la rama en la que te encuentras
- `git revert HEAD`            # Para revertir el último commit en Git

### 8. **Conectar con Git Hub**
- `git remote add origin https://github.com/lugosi92/practica_evaluable.git`
- `git push -u origin master`
- `git push origin master`    # Sincronizar con el repositorio remoto
- `git push -u origin master`  # La rama como local actual
- `git pull origin main`      # Actualizar rama


### 9. **Crear rama y cambiar a ella**
`git branch`               # Consultar ramas
`git branch mirama`
`git checkout mirama`      # Puede ser con directorios, ficheros, etc.
`git checkout -b`          # Para cambiara ella directamente

### 10. **Validar**
- `git merge mirama`         # Fusionar ramas 
- `git branch -d mirama`     # BORRAR RAMAS


### 11.**Crear etiqueta**
- `git show <nombretiqueta>`
- `git tag -a V1 -m "Etiqueta V1"`   # Crea una etiqueta anotada llamada "V1" 
- `git show V1`               # Esto mostrará los detalles asociados con la etiqueta "V1"
- `git tag`                   # Etiquetas existentes 


### 12.**Clonar Repositorio**
- `git clone https://github.com/lugosi92/practica_evaluable.git practica_evaluable_2`


### 13.**Provocar conflicto**

 ### 13.1**Clonar Repositoiro**
   - `git clone <url repositorio remoto>`

 ### 13.2**Cambiar a rama 2**
 - `git branch pruebas2`
 - `git checkout pruebas`

 ### 13.3**Crear LÍNEA 1 en archivo creado**
 - `echo "Creo archivo en pruebas2" > archivo.txt`

 ### 13.4**Crear LÍNEA 2**
 - `echo "Añado otro texto" >> archivo.txt`

 ### 13.5**VALIDAMOS (Añadir a área de trabajo)**
 - `git add archivo.txt`

 ### 13.6**Agregar comentario**
 - `git commit -m "Creando archivo.txt en la rama pruebas2 "`

 ### 13.7**Ver histórico ( ver si se ha creado )**
 - `git log --oneline`

 ### 13.8**Cambiar a MASTER**
 - `git checkout master`

 ### 13.9**Creamos un archivo con el mismo nombre**
 - `git checkout master`

 ### 13.10**Creamos Líneas nuevas**
 - `echo "Creo archivo.txt en master" > archivo.txt`

 ### 13.11**Validamos**
 - `git commit -m "Creado archivo.txt en master"`
 - `git log --oneline`

 ### 13.12**git merge mirama (desde master)**
 - `git merge mirama`

• En master fusiono, aparece el conflicto. Dos ramas con el mismo nombre indica que hay conflicto al añadir el archivo.txt. 

**RESOLVER**
Abrir archivo.txt—> borrar las líneas que no queremos 
Validar


### 14 **Sincronizar Repositorio**
- `git push origin main`

### 15 **Etiquetas**
- `git tag -a nombre_de_etiqueta -m "Mensaje de la etiqueta"`
- `git tg -d <nombre_de_la_etiqueta>`
- `git show -nombre_etiqueta-`
- `git push origin –tags`   # Manualmente al repositorio



 
