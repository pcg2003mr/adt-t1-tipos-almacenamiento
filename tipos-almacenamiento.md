# Tipos de almacenamiento

## Bases de datos no relacionales
### Alumnos que han participado
`Miguel Fernández Vallés y Jorge Fresno Menéndez`
### Origen. ¿Cuándo surgió? ¿Cómo se popularizó?
Surgen como respuesta a las limitaciones que tienen las bases de datos relacionales. Se crean en 1998, no por una empresa o entidad particular si no por diferentes empresas como Google, Amazon, Facebook... y creadores de grandes proyectos open source como MongoDB, Cassandra... solucionando las carencias de las RDBMS.

Comenzaron a ganar relevancia a mediados de la década de 2000, impulsadas por la necesidad de almacenar y procesar grandes volúmenes de datos generados por aplicaciones web 2.0, redes sociales y el Internet de las Cosas (IoT).

### Nivel de adopción
Aunque las bases de datos más usadas siguen siendo las relacionales, las bases de datos no relacionales han aumentado su uso hasta situar a MongoDB como la quinta base de datos más usada. Muchas empresas de todos los tamaños las utilizan para diversas aplicaciones, desde startups hasta grandes corporaciones. La elección de una base de datos NoSQL depende de las necesidades específicas de cada proyecto, como el tipo de datos, el volumen, la frecuencia de acceso y los requisitos de rendimiento.

