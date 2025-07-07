La captura de requisitos es el proceso de averiguar, normalmente en circunstancias difíciles, lo que se debe construir. Este proceso por lo general es complicado y difícil ya que con frecuencia los usuarios no saben cuáles son los requisitos ni tampoco cómo especificarlos de una manera precisa. A medida que el proyecto avanza, los usuarios, los intermediarios y los desarrolladores pueden ver como parece el sistema y por tanto llegan a comprender mejor las verdaderas necesidades y surgen una gran cantidad de cambios.
Es importante que los sistemas den soporte a la misión para la cual se construyen, es decir, el sistema debe proporcionar valor al negocio que lo utiliza y a sus clientes.

**Flujo de trabajo de la captura de requisitos**:
* Enumerar los requisitos candidatos
* Comprender el contexto del sistema
* Capturar requisitos funcionales. 
* Capturar requisitos no funcionales. 

#### ¿Que debe hacer el sistema? 

Los requisitos son las condiciones o capacidades que debe tener un sistema informático para que pueda resolver un problema o alcanzar un objetivo propuesto. El requisito es una necesidad documentada sobre el contenido, forma o funcionalidad de un producto o servicio. 

#### Características de un requisito 

* No son ambiguos 
* Concisos
* Consistentes 
* Completos 
* Alcanzables 
* Verificables

 > ***Requisitos funcionales***: son acciones elementales, funciones especificas del sistema. Cada usuario quiere que el sistema haga algo para el o ella, o sea, que lleve a cabo ciertos casos de uso.  
 
 > ***Requisitos no funcionales***: especifican propiedades del sistema, como restricciones del entorno o de la implementación, rendimiento, dependencias de la plataforma, facilidad de mantenimiento, extensibilidad, requisitos de seguridad, fiabilidad. Son más abstractos y no pueden relacionarse con un caso de uso concreto o una clase concreta del mundo real. Estos generan como artefacto resultante los "Requisitos adicionales" o "Casos de uso concretos" 

# Visión general de captura de requisitos 
### Enumeración de requisitos candidatos (planificación del trabajo) 

Son como la características del sistema existente, las cuales reflejan necesidades ( se crea un listado de posibles características del sistema a crear: ) y restricciones (reglas de negocio: pautas establecidas que restringen el negocio desde antes de la implementación del sistema), como también reflejan entradas y salidas esperadas del sistema a crear. 

Planificación y valores a tener en cuenta de cada característica: 
* **Estado** (propuesto, aprobado, incluido o validado)
- **Coste estimado de implementación** (tipos de recursos y horas-persona)
- **Prioridad** (crítico, importante o secundario)
- **Nivel de riesgo asociado a su implementación** 

> El análisis permite estimar el tamaño del proyecto y dividirlo en una secuencia de iteraciones y en subsistemas que representen las funcionalidades principales. 

> *Durante el proceso de desarrollo descubrimos que faltan requisitos o alguno es incorrecto. Por estas correcciones se dice que la captura es una "construcción incremental"*. 

### Comprender el contexto del sistema

**Modelado de dominio** -> *conceptos importantes y cómo se relacionan* 
**Modelado de negocio** -> *procesos* 

### Capturar requisitos funcionales

Restricciones de hardware o software. Asociados a casos de uso (especiales o actividades del caso de uso) o adicionales (alcanzan a todo el sistema) y se documetan en listados. 

Clasificación: 

* Performance → tiempo real, restricciones de tiempo, velocidad de procesamiento
- Precisión → precisión numérica, info numérica en el tiempo correcto
- Confiabilidad → disponibilidad de equipos, integridad de info
- Localización → geográfico, de responsabilidades
- Sociales → culturales, usabilidad
- Legales y políticos
- Mantenimientos y soporte
- Seguridad

![[Pasted image 20250702193211.png]]

### Capturar requisitos no funcionales

# Fases del desarrollo de software

![[Pasted image 20250702193259.png]]

Artefacto = producto 

* **Artefacto** : cualquier tipo de descripción o información creada o producida, cambiada o o utilizada por los trabajadores durante su trabajo con el sistema. 

![[Pasted image 20250702195520.png]]

## Flujo de trabajo captura de requisitos

![[Pasted image 20250703125855.png]]

Workflow de análisis de sistemas: 
1. Arquitecto -> analisis de Arq.
2. Ing de CU -> analizar un cu
3. ing. de componentes -> analizar una clase -> analizar un paquete 

