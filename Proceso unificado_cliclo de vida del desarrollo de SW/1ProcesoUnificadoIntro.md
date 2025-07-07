UML no está ligado a ningún ciclo de vida de desarrollo de software particular. Sin embargo la metodología del proceso unificado usa UML. Esta metodología es _**dirigida por un plan y evolutiva.**_

Es un proceso de desarrollo de software. Un proceso de desarrollo de software *es el conjunto de actividades necesarias para transformar los requisitos de un usuario en un sistema software*.
El proceso unificado es un **marco de trabajo genérico que puede especializarse para una gran variedad de sistemas de software, para diferentes áreas de aplicación, diferentes tipos de organizaciones, diferentes niveles de aptitud y diferentes tamaños de proyecto**.
Está basado en *componentes*, lo cual quiere decir que el sistema software en construcción está formado por componentes software interconectados a través de interfaces bien definidas.
El proceso unificado utiliza el ***Lenguaje Unificado de Modelado (UML)***, para preparar todos los esquemas de un sistema software.

#### Características 
Para obtener el máximo beneficio del proceso debe ser:

- **Dirigido por Casos de Uso:** Es decir, que primero _(las entradas del proceso unificado son CU_) se determina el comportamiento deseado del sistema _(centro = cliente)_, y luego los casos de uso son el criterio fundamental para verificar y validar las Arq., para las pruebas, y para la comunicación entre los involucrados en el proyecto.
	El término usuario no sólo hace referencia a usuarios sino a otros sistemas. En este sentido “usuario” representa alguien o algo que interactúan con el sistema que estamos desarrollando. Una interacción de este tipo es un caso de uso. Un caso de uso es un fragmento de funcionalidad del sistema que proporciona al usuario un resultado importante. Los casos de uso representan los requisitos funcionales y constituyen el modelo de casos de uso, el cual describe la funcionalidad total del sistema.
	Los casos de uso son herramientas para especificar los requisitos de un sistema, además guían su diseño, implementación y prueba, es decir, guían el proceso de desarrollo.
	Los casos de uso no sólo inician el proceso de desarrollo sino que le proporcionan un hilo conductor. Dirigido por casos de uso significa que el desarrollo sigue un “hilo”. Los casos de uso se especifican, se diseñan y los casos de uso finales son la fuente de la cual los ingenieros de prueba construyen sus casos de prueba.
	Los CU dan soporte a la trazabilidad entre modelos

- **Centrado en la Arquitectura:** Es decir, este es el artefacto básico usado para conceptualizar, gestionar y hacer evolucionar el sistema → un conjunto de vistas en el método que propone el proceso unificado para desarrollar SW centrado en CU. 

La arquitectura en un sistema de software se describe mediante diferentes vistas del sistema en construcción. El concepto de arquitectura de software incluye los aspectos estáticos y dinámicos más significativos del sistema.
La arquitectura surge de las necesidades de la empresa, como las perciben los usuarios y los inversores y se refleja en los casos de uso.

La arquitectura es una vista del diseño completo con las características más importantes resaltadas, dejando los detalles de lado. El proceso ayuda al arquitecto a centrase en los objetivos adecuados, como la comprensibilidad, la capacidad de adaptación al cambio y la reutilización. 

Cada producto tiene tanto una función como una forma. La función corresponde a los casos de uso y la forma a la arquitectura. Por ello debe haber interacción entre ellos y deben evolucionar en paralelo.

Los arquitectos modelan el sistema para darle una forma, por eso, es la arquitectura la que debe diseñarse para permitir que el sistema evolucione en su desarrollo inicial y a lo largo de las futuras generaciones. Para encontrar esta forma los arquitectos deben trabajar sobre casos de uso clave del sistema.

- **Proceso iterativo e incremental:** Involucra la gestión de un flujo de artefactos, ejecutables (comunicación continua con el cliente) y cada artefacto mejora a los anteriores → “Dirigido por el resigo” cada vez este se reduce más.

***Iterativo***
*Hace referencia a repetir el flujo de trabajo, se realiza una y otra vez.*

***Incremental***
• Los incrementos hacen referencia al crecimiento de la producción.
• Se pueden crear versiones del sistema e ir mejorándolas.
• Termina una actividad y entrega un incremento, una versión que "puede operar".

**Ventajas**
• Se obtiene un producto sólido
• Reduce costos
• Reduce tiempos
• Permite reducir riesgos

![[Pasted image 20250704115800.png]]
El modelo de análisis es un *modelo conceptual cuyo fin es acrecentar la composición de los CU y por ende el sistema*. Puede durar toda la vida del sistema. Son “realizaciones de CU” son base para el diseño.

