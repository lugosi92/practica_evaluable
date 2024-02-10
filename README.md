Directorios y Ficheros
echo "Contenido del archivo" > archivo.txt —> Añade texto y lo crea
touch archivo.txt —> Crea documento 
mkdir carpeta—> Crea directorio

Validar repositorios
Git status—> Estado actual del repositorio
Git add . —> Agregar todos los archivos modificados
Git status—> Estado actual del repositorio
Git comió -m “Comentario”—> Se utiliza en Git para confirmar los cambios realizados en los archivos 
git log --oneline —> Muestra el historial de commits de manera resumida

Revertir resetear commits
git reset --hard HEAD~1—>resetea el estado de tu directorio de trabajo y el área de preparación al estado del último commit de la rama en la que te encuentras
Git revert HEAD—> Para revertir el último commit en Git

Conectar con Git Hub
Git remote add origin https://github.com/lugosi92/practica_evaluable.git
Git push -u origin master
git push origin master—> Sincornizar con el repositorio remoto

Crear rama y cambiar a ella
Git branch —> consultar ramas
Git branch mirama
Git checkout mirama
Git checkout -b —> para cambiara ella directamente
//Validar
Git merge mirama—> fusionar ramas 
git branch -d mirama —> BORRAR RAMAS

Crear etiqueta
Git tag -a V1 -m “Etiqueta V1”—>  crea una etiqueta anotada llamada "V1" 
Git show V1—> Esto mostrará los detalles asociados con la etiqueta "V1", 
git tag—> etiquetas existentes

Clonar Repositorio
Git clone https://github.com/lugosi92/practica_evaluable.git practica_evaluable_2
