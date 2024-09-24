# Bases de Datos NoSQL

## Origen

El origen de las bases de datos no relacionales se remonta a finales de la década de los 90, cuando Carlos Strozzi lo usó por primera vez para referirse a su base de código abierto la cual no ofrecía un lenguaje SQL. 

A pesar de esto, el término no adquirió popularidad hasta 2009 gracias a un empleado de la empresa Rackspace quien lo empleó para descubrir y distribuir una nueva generación de bases no relacionales.

## Nivel de Adopción

El motivo principal de que aumentara su empleabilidad fue ocasionado por la llegada del Big Data, con la necesidad de sistemas capaces de manejar cantidades grandes de información no estructurada (mensajes en redes sociales, imágenes, datos, etc). El sistema de las bases NoSQL resultó ser muy eficiente para gestionar esta clase de datos al ser más eficiente que las estructuras rígidas de las bases relacionales. 

## Ventajas

1. Son más flexibles para elaborar esquemas de información
2. Fácilmente escalables horizontalmente, utilizadas para trabajar con grandes volúmenes de información
3. Su rendimiento es alto debido a que se han preparado para trabajar con patrones y modelos de datos específicos
4. Gracias a sus API exclusivas y la proporción de modelos creados para gestionar los distintos tipos de datos se han convertido en un sistema de almacenamiento muy funcional

## Inconvenientes

1. Son incompatibles con las consultas realizadas en lenguaje SQL
2. No tienen un sistema estandarizado
3. No poseen el soporte que puede proporcionar una empresa comercial al ser de código abierto
4. Suelen tener problemas de compatibilidad dado que no comparten un estándar

## Descripción del Funcionamiento

Las bases de datos no relacionales se emplean para almacenar datos no estructurados, de los que no se tiene ninguna información predefinida. Sin embargo, también se pueden utilizar para el almacenamiento y gestión de datos estructurados. En el ejemplo de una base de datos en la que se almacenarán DVDs de películas, estos podrían almacenarse en cuanto al título, fecha de estreno, género y director. 

En el caso de las bases de datos no relacionales, cada registro de una película se almacena como un único documento JSON. Todas se almacenan en un solo documento, es decir, que este almacenamiento nos ayuda a tener mayor escalabilidad horizontal y un desarrollo más intuitivo.

## Tipos

### Clave-valor

En este tipo de bases de datos no relacionales almacena la información en pares formados por una clave y su correspondiente valor. La clave actúa como un identificador único, mientras que el valor contiene los datos asociados. Este modelo es ideal para aplicaciones que requieren rapidez y escalabilidad, como en el caso de videojuegos, dispositivos conectados al Internet de las Cosas (IoT) o sistemas de caché.

### Documentos

En este modelo, los datos se almacenan en forma de documentos, generalmente en formato JSON, lo que ofrece flexibilidad y permite manejar estructuras jerárquicas y semiestructuradas. Esto facilita a los desarrolladores el proceso de almacenamiento, gestión y consulta sin tener que ceñirse a un esquema rígido. Es comúnmente empleado en sistemas de gestión de contenidos y en la administración de perfiles de usuarios.

### Gráficos

Las bases de datos de gráficos están diseñadas para gestionar datos que tienen relaciones complejas. Las entidades se representan mediante nodos y las relaciones entre ellas se modelan con aristas. Este enfoque resulta especialmente útil en redes sociales, motores de recomendación y sistemas dedicados a la detección y prevención de fraudes.

### En memoria

Las bases de datos en memoria están pensadas para ofrecer respuestas extremadamente rápidas, con tiempos de acceso medidos en milisegundos. Son capaces de manejar grandes volúmenes de tráfico, lo que las convierte en una solución ideal para aplicaciones que requieren procesamiento en tiempo real, como clasificaciones en videojuegos o herramientas de análisis de datos en tiempo real.

## Usos

Las bases de datos NoSQL sobresalen en casos donde es necesario manejar una gran cantidad de usuarios distribuidos globalmente, brindando experiencias altamente personalizadas. Este tipo de aplicaciones interactivas se benefician de la flexibilidad y agilidad que ofrecen las bases de datos NoSQL.

Estas bases de datos priorizan la alta disponibilidad, proporcionan un rendimiento constante, escalan horizontalmente de manera rápida sin interrupciones y son capaces de gestionar grandes volúmenes de datos variados.

Estas características hacen que las bases de datos NoSQL sean ideales para aplicaciones que requieren alta escalabilidad, confiabilidad y disponibilidad continua.

Entre los casos de uso más comunes de NoSQL se encuentran:

- Aplicaciones web, IoT y móviles
- Aplicaciones web en tiempo real
- Personalización, recomendaciones y experiencias en tiempo real para los usuarios
- Gestión de inventarios y catálogos
- Detección de fraudes y autenticación de identidad
- Tecnología publicitaria