![[Pasted image 20250704115851.png]]
El proceso unificado se repite a lo largo de una serie de ciclos que constituyen la vida de un sistema. Cada ciclo concluye con una versión del producto para los clientes y consta de cuatro fases:

1. ***Fase de inicio***: se desarrolla una descripción del producto final a partir de una buena idea y se presenta el análisis de negocio para el producto.
2. ***Fase de Elaboración***: se especifican en detalle la mayoría de los casos de uso del producto y se diseña la arquitectura del sistema. El resultado de esta fase es una línea base de la arquitectura, y la disposición del director de planificar las actividades y estimar los recursos necesarios para terminar el proyecto.
3. ***Fase de Construcción***: se crea el producto. Aquí la línea base de la arquitectura crece hasta convertirse en el sistema completo. Al final de esta fase, el producto tiene todos los casos de uso que la dirección y el cliente han acordado para el desarrollo de esta versión. Sin embargo, puede tener defectos.
4. ***Fase de Transición***: cubre el periodo comprendido durante el cual el producto se convierte en versión beta. Esta fase corrige errores antes de la entrega. El equipo de mantenimiento divide los errores en 2 categorías: los que tienen suficiente impacto en la operación para justificar una versión incrementada y los que pueden corregirse en la siguiente versión normal.

Cada fase se subdivide a su vez en iteraciones o mini proyectos y cada iteración pasa por los 5 flujos de trabajo fundamentales: **Captura de requisitos, Análisis, Diseño, Implementación, Prueba**

![[Pasted image 20250707125659.png]]

## Etapa de análisis

#### Diagrama de clases
Los CU que se detectan en la etapa de análisis no actualizan la lista de req. funcionales

**FIN:** *modelar la parte estática del modelo de procesos, en concreto, las relaciones entre clases (”bloques de construcción”), interfaces y colaboraciones.*

- Uno de los diagramas estructurales esenciales de UML, herramienta principal del modelado OO
- Usado en la fase de análisis y diseño (vista de diseño y de procesos)

![[Pasted image 20250704120023.png]]

##### Relaciones entre clases

* **Asociación** 
	Relación estructural fundamental del diagrama de clases
	**¿Cuándo?**

	- La relación surge de los requisitos

		
	- Dos clases se asocian cuando una requiere información de la otra. **-** **A** usa un servicio de **B**
	- **A** crea **B
	- A** es una colección de objetos de **B
	- A** envía un mensaje a **B**

	**Propiedades** Las clases se encuentran vinculadas durante toda su existencia

	**Orden:** Cuántas clases asocia
* **Composición**
	Asociación **fuerte** entre conjuntos y sus partes

	**Propiedades**
	A es parte de B

	- _**Exclusividad:**_ La parte pertenece a un único conjunto
	- _**Dependencia:**_ Las partes se crean y eliminan cuando se hace esto en el conjunto. La parte solo existe si existe el todo, si se elimina la parte no se elimina el todo y la cantidad de partes puede variar en el tiempo, pudiendo incluso quedarse sin partes.
	- Siempre especificar cardinalidad 
	![[Pasted image 20250704121517.png]]
	
* **Agregación** (relación débil)
	Asociación débil entre un conjunto y sus pares (contención física)

	**Propiedades** A es parte de B

	- Relación unidireccional **A** ← **B -** Si **B** se elimina no necesariamente se elimina **A -** Una instancia **A** puede ser parte de muchas instancias **B**
	**¿Cuándo?**

	- Se desea hacer explícita la relación por motivos de ensamblaje
	- Los cambios en el conjunto afectan a las partes
	- Tiempo de vida de **B** afecta el de **A**
	 💡 Ante la duda usar asociación normal
* **Generalización** 
	Relación de herencia

	**Propiedades**
	A hereda las características de B
	- El N° de atributos de A es la suma de las propias y las heredadas.
	- No se recomiendan + de 5 niveles de generalización.
	- Aún en una generalización las clases que heredan deben tener al menos un atributo.
	- El diagrama no permite saber qué clases son abstractas y qué se instancia y qué no, no es criterio para decisiones


##### Clases
“Conjunto de objetos que comparten los mismos atributos, operaciones y relaciones y semántica” → Patrón para la construcción de objetos

**Enlace** = Instancia de relación 
**Objeto** = Instancia de clase

