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
- Colgando del directorio creado en el paso anterior, crea un fichero mediante el comando cat que contenga los treinta primeros números impares (1, 3, 5,..., 57, 59) (cada uno en una línea distinta).
~~~
cat > nombreFichero
1
3
5
...
~~~
Hay que ir añadiendo todos a mano y pulsar Control + D al terminar para guardar los cambios.
> Nota: También podemos cancelar los cambios con Control + C en caso de equivocarnos.
- Visualiza las cinco últimas líneas del fichero creado anteriormente.
~~~
tail -5 nombreFichero
~~~
- Visualiza las trece primeras líneas del fichero anterior.
~~~
head -13 nombreFichero
~~~
- Visualiza página a página el contenido del fichero creado en el paso b).
- Visualiza el directorio de trabajo actual y si no corresponde con tu directorio de inicio cámbiate a este.
- Sin cambiar de directorio, modifica el nombre del fichero creado en el paso b) y dale como nuevo nombre impares.
- Crea otro fichero mediante el comando cat que contenga tu nombre y apellidos en distintas líneas. 
- Mueve este último fichero para que cuelgue del directorio creado en el paso a).
- Crea otro directorio que cuelgue del que se creó en el paso a).
- Haz una copia de los ficheros creados en los pasos b) y h) en el último directorio que has creado.
- Haz que tu directorio de trabajo actual coincida con tu directorio de inicio.
- Desde tu directorio de inicio, visualiza un listado largo y recursivo del directorio creado en el paso a).
- Elimina, pidiendo confirmación, los ficheros que cuelgan del directorio creado en el paso j).
- Desde tu directorio de inicio elimina de forma recursiva el directorio creado en el paso a)..
- Consulta en el manual de usuario el comando date determinando el formato que presenta para la hora y fecha. 

