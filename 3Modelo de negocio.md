
**¿Cual es el fin del modelo de negocio?** 
Su fin es la *compresión del contexto, identificando los procesos de negocio, casos de uso del sistema de SW a desarrollar de sus futuros usuarios y el valor que a estos confiere*. 

Determinar el alcance del proyecto -> determinar tiempo y costo. 

***Proceso*** : 
1. Análisis externo → modelo de casos de uso del negocio (listado de procesos en función del cliente)
2. Análisis interno → modelo de análisis del negocio (descripción de procesos)

>**Uso del modelo de dominio**: las clases del dominio y el glosario de términos se utilizan en el desarrollo de los modelos de caso de uso y análisis. Un modelo de dominio es en realidad un caso especial de un modelo de negocio más completo, por lo tanto, desarrollar un modelo de negocio es una alternativa más potente que desarrollar un modelo de dominio.

### ¿Que es un modelo de negocio? 

En primer lugar, un modelo de casos de uso del negocio, describe los procesos de negocio de una empresa en términos de casos de uso del negocio y actores del negocio que corresponden con los procesos del negocio y los clientes respectivamente.

Un modelo de objetos del negocio es un modelo interno a un negocio. Describe cómo cada caso de uso del negocio es llevado a cabo por parte de un conjunto de trabajadores que utilizan un conjunto de entidades del negocio y de unidades de trabajo. 

### Modelo de CU del negocio 

**Modelo de negocio** = actores del negocio + CU iniciado por ellos + actores colaboradores estos CU

**Modelo de CU** = especificación del modelo de negocio. Se añade además actores y sus CU (incluidos o extendidos)

### Elementos (artefactos)

![[Pasted image 20250703115111.png]]

# Flujo de trabajo (modelo de negocio)

1. Identificar actores del negocio
2. Identificar casos de uso de actores del negocio 
3. Establecer asociaciones entre actores del negocio y casos de uso 

### Actores

Quienes interactúan con el sistema pero no pertenecen a él, y son beneficiados por este y colaboran

- El analista de sistemas da nombre a los actores y hace una descripción breve de c/u en la que esboza sus necesidades y responsabilidades.
- Lo hacen desde un rol, un actor es una persona, un dispositivo de otro sistema administrativo, responsable de… (trabajador) → rol representado por una persona, cada actor desempeña una actividad.

"*Los actores delimitan el entorno del sistema*" 

* **Actores de negocio**: se benefician del sistema. El sistema se rea para ellos, pero son externos a este. Desencadenan acciones. 
* **Actor interno**: necesarios para que ciertas funciones se lleven a cabo. Muchas veces los desencadenan y pertenecen al sistema. 
* **Actor colaborador**: dan soporte al sistema para que pueda realizar sus actividades y brindan información inmediata, son sistemas en si mismos y no inician acciones.
	- Sólo son parte del modelo de negocio cuando colaboran a un CU de este. 
	- Instancia de un actor (caso de uso real): Interacción concreta, ejecución particular de un caso de uso.

### Casos de uso 

Acciones que el sistema lleva a cabo interactuando con actores.

Abstracción de “fragmentos de funcionalidad” que aportan un resultado de valor a los actores. 

Por lo tanto es una especificación, ya que especifica el comportamiento de “cosas” dinámicas.

También es un “clarificador” lo que quiere decir que tiene operaciones y atributos. Una descripción puede incluir **diagramas de estados** (especifican el ciclo de vida en términos de estado y transiciones entre los estados), de **actividad** (describen el ciclo de vida, describiendo la secuencia temporal de acciones dentro de cada transición), **colaboraciones** y **diagramas de secuencia**. 

Se consideran atómicas las instancias de casos de uso, cada una de ellas se ejecuta por completo o no se ejecuta. 
	*La cantidad de casos de uso base siempre es iguala la cantidad de requisitos funcionales.*

#### Flujo de sucesos 
Especificación de cu es una secuencia de acciones en forma de texto y diagrama. 

- Preciso pero fácil de leer por desarrolladores y usuarios
- Especificación de cuándo empieza y termina el CU
- Orden de los sucesos: _camino básico ( + completo y - probable )_ y _caminos alternativos_
- Acciones del sistema e intercambios de actores
- Cada CU se describe de forma aislada aunque se incluye descripción de requisito no funcional

#### Prototipo de interfaz de usuario / Graphical User Interfase (GUI)

1. **Crear un diseño lógico de interfaz**

Recorrer cada actor y sus caso de uso e identificas los elementos (objetos con los que el usuario interactúa y manipula) de la interfaz.

- Los elementos se corresponden con los atributos del CU.
- Un elemento puede ser usado en muchos CU y en distintas interfaces, desempeñando papeles diferentes (bocetos en papel y prototipos ejecutables IGU).

El prototipo de interfaces se usa durante el proceso de **captura de requisitos**, y sirve para la especificación de la interfaz. La **implementación** se realiza en paralelo a los flujos de análisis, diseño e implementación. El *prototipo ayuda al usuario a entender el sistema y validar los requerimientos*. 

![[Pasted image 20250703121053.png]]

### Descripción de la arquitectura 

A través del modelo de casos de uso, los requisitos adicionales y el glosario, el arquitecto prioriza los casos de uso, para determinar (esbozar) cuáles deben ser desarrollados en las primeras iteraciones.

![[Pasted image 20250703121404.png]]

**Casos de uso concretos:** Iniciados por un actor y sus instancias son una secuencia de acciones completa ejecutada por el sistema.

**Casos de uso abstractos:** Existe solo para ser usado por otros caso de uso y no es instanciable.

## Relaciones

* **Asociaciones** 
	* iniciación 
	* Colaboración: *cuando empieza a ejecutarse la acción se envía info al colaborador que corresponde. Siempre en un sistema que puede responder instantáneamente a su acción realizada*.
* **Inclusión**
	Un CU, dispara ( o incluye) a otro (si o sí el include lleva 2 cu). En terminos simples, cuando relacionamos dos cu con un include, deimos que primero el cu base dispara al include. O sea, que el el caso de uso que dispara el cu de base es esencial para lograr el resultado de valor del cu base.
- **Extensión:**
    
    Idem inclusión pero para relaciones ocasiones o condicionadas
    
    Extend. La polémica al querer seleccionar una de las dos relaciones es que en el “extend” también podemos ver, desde la perspectiva del usuario, a los dos flujos como si fueran uno sólo. Y en ciertos escenarios el CU base no podría cumplir su objetivo si no se ejecutara la extensión. Pero, una de las diferencias básicas es que en el caso del “extend” hay situaciones en que el CU de extensión no es indispensable que ocurra, y cuando lo hace ofrece un valor extra (extiende) al objetivo original del caso de uso base. En cambio en el “include” es necesario que ocurra el caso incluido, tan sólo para satisfacer el objetivo del caso de uso base. Ejemplo: Puedes “Realizar Venta” sin “Acumular Puntos de Cliente VIP”, cuando no eres un cliente VIP. Pero, si eres un cliente VIP sí acumularás puntos. Por lo tanto, “Acumular Puntos” es una extensión de “Realizar Venta” y sólo se ejecuta para cierto tipo de ventas, no para todas.
    
- **Generalización**
    
    Un elemento (A) hereda las característica
    - Cuando dos actores se ocupan, sus funciones, a veces se crea, un atributo general que ambos heredan
 
Los casos de uso (instancias) reales se obtienen aplicando las reglas de generalización y extensións de otro (B) 