***Propiedades***
Las clases deben cubrir toda clase de Dominio y todos los Casos de Uso
- Instanciar es útil para detectar clases de una factura, documentación, etc. Siempre se guarda la fecha.
- Operaciones básicas: crear, ver o consultar, modificar, eliminar
- La vigencia siempre supone 2 atributos: inicio y fin

![[Pasted image 20250704121755.png]]

##### Clases de asociación 

* Suceso que genera información
* Siempre que un objeto A se enlaza con un objeto B, se crea un objeto C

![[Pasted image 20250704121844.png]]
##### Clase parámetro (parametrizada) 
Cuando un atributo puede cobrar un conjunto de valores (tienen 1 atributo, su nombre), se crea una clase con el objeto de:

- Guardar el conjunto de etiquetas una única vez para disminuir el uso de memoria
- Restringir los valores que puede tomar el atributo
- Se crea con el fin de optimizar
- El proceso en que se inserta la creación de clases parámetro se conoce como _normalización de la información_
- Crear una clase parámetro implica crear un CU que administre las instancias (muchas se demominan “ABM NombreParámetro”) de esa clase parámetro.    
- Muchas veces estas clases toman como nombre como: Par_nombreAtributo
- Muchas veces se crea


![[Pasted image 20250704121959.png]]
#### Especificación de CU 

Cada uno de los casos de uso se especifica: Extensión (A y B se especifican, Generalización (Se especifica cada uno de los hijos (B y C) con lo que hereda del padre A)

![[Pasted image 20250704122924.png]]

##### Parte 2: descripción detallada a partir de la secuencia

- ***Precondición***    
    Condiciones que se deben cumplir para que se ejecute el CU → CU cumplidos (_Ej: Cliente registrado_)
    - No se verifican en el camino normal del CU
    - Se escriben en presente simple
- ***Estado inicial***
    Estado que deben tener los atributos involucrados en el CU. _Ej: Servicio = “pagado”_
- ***Postcondición***
    Conjunto de condiciones que se deben cumplir para que el CU se dé por finalizado.
    **Éxito**
    *Ej: - Se modifica la historia clínica del cliente → Objetivo del CU cumplido
    - Se imprime comprobante → Comunicación mails, mensajes, etc.
    - Se modifica estado de una cama → Cambio valores - atributos
    - Se guarda internación → Clases creadas*
    **Fracaso**
    _Ej: - No hay camas disponibles → Motivos_
    - Se verifican cuando el CU finaliza. No se aclara de estas verificaciones en el camino normal.

![[Pasted image 20250704123033.png]]
_**Referencias**_
**Camino Normal:** _Aquello que lleva a que el CU se ejecute exitosamente_
**Buscar habitación correspondiente al tratamiento:** _Indicar validaciones → No se incluye validaciones de los datos ingresados por el usuario, se supone que ese ingresado sin errores._
**Ex 01:** _La excepción se da cuando el paso no puede ejecutarse._
**GUI 2:** _Si se solicita información, aclarar todos los datos que se piden si se muestra una GUI, aclarar que datos se muestran._
**SF 01:** _Si las acciones asociadas al condicional son de 1 paso, se escribe en el camino normal, sino hay que hacer subflujos → los condicionales se ponen del lado del sistema_
**Ext. Registro:** _Se ejecuta y se regresa, debe corresponder con modelo CU._
**Acción 1:** _Pasos concurrentes: Se debe realizar ambos pero no importa en que orden._
**Acción 2:** _Indicar datos guardados y actualizaciones de objetos._
**Acción ir a { paso 5 }:** _Ver paso 5 (Si se escribiera esta referencia en un subflujo o excepción se escribe como {ret 1})_
- _No se indican posibles anulaciones por parte del usuario durante el proceso._
- _Si hay colaboradores, sus acciones se indican en la misma columna que las de los actores iniciales._

![[Pasted image 20250704123121.png]]

Ref;
- Siempre hay que hacer un cuadro por cada uno tanto subflujo o excepciones.
- Se recomienda poner en subflujos las extensiones e inclusiones a otros CU para visualizar más fácilmente la complejidad del CU → Extensiones en excepciones ; Inclusiones en subflujos.
- No se escribe return, se da por supuesto.
- A veces las Excepciones terminan en FIN CU.
- Si hay fracaso, se da por supuesto y no se anota que los datos que se hayan quedado se eliminan.

###### Parte 3: info adicional 
 **Consideraciones de diseño/requisitos no funcionales (cd)**
	Sugerencias → a solicitud del cliente

**Reglas de negocio (rn)**
	Distinto a precondiciones
 **GUI**:
	Se incluye su nombre y un dibujo