Estas son las bases de datos más usadas, donde podemos ver a MongoDB en el quinto lugar:
![Bases más usadas](https://learnsql.es/blog/las-bases-de-datos-mas-populares-en-2023/most-popular-databases-2023-3.webp)

### Descripción del funcionamiento del sistema de almacenamiento
En lugar de utilizar tablas y relaciones con las bases de datos relacionales, emplean modelos de datos más flexibles como:

- ***Clave-Valor***: Cada dato se almacena como un par único de clave y valor. Por ejemplo una simple lista de compras donde cada ítem (clave) tiene asociado un valor (cantidad).
- ***Documentos***: Los documentos almacenan datos en un formato similar a JSON, lo que permite estructuras anidadas y flexibles. Esto significa que puedes tener objetos dentro de objetos, creando estructuras de datos más complejas y representativas de la información real.
- ***Columnas***: A diferencia de las bases de datos relacionales que organizan los datos en filas y columnas, las bases de datos de columnas invierten esta lógica. Los datos se organizan en columnas, y cada columna puede tener diferentes tipos de datos.
- ***Gráficos***: Los datos se representan como nodos (entidades) y relaciones (conexiones) entre ellos. Esto permite modelar datos con relaciones complejas y jerárquicas.

### Ventajas e incovenientes
**Ventajas**
1. *Escalabilidad*: Gracias a su escalabilidad horizontal frente a la vertical de las relacionales, en lugar de aumentar la potencial del servidor, puedes agregar más servidores para aumentar la carga de trabajo.
2. *Flexibilidad*: No se limitan a un esquema rígido, permitiendo adaptarse fácilmente a los cambios en datos y nuevos tipos de información.
3. *Rendimiento optimizado*: Al diseñarse para un tipo específico de trabajo, pueden ofrecer un rendimiento superior en ciertas operaciones, como lecturas y escrituras de alta velocidad.
4.  *Economía*: No se necesitan servidores con gran cantidad de recursos para operar.

**Desventajas**
1. *Madurez*: Algunas bases de datos NoSQL aún están en desarrollo y pueden carecer de algunas características o funcionalidades.
2. *Falta de estándares*: : No se tiene un criterio plenamente definido, variando el lenguaje según el tipo de base de datos que se vaya a utilizar.
3. *Complejidad*: La gestión es más compleja que en una base de datos relacional.
4. *Herramientas GUI:*  La mayoría de las bases de datos NoSQL no contienen una interfaz gráfica. Requiere conocimiento especial para poder ejecutarlas.

### Usos
Una base de datos NoSQL es la mejor opción para gestionar datos indeterminados, no relacionados o que cambian rápidamente. Pueden usarse para aplicaciones que cumplan:
+ Necesidad de esquemas flexibles que permitan un desarrollo más rápido e iterativo.
+ Realizar consultas complejas y uniones entre tablas.
+ Exigencia de un escalado horizontal mediante la fragmentación de los servidores.
+ Alto nivel de integridad de los datos y transacciones ACID (atomicidad, coherencia, aislamiento y durabilidad).

### Tipos
#### Bases de datos clave-valor
Son las más sencillas de todas y almacenan datos en una organización de pares de clave y valor. Son las que permiten más altas velocidades en la lectura y escritura de datos y se usan principalmente en sistemas de almacenamiento en caché.

![Clave-valor](https://www.certia.net/wp-content/uploads/2021/03/Clave_Valor.jpg)
#### Bases de datos de documentos
Las bases de datos de documentos almacenan datos en colecciones, siendo los elementos de cada una de esas colecciones documentos que contienen pares clave/valor. Además de también tener un identificador único para cada documento, los campos de los que consta este documento sí son transparentes para el sistema de administración.

![Documentos](https://www.certia.net/wp-content/uploads/2021/03/Documento-JSON.jpg)
#### Bases de datos de columnas anchas
Están pensadas para requerir menos consultas a la hora de recuperar datos puesto que guardan todos los datos relacionados en “grupos”, teniendo cada familia de columnas un conjunto de columnas con una relación lógica entre ellas.

![Columnas](https://www.certia.net/wp-content/uploads/2021/03/Familia-columnas.jpg)
#### Bases de datos orientadas a grafos
Están compuestas por documentos que se relacionan entre sí y que permiten representar relaciones complejas entre los datos y así realizar consultas eficientes a través de los nodos y aristas analizando sus relaciones.

![Grafos](https://www.certia.net/wp-content/uploads/2021/03/Grafos.png)

### Casos de uso reales observados
1. **Redes sociales**

![Redes](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTQKrFhY-ljA-u7J5IMWeTv8zmpBx4PP9nQMw&s)

Facebook utiliza Cassandra para manejar los datos generados por usuarios como comentarios, likes, publicaciones...X utiliza también Cassandra y Storm para procesar en tiempo real los tweets y construir un índice de búsqueda invertido.

2. **Comercio electrónico**

![Comercio](https://brandemia.org/contenido/subidas/2022/11/logo-amazon-2000-actualidad-1024x576.png)

Utiliza DynamoDB para almacenar información de productos, pedidos, recomendaciones y datos de clientes en tiempo real. Esto les permite ofrecer una experiencia de compra personalizada y escalable.

3. **Juegos en Línea**

![Juego](https://brand.riotgames.com/static/a91000434ed683358004b85c95d43ce0/8a20a/lol-logo.png)

Riot Games emplea Cassandra para manejar la gran cantidad de datos generados por League of Legends, como estadísticas de partidas, perfiles de jugadores y chat.

Blizzard Entertainment utiliza MongoDB para almacenar datos de los jugadores, como personajes, inventario y progreso en el juego.

4. **Plataformas de streaming**

![Netflix](https://m.media-amazon.com/images/I/51LGj5--KsL.png)

Netflix emplea Cassandra para almacenar datos de usuarios, como historial de visualización, calificaciones y recomendaciones. También utiliza Elasticsearch para realizar búsquedas de contenido.

## TAREA 1 | TEMA DEL GRUPO | BASE DE DATOS DE OBJETOS
 
### Autores: 
Carmen y Judith
 
### Origen, ¿Cuándo surgió? ¿Cómo se popularizó?:

Las bases de datos de objetos surgieron en la década de 1960, gracias a los esfuerzos de Kristen Nygaard y Ole-Johan Dahl, pioneros en el desarrollo de sistemas informáticos. Su objetivo era crear un software que replicara fielmente los objetos físicos en un entorno digital, lo que llevó a la creación del lenguaje de programación Simula-67. 
La popularización de las bases de datos de objetos se produjo en los años 80, impulsada por Alan Kay y Xerox. Utilizando Simula-67 como base, desarrollaron Smalltalk, un lenguaje que eventualmente influyó en la creación de C++. 
En la actualidad, las bases de datos de objetos están recuperando relevancia debido a la creciente demanda de aplicaciones que emplean lenguajes de programación orientados a objetos y al apoyo de las comunidades de software libre y POO. 


### Nivel de adopción:

El uso de las bases de datos orientadas a objetos es relativamente limitado en comparación con las bases de datos relacionales. Su aplicación se centra principalmente en áreas que manejan grandes volúmenes de datos complejos y requieren una representación precisa de objetos del mundo real, como en ingeniería y diseño. 
 
### Descripción del funcionamiento del sistema de almacenamiento:

En términos generales, estas bases de datos utilizan la programación orientada a objetos para almacenar y gestionar datos. 

Componentes y Funcionamiento: 

-  Almacenamiento de Objetos 

   - En lugar de utilizar tablas, las bases de datos orientadas a objetos almacenan los datos en forma de objetos, que son instancias de clases con propiedades y métodos definidos. 

- Integridad de Datos 

  - Implementan mecanismos para asegurar la integridad de los datos, como la gestión de transacciones, control de concurrencia y recuperación ante fallos. 

- Persistencia de Objetos 

  - Los objetos creados bajo este modelo pueden ser almacenados directamente en la base de datos sin necesidad de convertirlos a otro formato, como filas o columnas. 

- Consultas 

  - A diferencia de las bases de datos relacionales, estas utilizan lenguajes de consulta orientados a objetos, que permiten realizar consultas complejas sobre los objetos y sus relaciones. 

 
### Ventajas e inconvenientes:

- Ventajas
  - Son perfectas para trabajar con lenguajes de programación orientados a objetos, facilitando su integración en la base de datos.
  - Permiten manipular conjuntos de datos complejos de manera rápida y eficiente.
  - Cada objeto tiene un identificador único asignado.
  - Las transacciones ACID se completan sólo cuando no hay conflictos entre los datos.
  - Cuentan con un sistema de memoria caché que agiliza su uso.
  - Son capaces de manejar grandes volúmenes de datos.

 - Desventajas
   - Su uso no está muy extendido.
   - Si no están bien optimizadas, pueden ser menos eficientes que las bases de datos relacionales.
   - No tienen estándares claros y definidos.
   - Existe poca documentación disponible.
   - Tienen una curva de aprendizaje pronunciada. 
 
### Usos:

La utilización de las bases de datos orientadas a objetos se limita a áreas muy específicas, como la ingeniería, las telecomunicaciones y la biología molecular, porque permiten una manipulación y visualización de datos mucho más sencilla y directa. 

En resumen, su uso se centra en el almacenamiento y manejo de datos muy complejos y/o voluminosos, permitiendo establecer relaciones directas entre los datos, sin necesidad de distribuirlos en tablas como en las bases de datos tradicionales. 
 
### Tipos: Tipos de ficheros, bases de datos representativas, etc:

- Ficheros de objetos puros
   - Almacenan objetos completos, incluyendo sus atributos y métodos

 - Ficheros de objetos relacionales
   - Combinan las caracteristicas de diferentes modelos de bases de datos y pueden manejar tanto datos estructurados como no esctructurados

- Bases de Datos Representativas
  - Db4o
     - Base de datos orientada a objetos, ideal para Java y .NET.
  - ObjectDB
     -  Optimizada para aplicaciones Java.
  - Versant Object Database
     - Ofrece gran rendimiento y escalabilidad, utilizada en aplicaciones empresariales.
  - GemStone/S
     - Soporta Smalltalk, adecuada para aplicaciones críticas. 

### Casos de uso reales observados:

Tienda de material deportivo: En una base de datos de objetos, cada artículo se guarda con sus atributos y métodos. Por ejemplo, unos patines azules, tanto para niños como para adultos. Los patines pertenecen a la clase <patines>, donde también podemos incluir patines de otros colores. La clase patines es una subcategoría de “productos deportivos con ruedas” y puede extenderse según sea necesario. Al acceder mediante el código identificador único del objeto, obtenemos todos sus métodos y atributos. 

Sistema de información geográfica: Los datos geográficos pueden representarse como objetos. Por ejemplo, un objeto “Ciudad” con atributos como “nombre, población y ubicación”, donde “ubicación” puede ser un objeto geográfico. Las bases de datos orientadas a objetos permiten almacenar y manipular estos datos espaciales de manera más directa que en una base de datos relacional. 

Gestión de contenidos multimedia: Este caso puede abordarse de diversas maneras, similar a los anteriores. Por ejemplo, un objeto “Video” podría tener

