## Bases de Datos Orientadas a Objetos (BDOO)

### Autores
* Luis Iturrioz López
* David Fernández Suco

### Origen y Popularización
El origen se remonta a la década de los 70 con los primeros lenguajes de programación orientados a objetos, pero el término “base de datos orientado a objetos” no nació hasta el 85. La popularización se dio en parte por el aumento de aplicaciones que requerían manejar datos complejos, como gráficos, multimedia y sistemas CAD. Además, la proliferación de lenguajes de programación orientados a objetos, como C++ y Java, facilitó su adopción.

### Nivel de Adopción
La adopción es limitada, aunque tiene ciertos nichos donde son populares, como cuando se trabaja con datos complejos, pero en general distan bastante de estar adoptadas a gran escala. 

### Descripción del funcionamiento del sistema de almacenamiento
Funcionan agrupando en paquetes relacionados la información, estos paquetes son objetos que almacenan la información, a diferencia de otras bases de datos que guardan su información en filas y columnas. Las BDOO emplean lenguajes de programación y se pueden aplicar métodos, clases y subclases.

### Ventajas e inconvenientes
* **Ventajas:**
    * Mayor capacidad de modelado: Representan el mundo real de forma más intuitiva 
    * Flexibilidad: Permiten adaptarse a cambios en los requisitos de una aplicación
    * Manejo de datos complejos: Son ideales para gestionar datos de gran tamaño y complejidad. 
    * Integración con lenguajes orientados a objetos: La integración con lenguajes como Java o C++ es más natural 
    * Reutilización de código: Al permitir la creación de clases y jerarquías de clases, se promueve la reutilización de código. 
* **Inconvenientes:**
    * Complejidad: Requiere un mayor conocimiento y experiencia por parte de los desarrolladores. 
    * Madurez: Las BDOO aún no están tan maduras como las bases de datos relacionales, lo que puede implicar una menor disponibilidad de herramientas y soporte. 
    * Rendimiento: En algunos casos, el rendimiento de las BDOO puede ser inferior al de las bases de datos relacionales, especialmente en consultas complejas
    * Falta de un estándar universal: No existe un estándar universal para las BDOO, lo que dificulta la portabilidad de las aplicaciones entre diferentes sistemas.
    * Costo: Las licencias de los sistemas de gestión de bases de datos orientados a objetos suelen ser más costosas que las de los sistemas relacionales.

### Usos
* Modelado de datos complejos: Son ideales para representar entidades del mundo real con sus atributos y relaciones de manera intuitiva.  
* Gestión de datos multimedia: Gracias a su capacidad para almacenar objetos complejos, son excelentes para manejar imágenes, videos, audio y otros tipos de datos multimedia.
* Gestión de información geográfica (GIS): Los sistemas GIS utilizan BDOO para modelar entidades geográficas como puntos, líneas y polígonos, así como sus atributos y relaciones espaciales. 
* Aplicaciones CAD/CAM: En el diseño asistido por computadora (CAD) y la fabricación asistida por computadora (CAM), permiten representar de forma precisa objetos tridimensionales y sus relaciones geométricas. 
* Inteligencia artificial: Son útiles en aplicaciones de inteligencia artificial, como sistemas expertos y redes neuronales, para representar el conocimiento y los datos de manera estructurada. 

### Tipos
* **BDOO Puras:**
    * Definición: Implementan de forma completa los conceptos de la programación orientada a objetos, como la herencia, el polimorfismo y la encapsulación.
    * Características: Ofrecen un alto nivel de abstracción y una estrecha integración con los lenguajes de programación orientados a objetos.
* **BDOO Híbridas:**
    * Definición: Combinan características de las bases de datos relacionales y orientaadas a objetos.
    * Características: Ofrecen un equilibrio entre la flexibilidad de las BDOO y la eficiencia de las bases de datos relacionales.
* **Objetos-Relacionales:**
    * Definición: Son una evolución de las bases de datos relacionales que añaden soporte para tipos de datos complejos y objetos.
    * Características: Permiten almacenar y manipular tanto datos estructurados como no estructurados, ofreciendo una mayor flexibilidad.

### Casos de uso reales
* **CATIA (CAD)** utiliza BDOO para gestionar la información de los diseños, desde piezas individuales hasta ensamblajes completos. Esto facilita la creación de configuraciones, variantes y la gestión del ciclo de vida del producto.
* **ArcGIS (GIS)** utiliza BDOO para almacenar y gestionar la información geográfica. Por ejemplo, un río puede ser representado como un objeto con atributos como longitud, caudal y calidad del agua, y relacionado con otros objetos como puentes o ciudades.
* **BioJava (Bioinformática)** utiliza BDOO para representar secuencias de proteínas, estructuras 3D y vías metabólicas. Esto facilita el análisis y la comparación de datos biológicos. 

