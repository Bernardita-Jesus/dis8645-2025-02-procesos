# Proyecto 02

## Grupo-05 "Waos" : Integrantes

- [Morgan Aravena Arze](https://github.com/Mosswhosmoss)
- [Aileen Guiselle D'Espessailles Rojas](https://github.com/aileendespessailles-design)
- [Carla Andrea del Carmen Pino Barrios](https://github.com/Coff4)
- [Sebastián Alejandro Sáez Olivares](https://github.com/SebastianSaez1003)

## Presentación textual 

### Introducción

El proyecto, de manera general, consiste en hacer una máquina saludadora.

Para la ideación del proyecto usamos la propuesta de [SebastianSaez1003](https://github.com/SebastianSaez1003), que quería usar un servomotor desde el semestre pasado.

Nuestro proyecto se centra en desarrollar un robot que te salude dependiendo de la temperatura.

El saludo se define como ["Un acto comunicacional (entre humanos), en el que una persona hace notar a otra su presencia" - Wikipedia](https://es.wikipedia.org/wiki/Saludo). 

En nuestro caso, los sensores serían un sensor de temperatura, humedad y presión y un sensor ultrasónico, y los actuadores, dos servomotores y una pantalla. 

### Friolin

Friolin, nuestro robot friolento, funciona con un sensor ultrasónico HC-SR04, que usaremos para detectar si hay o no hay alguien frente al robot; un sensor DHT11, que es de temperatura, humedad y presión; en nuestro caso solo utilizaremos la función de temperatura; una pantalla OLED SSD1306, para mostrar una retroalimentación visual con características faciales; y un servomotor, para que cometa el acto de saludar con el brazo.

**paso a paso del proyecto**

1. Máquina inicia en estado neutro
2. Si no detecta a nadie se mantiene en este estado, en donde ambas manos estarán en suspensión y en la pantalla no se mostrará nada
3. Si detecta a una persona, se esperan 3 segundos para actuar según la temperatura medida en el ambiente
4. Si la temperatura es menor o igual a (15) grados celsius, el servomotor no actuará y mostrará en display un mensaje del porqué no quiere saludar, además de una expresión facial importada a través del Arduino que se puede observar en el display
5. Si la temperatura es mayor a (15) grados celsius, el servomotor actuará para dar el saludo (donde su "brazo" se moverá de lado a lado entre los grados 135 y 45 para simular un saludo de mano como lo realizaría un humano) y se mostrará en display un mensaje de texto para saludar, junto a una expresión facial.
6. El ciclo del saludo se repetirá 3 veces y el mensaje durará 15 segundos en la pantalla
7. La persona al retirarse hará que la máquina vuelva a su estado neutro.

**Mapa de flujo**


### Desarrollo

Para poder programar a friolin de manera más fácil partimos con el desarrollo del pseudocódigo donde se separaron las funciones de cada sensor y actuador  en archivos .h y .cpp para que el archivo .ino quedará todo ordenado, se partió con la ideación de los parámetros de cada sensor sensor, para poder comenzar con la investigación exacta de que queríamos hacer.
En este punto del pseudocódigo también se definieron las clases, donde, con la ayuda de Aarón Moraga pudimos definir cada una de las acciones que queríamos que se desarrollaran.

(Las clases se hicieron en el archivo .cpp y los parámetros en .h)

Luego de ver todos los parámetros nos separamos por investigación de sensor/actuador y por la persona que uniría todo en el código madre.

### Avances de pseudocódigo

#### Pseudocódigo V0

En esta versión del pseudocodigo se hizo la separacion de tabs dentro del archivo, por el momento solo con archinos .ino

![carpeta pseudocodigo](imagenes/pseudocodigoV0.png)

#### Pseudocódigo V0_1_4

Esta es la versión final del pseudocódigo, hay muchos errores y con la ayuda de Aaron Montoya Moraga empezamos a ordenar y resumir los archivos  llegando a la primera versión de codigoRobotFriolento.INO 

#### codigoRobotFriolento_0_1_0



### Comentarios finales








