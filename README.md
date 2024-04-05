# Curso JAVA Udemy
## Pasos para replicar este proyecto

1. Clonar este repositorio en la carpeta donde vayamos a trabajar con él, sirva como ejemplo _xampp/htdocs/_:

    ``` git clone https://github.com/GMVIT/PlataformaAgencias.git ```
    
2. Lo ideal es trabajar sobre una rama distinta que parta desde master / main, por ello en el momento que vayamos a comenzar un nuevo desarrollo crearíamos una nueva:

    ``` git checkout -b nombre_de_la_nueva_rama ```

3. ### Modificación de archivos ### 
- Si tenemos actualizado nuestro repositorio local (nube) (frente a lo que tenemos en repositorio remoto (PC), que sería este en Github),
nos aseguraríamos con el commando ``` git pull ```, que traería los últimos cambios en el repositorio / rama si los hubiera. 
- Si modificamos algún archivo, con ``` git status ``` comprobaremos cuáles han sido modificados, añadidos o eliminados.
- Si queremos ver, además, qué cambios se han realizado de manera más minuciosa, utilizaremos el comando ``` git diff ```, que nos irá mostrando uno a uno los cambios realizados.
- Para "añadir" los cambios, debemos añadir los archivos que hayan sido añadidos, modificados o eliminados con la intrucción ``` git add nombredelarchivo ```; en la medida de lo posible
evitaremos usar el comando ``` git add . ``` ya que nos interesaría controlar en cada momento qué archivos se están cambiando.
- Tras añadir, con la intrucción anterior, los archivos pendientes, debemos realizar la acción del commit, que es lo que designa qué
vamos a preparar para la subida. La sintaxis es la siguiente:
``` git commit -m "Mensaje descriptivo" ```

Tras esto, si hacemos un ``` git status ``` nuevamente nos mostrará en consola qué tenemos preparo para subir. Una vez nos aseguremos que está todo correcto
debemos subir los cambios a remoto (hacer push), con la siguiente sintaxis: 
``` git push origin nombredelarama ``` 

_ejemplo: ``` git push origin feature/PA-240_ ``` --> donde feature/PA-240 sería un ejemplo de una nueva funcionalidad (feature) seguido de PA (PlataformaAgencias) y un número (ID).

