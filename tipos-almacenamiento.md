# Tipos de almacenamiento

## Titulo: Bases de Datos Relacionales

### [¿Qué es una base de datos relacional?]. 
Una base de datos relacional (RDB) es una forma de estructurar información en tablas, filas y columnas. Un RDB tiene la capacidad de establecer vínculos (o relaciones) entre información mediante la unión de tablas, lo que facilita la comprensión y la obtención de estadísticas sobre la relación entre varios datos. 

### [Nivel de adopción] 
Las bases de datos relacionales (RDBMS) son populares en la industria por su estructura en tablas y capacidad para mantener la integridad de los datos mediante relaciones entre tablas. Ejemplos comunes incluyen MySQL, PostgreSQL, Oracle y SQL Server, preferidos en entornos empresariales por su madurez y uso estandarizado de SQL.  

Además, cuentan con un ecosistema robusto de herramientas, amplia documentación y desarrolladores experimentados. Sin embargo, tienen limitaciones con datos no estructurados o grandes volúmenes de datos, donde las bases NoSQL son más eficientes. 

### [Funcionamiento del sistema de almacenamiento] 
Las bases de datos relacionales almacenan datos en tablas compuestas por filas (registros) y columnas (atributos). Las claves primarias identifican de manera única cada registro, mientras que las claves foráneas conectan tablas, referenciando claves primarias de otras tablas. Los usuarios interactúan con la base de datos mediante SQL para gestionar datos. 

Además, soportan transacciones, que son conjuntos de operaciones que deben completarse en su totalidad para mantener la consistencia e integridad de los datos. 

### [Ventajas e Inconvenientes:] 
1) **Ventajas:**
 El principal beneficio del modelo de base de datos relacional es que proporciona una manera intuitiva de representar datos y permite un acceso fácil a datos relacionados. 

-Flexibilidad: Es fácil agregar, actualizar o borrar tablas, relaciones y hacer otros cambios a los datos cuando lo necesites sin cambiar la estructura general de la base de datos ni afectar las aplicaciones existentes. 

-Cumplimiento de ACID: Las bases de datos relacionales admiten el cumplimiento de ACID (atomicidad, coherencia, aislamiento y durabilidad) para garantizar la validez de los datos, sin importar si se producen errores, fallas o contratiempos de otro tipo. 

-Facilidad de uso: Es fácil ejecutar consultas complejas con SQL, lo que permite que incluso los usuarios no técnicos aprendan a interactuar con la base de datos. 

-Colaboración: Varias personas pueden operar y acceder a datos de manera simultánea. El bloqueo integrado impide el acceso simultáneo a los datos cuando se actualizan. 

-Seguridad Integrada: La seguridad basada en roles garantiza que el acceso a los datos esté limitado a usuarios específicos. 

-Normalización de Bases de Datos: Las bases de datos relacionales usan una técnica de diseño conocida como normalización que reduce la redundancia de los datos y mejora su integridad. 

2) **Inconvenientes:**
-Escalabilidad limitada: Las RDBMS suelen tener dificultades para escalar horizontalmente (añadir más servidores), lo que las hace menos eficientes en grandes volúmenes de datos distribuidos.

-Consultas complejas y lentas: Las consultas SQL pueden volverse muy complejas y difíciles de mantener, especialmente con datos altamente relacionados. Esto puede afectar el rendimiento.

-Rigidez en el esquema: El esquema de una base de datos relacional es rígido y estructurado, lo que hace que sea complicado modificar la estructura de las tablas cuando cambian los requisitos del negocio o de la aplicación.

-Altos costos de transacciones: Aunque las RDBMS soportan transacciones ACID (Atomicidad, Consistencia, Aislamiento, Durabilidad), mantener estas propiedades puede ser costoso en términos de rendimiento, especialmente en grandes volúmenes de datos.

-Ineficiencia con datos no estructurados: Las RDBMS no son adecuadas para gestionar datos no estructurados o semi-estructurados como documentos, imágenes, videos o grandes conjuntos de datos sin un formato claro.

-Sobrecarga de administración: La necesidad de mantener la integridad referencial, constraints, y otras características propias de las RDBMS puede generar sobrecarga de administración y más tiempo de desarrollo.

### [Diferencia entre bases de datos relacionales y no relacionales:] 

La principal diferencia entre las bases de datos relacionales y no relacionales (bases de datos NoSQL) es la forma en que se almacenan y organizan los datos. Las bases de datos no relacionales no almacenan datos de manera tabular y basada en reglas. En su lugar, almacenan datos como archivos individuales y no conectados, y se pueden usar para tipos de datos complejos y no estructurados, como documentos o archivos de rich media. 
