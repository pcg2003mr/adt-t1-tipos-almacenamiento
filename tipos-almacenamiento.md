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
![Redes](https://cdn.cms-twdigitalassets.com/content/dam/legal-twitter/sharing-card.png.twimg.768.png)(https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTQKrFhY-ljA-u7J5IMWeTv8zmpBx4PP9nQMw&s)

Facebook utiliza Cassandra para manejar los datos generados por usuarios como comentarios, likes, publicaciones...X utiliza también Cassandra y Storm para procesar en tiempo real los tweets y construir un índice de búsqueda invertido.
