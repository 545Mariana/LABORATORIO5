# LABORATORIO5


Objetivo de la practica:

El objetivo del siguiente codigo es implementar un contador binario en el µC Cortex M3 a traves del uso de leds y dos botones. Al presionar el primero de los botones el contador ira aumentando, al apretar el segundo boton el contador ira decrementando, por ultimo, si los dos botones son apretados al mismo tiempo el contador se reiniciara.

#Desarrollo:
Para desarrollar lo antes mencionado tendramos los siguientes archivos
#Archivos con extension S
Los archivos contienen el codigo ensamblador ARM. Los codigos dentro de estos archivos los declaramos como variables globales para que al ser llamados en otras funciones puedan ser utilizadas.

La funcion main es la que contiene el codigo donde se configuraran los puertos de entrada y salida. En ella se utilizan otras funciones como read_button, output, digital_read que son las que configuran los pines y botones.

En el archivo output para configurar al menos 10 LEDS debemos cargar el numero exadecimal en nuevo registro para asi con AND  habilitar los puertos que queremos configurar.

Para grabar nuestro código en nuestra blue pin debemos ingresar en la terminal "make" que hara que se generen los arvhivos .o .
Al tener los archivos .o aplicamos el otro comando que es make write que sera el que grabe en nuestra blue pin.

![Captura desde 2023-05-26 14-51-52](https://github.com/545Mariana/LABORATORIO5/assets/109254012/f4088cd8-fecc-4ea1-a2cd-2498aa18aeb9)

