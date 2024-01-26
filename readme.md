1. Crear un repositorio en local

Abre tu terminal y navega hasta el directorio donde deseas crear el repositorio.
    Uso el comando cd hasta llegar a la carpeta lemoncode.
Crea una carpeta con el nombre del repositorio.
    mk dir LaboratorioGit
Ingresa a la carpeta que acabas de crear.
    cd \LaboratorioGit\
Inicializa el repositorio de Git
    git init

2. Subir el repositorio a GitHub

Crea un nuevo repositorio en GitHub.
    GitHub/Home/Nuevo repositorio/indicamos el nombre, público/privado y si queremos readme
Copia el URL del repositorio que acabas de crear en GitHub
    https://github.com/kike-nine/LaboratorioGit
Conecta tu repositorio local con el repositorio en GitHub.
    git add .
    git commit -m "archivo readme con la explicación"
    git remote add origin git@github.com:kike-nine/LaboratorioGit.git
    git push --set-upstream origin master
Verifica que la conexión se haya establecido correctamente.
    Se ha subido correctamente en GitHub en la rama master.

3. Hacer un commit y un push

Crea un archivo en la carpeta del repositorio.
    Hola.html
Añade el archivo al staging.
    "git add ." y luego "git status" para comprobar si el arhivo está listo para hacer commit.
Crea un commit con un mensaje descriptivo.
    git commit -m "Haciendo el commit del archivo Hola.html"
    git status para comprobar que se ha realizado correctamente.
Sube los cambios al repositorio en GitHub.
    git push (cambio realizado con existo en GitHub).