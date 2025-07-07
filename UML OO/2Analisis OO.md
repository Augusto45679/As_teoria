Durante el análisis, analizamos los requisitos que se describieron en la captura de requisitos, refinándolos y estructurándolos. El objetivo de hacerlo es conseguir una comprensión más precisa de los requisitos y una descripción de los mismos que sea fácil de mantener y que nos ayude a estructurar el sistema entero.
Si conseguimos llegar a un acuerdo con el cliente sobre lo que debería hacer el sistema, es probable que aún queden aspectos sin resolver relativos a los requisitos del sistema. Éste es el precio que hay que pagar por usar un lenguaje intuitivo pero impreciso del cliente durante la captura de requisitos. A fin de comunicar eficientemente las funciones del sistema al cliente:
* Los casos de uso deben mantenerse tan independientes unos de otros como sea posible.
* Los casos de uso deben describirse utilizando el lenguaje del cliente.
* Debe estructurarse cada caso de uso para que forme una especificación de funcionalidad completa e intuitiva.

Dados esos temas sin tratar, el propósito fundamental del análisis es resolverlos analizando los requisitos con mayor profundidad, pero con la gran diferencia de que puede utilizarse el lenguaje de los desarrolladores para describir resultados.

En consecuencia, en el análisis podemos refinar los requisitos y estructurarlos como más nos convenga.

Esta estructura (basada en clases de análisis y paquetes) es independiente de la estructura que se dio a los requisitos, aunque existe una trazabilidad directa entre ambas.

![[Pasted image 20250707184405.png]]

## Artefactos del modelo de análisis

1. **Modelo de análisis**
![[Pasted image 20250707184902.png]]

2. **Clase del análisis**:  una clase de análisis representa una abstracción de una o varias clases y/o subsistemas del diseño del sistema. Este tipo de clase se centra en el tratamiento de los requisitos funcionales y pospone los no funcionales especiales. Además define atributos, pero con gran abstracción. Participa en relaciones del tipo conceptual, es decir, son distintas a las relaciones de implementación. Se clasifican en:
	* ***Clase de interfaz***:  se utilizan para modelar la interacción entre el sistema y sus actores. Esta interacción a menudo implica recibir (y presentar) información y peticiones de (y hacia) los usuarios y los sistemas externos. Las clases de interfaz representan a menudo abstracciones de ventanas, formularios, sensores, API’s, etc. Cada clase de interfaz debería asociarse con un actor y viceversa. 
		![[Pasted image 20250704172724.png]]
	
	* ***Clase de entidad***:  se utilizan para modelar información que posee una vida larga y que es a menudo persistente. Reflejan la información de un modo que beneficia a los desarrolladores al diseñar e implementar el sistema, incluyendo su soporte de persistencia. 
		![[Pasted image 20250704172735.png]]
	* ***Clase de control***: representan coordinación, secuencia, transacciones y control de otros objetos. Se usan con frecuencia para encapsular el control de un caso de uso en concreto. También se utilizan para representar derivaciones y cálculos complejos, que no pueden asociarse con ninguna información concreta. Los aspectos dinámicos del sistema se modelan con clases de control.
		![[Pasted image 20250704172730.png]]
	
3. **Realización de caso de uso- análisis**: una realización de caso de uso – análisis es una colaboración dentro del modelo de análisis que describe cómo se lleva a cabo y se ejecuta un caso de uso determinado en términos de las clases del análisis y de sus objetos del análisis en interacción. Una realización de caso de uso proporciona por tanto una traza directa hacia un caso de uso concreto del modelo de casos de uso.
	- Diagrama de clases. 
	- Diagrama de interacción.
	- Flujo de sucesos-análisis.
	- Requisitos especiales: son descripciones textuales que coleccionan todos los requisitos no funcionales sobre una realización de caso de uso. 
4. **Paquete del análisis**:  los paquetes del análisis proporcionan un medio para organizar los artefactos del modelo de análisis *en piezas manejables*. Un paquete de análisis puede constar de clases de análisis, realizaciones de casos de uso, e incluso otros paquetes. Los paquetes del análisis deberían ser: Cohesivos o Débilmente acoplados. Además, los paquetes del análisis pueden representar una separación de intereses de análisis. Deberían crearse basándose en los requisitos funcionales y en el dominio del problema, y deberían ser reconocibles por las personas con conocimiento del dominio. Probablemente estos paquetes se conviertan en subsistemas futuros. 
	- ***Paquete de servicio***: son un tipo particular de paquete, proporcionado por el sistema al cliente, para que ofrezca a sus usuarios los casos de uso necesarios para llevar a cabo su negocio. Los paquetes de servicio contienen un conjunto de clases relacionadas funcionalmente. Estos paquetes son indivisibles, reutilizables, y son fundamentales para el diseño y la implementación.
5. **Descripción de la arquitectura**: (vista del modelo de análisis). Mediante la vista de la arquitectura del modelo de análisis podemos ver la descomposición del modelo de análisis en paquetes de análisis y sus dependencias; las clases fundamentales del análisis y las realizaciones de casos de uso.

#### Trabajadores

- **Arquitecto**: Es el responsable de la integridad y la arquitectura del modelo de análisis, garantizando que éste sea correcto, consistente y legible como un todo. El modelo de análisis es correcto si cumple con el modelo de casos de uso.
- **Ingeniero de Casos de Uso**: Es responsable de la integridad de una o más realizaciones de casos de uso, garantizando que cumplen los requisitos que recaen sobre ellos. Una realización de caso de uso debe llevar a cabo correctamente el comportamiento de su correspondiente caso de uso del modelo de casos de uso, y sólo ese comportamiento.
- **Ingeniero de componentes**: Se encarga de definir y mantener las responsabilidades, atributos, relaciones y requisitos especiales de una o varias clases y paquetes del análisis, asegurándose de que cada clase del análisis cumple con los requisitos que se esperan de ella de acuerdo a las realizaciones de caso de uso en las que participa.

Primer etapa
![[Pasted image 20250704124040.png]]

1.1 desglosado  
![[Pasted image 20250704123926.png]]