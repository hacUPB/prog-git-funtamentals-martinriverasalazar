"""
PROCESO PARA CREAR UN REPOSITORIO REMOTO EN GITHUB
Y SINCRONIZARLO CON UN REPOSITORIO LOCAL USANDO GIT

=================================================
1. CREAR EL REPOSITORIO REMOTO EN GITHUB
=================================================

1. Ingresar a https://github.com y iniciar sesión.
2. Hacer clic en el botón "New repository".
3. Completar los datos:
   - Repository name: nombre_del_repositorio
   - Description (opcional)
   - Elegir Public o Private
   - NO marcar "Initialize this repository with a README"
4. Hacer clic en "Create repository".

GitHub mostrará la URL del repositorio, por ejemplo:
https://github.com/usuario/nombre_del_repositorio.git


=================================================
2. CREAR O USAR UN REPOSITORIO LOCAL
=================================================

En la terminal, ubicarse en la carpeta del proyecto:

    cd ruta/del/proyecto

Si el repositorio local NO existe:
    
    git init

Esto crea el repositorio local y la carpeta oculta .git


=================================================
3. AGREGAR ARCHIVOS AL REPOSITORIO LOCAL
=================================================

Ver el estado del repositorio:

    git status

Agregar archivos al área de preparación (staging):

    git add .

Guardar los cambios con un commit:

    git commit -m "Primer commit"


=================================================
4. CONECTAR EL REPOSITORIO LOCAL CON GITHUB
=================================================

Agregar el repositorio remoto usando la URL de GitHub:

    git remote add origin https://github.com/usuario/nombre_del_repositorio.git

Verificar que el remoto fue agregado correctamente:

    git remote -v


=================================================
5. ENVIAR LOS CAMBIOS AL REPOSITORIO REMOTO
=================================================

Subir los commits al repositorio remoto:

    git branch -M main
    git push -u origin main

Esto sincroniza el repositorio local con GitHub.


=================================================
6. FLUJO BÁSICO DE TRABAJO POSTERIOR
=================================================

Cada vez que haya cambios:

    git status
    git add .
    git commit -m "Descripción de los cambios"
    git push


=================================================
RESUMEN DE COMANDOS CLAVE
=================================================

git init               -> Inicializa repositorio local
git status             -> Muestra el estado del repositorio
git add .              -> Agrega archivos al staging
git commit -m "msg"    -> Guarda cambios
git remote add origin  -> Conecta con GitHub
git push               -> Envía cambios al repositorio remoto
"""

