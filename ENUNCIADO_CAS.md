# PASOS A SEGUIR:
1. Abrimos una consola de comandos (en windows ejecutamos el orden cmd)
1. En nuestro disco local, vamos a la carpeta donde tenemos nuestros desarrollos
    En mi caso `c:\ Users\mviel\2020-React\`
1. nos descargamos el que tenemos en el repositorio remoto (en GitHub) creado por el profesor, es decir
  vamos a *Clonar* ese repositorio:
   `git clone url_del_repositorio`
1. ya tenemos una copia del repositorio remoto en la máquina local. *NO CERRAMOS LA CONSOLA DE ÓRDENES !!*

A partir de ahora trabajaremos en local y subiremos los cambios en el repositorio remoto.
1. Modificamos, en local, el archivo README.md para añadirle
    - Tu nombre con una cabecera (Header) de tamaño 1
    1. Subiréis los cambios a GitHub, para ello,
        - Guarda el archivo README.md modificado (ctrl + s)
        - Añade los cambios en el Stage Area
        - haz un commit con el comentario "añado mi nombre"
        - después haz un push
        - refrescar la página del navegador donde tenemos el repositorio remoto en GitHub, para comprobar los cambios.
1. Añadiremos el archivo README.md una lista con 3 cosas que nos gustaría conseguir al finalizar el Ciclo/curso.
    1. Subiréis los cambios a GitHub
        - - Guarda el archivo README.md modificado (ctrl + s)
        - Añade los cambios en el Stage Area
        - haz un commit con el comentario "añado lista cosas fin ciclo/curso"
        - después haz un push
        - refrescar la página del navegador donde tenemos el repositorio remoto en GitHub, para comprobar los cambios
1. Descargaremos de internet el logo de GitHub y lo guardaremos en nuestro repositorio local
    1. añadiremos esa imagen al stage Area, para subirla a nuestro repositorio remoto
        - Añade el archivo de la imagen del logo en el Stage Area
        - haz un commit con el comentario "añado el logo de GitHub"
        - después haz un push
1. Modificaremos el archivo README.md para que nos muestre el logo de GitHub
    - Guarde el archivo (ctrl + s)
    - Añadiremos los cambios en el Stage Area
    - haz un commit con el comentario "añado logo GitHub"
    - después haz un push
    - refrescar el navegador que tenemos en GitHub, para comprobar los cambios
1. Añadiremos el texto: `Ya hemos practicado con GitHub`, en el dichero README.md
    - Seguiremos las acciones habituales

1. Deshaciendo el último cambio subido a GitHub.
    - Imagínese que modifique una/unos archivos para implementar una mejora.
    Ha guardado los cambios, y los ha subido a GitHub. Pero prueba la app y ahora falla más que antes.
    Por tanto decide dejarlo todo como estaba, antes de los últimos cambios realizados. 

    Es decir, *vamos a deshacer la última acción realizada* antes (el punto 5).
    - desde la consola de comandos revisamos los últimos 10 commits que hemos hecho.
        1. ejecutaremos la orden: `git log -10`
            - tomaremos el identificador del commit que queremos restaurar (véase imagen llistat_commits.png)! [Listado de Commits] (./ llistat_commits.png)
        1. ejecutaremos la orden:
           - `git reset --hard <identificador_del_commit>`
        1. enviaremos los cambios a la rama master del repositorio remoto (GitHub):
           - `git push origin HEAD: master --force`
