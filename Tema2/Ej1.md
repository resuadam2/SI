# Ejercicio 1. Partiendo de tu directorio de inicio, realiza cada uno de los siguientes apartados:
- Crea un directorio que cuelgue de tu directorio de inicio.

Para posicionarse en el directorio de inicio:
~~~
cd 
~~~
Para crear el directorio:
~~~
mkdir nombreCarpeta
~~~
> Nota: el nombre de la carpeta puede ser cualquiera admitido por el sistema.
- Colgando del directorio creado en el paso anterior, crea un fichero mediante el comando cat que contenga los treinta primeros números impares (1, 3, 5,..., 57, 59) (cada uno en una línea distinta).
~~~
cat > nombreCarpeta/nombreFichero
1
3
5
...
~~~
Hay que ir añadiendo todos a mano y pulsar Control + D al terminar para guardar los cambios.
> Nota: También podemos cancelar los cambios con Control + C en caso de equivocarnos.
> Nota: usamos la **ruta relativa** al fichero para crearlo dentro de la carpeta creada en el anterior ejercicio.
> Nota: El nombre del fichero puede ser cualquiera admitido por el sistema.
- Visualiza las cinco últimas líneas del fichero creado anteriormente.
~~~
tail -5 nombreFichero
~~~
- Visualiza las trece primeras líneas del fichero anterior.
~~~
head -13 nombreFichero
~~~
- Visualiza página a página el contenido del fichero creado en el paso b).
~~~
more nombreFichero
~~~
- Visualiza el directorio de trabajo actual y si no corresponde con tu directorio de inicio cámbiate a este.

Para visualizar el directorio de trabajo actual:
~~~
pwd
~~~
Para volver al directorio de inicio:
~~~
cd
~~~
- Sin cambiar de directorio, modifica el nombre del fichero creado en el paso b) y dale como nuevo nombre impares.
~~~
mv nombreCarpeta/nombreFichero nombreCarpeta/impares
~~~
> Nota: Sin movernos del directorio de inicio, usamos la **ruta relativa** al fichero creado para con el comando mv cambiarle el nombre, dándole la misma ruta pero con un nombre de fichero distinto en el segundo argumento enviado al comando
- Crea otro fichero mediante el comando cat que contenga tu nombre y apellidos en distintas líneas. 
~~~
cat > ficheroNombre
Nombre
Apellido1
Apellido2
~~~
Salimos de la edición con Control + D de nuevo para guardar los cambios
- Mueve este último fichero para que cuelgue del directorio creado en el paso a).
~~~
mv ficheroNombre nombreCarpeta/ficheroNombre
~~~
- Crea otro directorio que cuelgue del que se creó en el paso a).
~~~
mkdir nombreCarpeta/subCarpeta
~~~
> Nota: Nótese que *nombreCarpeta* hace referencia a la carpeta creada en el primer paso y *subCarpeta* a la carpeta que generamos en este.
- Haz una copia de los ficheros creados en los pasos b) y h) en el último directorio que has creado.
~~~
cp nombreCarpeta/impares ficheroNombre nombreCarpeta/subCarpeta
~~~
> Nota: Al comando cp para copiar podemos pasarle uno o más archivos, como en este caso, siempre y cuando el último argumento sea un directorio destino dónde copiar los archivos anteriores.
- Haz que tu directorio de trabajo actual coincida con tu directorio de inicio.
~~~
cd
~~~
- Desde tu directorio de inicio, visualiza un listado largo y recursivo del directorio creado en el paso a).
~~~
ls -lR nombreCarpeta
~~~
> Nota: Con la opción -l hacemos que el listado del comando *ls* sea largo y con la opción -R hacemos que sea recursivo, es decir, que no solo nos muestre lo que hay en la carpeta que le mandamos como argumento(s) si no también lo que hay dentro de las carpetas que están dentro de ella y así sucesivamente.
- Elimina, pidiendo confirmación, los ficheros que cuelgan del directorio creado en el paso j).

Primero nos posicionamos en la carpeta:
~~~
cd nombreCarpeta/subCarpeta
~~~
Ahora, borramos todos los ficheros que hay en ella:
~~~
rm -i *
~~~
> Nota: También podríamos ir pasandole los archivos uno por uno separados por espacios. Con la opción -i pedimos confirmación.
- Desde tu directorio de inicio elimina de forma recursiva el directorio creado en el paso a)..

Nos volvemos a mover al directorio de inicio:
~~~
cd
~~~
Ahora borramos todo el directorio de forma recursiva con la opción -R:
~~~
rm -R nombreCarpeta
~~~
- Consulta en el manual de usuario el comando date determinando el formato que presenta para la hora y fecha. 
~~~
man date
~~~
> Nota: Es posible que nos falle si el comando date no está instalado, si fuese necesario instalarlo antes tendriamos que usar el siguiente comando:
~~~
apt get install date
~~~
