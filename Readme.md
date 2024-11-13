
HTTPS: https://github.com/ZuleimaMunozJimenez/GIT-IA.git

Alumno 1: Zuleima Muñoz
Alumno 2: Alejandro Cabo


Comandos usados:

- git clone
- git add
- git commit
- git push


Para resolver los ejercicios hasta ahora realizados como alumna 1 he empleado:

- git config --global user.name 'MiNombre' : Para evitar problemas con las credenciales de mi cuenta de 
GitHub.
- git config --global user.email 'MiEmail' : Por la misma razón que el anterior.
- git init : Para inicializar el repositorio.
- git status : Para comprobar el estado del repositorio después de haber añadido los archivos de Farmacia.
- git add . : Para añadir los ficheros al área de preparación.
- git commit -m 'Inicialización del repositorio con archivos Farmacia' : Para registrar los cambios en el repositorio.
- git remote add origin https://github.com/ZuleimaMunozJimenez/GIT-IA.git : Para inicializar el repositorio remoto creado en GitHub anteriormente.
- git remote : Para revisar si hemos agregado el remote correctamente.
- git push origin master : Para enviar los archivos a GitHub. Para que funcione hemos tenido que crear un token desde GitHub para iniciar sesión.
- git pull origin master : Para actualizar los datos modificados por alumno 2.
- Vamos a volver a usar nuevamente _git add ._ , _git commit -m 'Actualización README'_
- git push origin master : Para subir los cambios realizados.

7.
<<<<<<< HEAD
- git branch "nombreRama" para crear una rama
- git branch -m "ramaActual" "ramaNueva" para cambiar el nombre de la rama

8.
- Al usar git branch nos muestra el listado de las ramas en ella vemos un asterisco que nos indica en que rama estamos, en este caso, rama master

=======
- git checkout master para comprobar si estamos en la rama master
- git checkout -b "nombreRama" para crear y moverse a esa rama

8.
- El asterisco que aparece es para indicarnos la rama en la que estamos situados, en nuestro caso aparace en la rama master

9
- En el apartado 9 ambos alumnos creamos los dos ficheros

10
- Usamos el comando git fetch origin que actualiza los ultimos cambios en remoto
- Y git diff origin/master..ramaAlumno2 para comprobar la diferencia entre la rama master y la nuestra.

11.
- git merge 'nombreRama' : Para fusionar la rama master con nuestra rama de trabajo.
- git push origin master : Para subir al repositorio remoto los cambios.

Los dos no hemos podido realizar los mismos pasos. Porque al hacer push el segundo, nos da un error sobre que hay contenido que no está en el repositorio local.
Por eso, hacemos git pull origin master para traer los cambios y posteriormente el push para subir los nuestros.


12.
Para solucionar el problema tedioso de la solicitud constante de credenciales hacemos uso de git config --global credential.helper store . Esto hace que al ejecutar otro push o pull guarde las credenciales en texto plano y no vuelve a solicitarnosla.


