UML no está ligado a ningún ciclo de vida de desarrollo de software particular. Sin embargo la metodología del proceso unificado usa UML. Esta metodología es _**dirigida por un plan y evolutiva.**_

Para obtener el máximo beneficio del proceso debe ser:

- **Dirigido por Casos de Uso:** Es decir, que primero _(las entradas del proceso unificado son CU_) se determina el comportamiento deseado del sistema _(centro = cliente)_, y luego los casos de uso son el criterio fundamental para verificar y validar las Arq., para las pruebas, y para la comunicación entre los involucrados en el proyecto.

Los CU dan soporte a la trazabilidad entre modelos

- **Centrado en la Arquitectura:** Es decir, este es el artefacto básico usado para conceptualizar, gestionar y hacer evolucionar el sistema → un conjunto de vistas en el método que propone el proceso unificado para desarrollar SW centrado en CU
- **Proceso iterativo e incremental:** Involucra la gestión de un flujo de artefactos, ejecutables (comunicación continua con el cliente) y cada artefacto mejora a los anteriores → “Dirigido por el resigo” cada vez este se reduce más.

![[Pasted image 20250704115800.png]]
El modelo de análisis es un *modelo conceptual cuyo fin es acrecentar la composición de los CU y por ende el sistema*. Puede durar toda la vida del sistema. Son “realizaciones de CU” son base para el diseño.

![[Pasted image 20250704115851.png]]

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



