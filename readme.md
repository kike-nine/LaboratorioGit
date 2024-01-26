**1. Crear un repositorio en local**

Abre tu terminal y navega hasta el directorio donde deseas crear el repositorio.
    >Uso el comando cd hasta llegar a la carpeta lemoncode.
Crea una carpeta con el nombre del repositorio.
    >mk dir LaboratorioGit
Ingresa a la carpeta que acabas de crear.
    >cd \LaboratorioGit\
Inicializa el repositorio de Git
    >git init

**2. Subir el repositorio a GitHub**

Crea un nuevo repositorio en GitHub.
    >GitHub/Home/Nuevo repositorio/indicamos el nombre, público/privado y si queremos readme
Copia el URL del repositorio que acabas de crear en GitHub
    >https://github.com/kike-nine/LaboratorioGit
Conecta tu repositorio local con el repositorio en GitHub.
    >git add .
    >git commit -m "archivo readme con la explicación"
    >git remote add origin git@github.com:kike-nine/LaboratorioGit.git
    >git push --set-upstream origin master
Verifica que la conexión se haya establecido correctamente.
    >Se ha subido correctamente en GitHub en la rama master.

**3. Hacer un commit y un push**

Crea un archivo en la carpeta del repositorio.
    >Hola.html
Añade el archivo al staging.
    >"git add ." y luego "git status" para comprobar si el arhivo está listo para hacer commit.
Crea un commit con un mensaje descriptivo.
    >git commit -m "Haciendo el commit del archivo Hola.html"
    >git status para comprobar que se ha realizado correctamente.
Sube los cambios al repositorio en GitHub.
    >git push (cambio realizado con existo en GitHub).

**4. Crear una rama**

Crea una rama nueva llamada "development".
    >git branch development
Cambia a la nueva rama.
    >git checkout development
Realiza algunos cambios en el archivo que creaste.
    >Cambio el <h1> del archivo Hola.html 
Añade y haz un commit con los cambios en la rama "development".
    >git add .
    >git commit -a -m "cambiando el título de Hola"
Sube los cambios a Github.
    >git push --set-upstream origin development

**5. Hacer un merge**

Vuelve a la rama "main".
    >git checkout master
Haz un merge de la rama "development" a la rama "main".
    >git merge development
Si no hay conflictos, los cambios realizados en la rama "development" se incorporarán a la rama "main".
    >Updating 09b8fee..79d0ad2
    >Fast-forward
    > Hola.html |  2 +-
    > readme.md | 19 +++++++++++++++++--
    > 2 files changed, 18 insertions(+), 3 deletions(-) 
Haz un push de los cambios al repositorio en GitHub.
    >git push
