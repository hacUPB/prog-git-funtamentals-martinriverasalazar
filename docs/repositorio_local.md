## Pasos para crear un repositorio local con Git
**1 Abrir la terminal**

Primero, abre la consola o terminal y navega hasta la carpeta donde quieres crear el repositorio.

cd ruta/del/directorio  


Si quieres crear una carpeta nueva para el proyecto:

mkdir mi_proyecto
cd mi_proyecto

**2 Inicializar el repositorio Git**

Dentro de la carpeta del proyecto, ejecuta el comando:

git init


~~¿Qué hace este comando?~~

Crea una carpeta oculta llamada .git

Esa carpeta contiene toda la información del control de versiones

A partir de este momento, el directorio ya es un repositorio Git

La terminal mostrará un mensaje similar a:

Initialized empty Git repository in /mi_proyecto/.git/

**3 Ver el estado del repositorio**

Para comprobar que Git está funcionando correctamente:

git status


Este comando muestra:

Archivos sin seguimiento (untracked)

Archivos listos para guardar cambios

Confirmaciones pendientes

**4 Crear archivos en el repositorio**

Puedes crear archivos normalmente, por ejemplo:

touch README.md


Luego verifica el estado:

git status


Git indicará que el archivo aún no está siendo seguido.

**5 Agregar archivos al área de preparación (staging)**

Para indicarle a Git qué archivos quieres guardar:

git add README.md


O para agregar todos los archivos:

git add .

6️⃣ Guardar los cambios (commit)

Finalmente, se realiza un commit, que es como tomar una “foto” del estado actual del proyecto:

git commit -m "Primer commit del proyecto"


📌 El mensaje del commit debe describir brevemente qué cambios se hicieron.
