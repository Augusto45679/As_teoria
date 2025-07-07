El objetivo del proceso de ing. de requerimientos es *crear y mantener un documento de requerimientos del sistema*. El proceso general corresponde a cuatro subprocesos de alto nivel de la ing. de requerimientos. Una perspectiva alternativa sobre este proceso, es verlo como una actividad de tres etapas donde las actividades se organizan como un proceso iterativo alrededor de una espiral. La cantidad de dinero y esfuerzo dedicados a cada actividad en una iteración depende de la etapa del proceso general y del tipo de proceso generado.

Su fin es "documentar, administrar y gestionar requisitos del sistema".

![[Pasted image 20250703122527.png]]
El fin de la ingeniería en requerimientos es crear y mantener un documento de requerimientos del sistema. 

* **Gestión de requerimientos**: actualizar documentos cuando el sistema sufre cambios. 
* Su bien es auxiliado por métodos estructurados, cada captura de requisitos es distinta, pues supone el análisis de un sistema social. 

##### Estudio de viabilidad

Los resultados del estudio de viabilidad debería ser un informe que recomiende si merece o no la pena seguir con la ing. de requerimientos y el proceso de desarrollo del sistema. Un estudio de viabilidad es un estudio corto y está orientado a resolver varias cuestiones como: 
	• Si el sistema contribuye a los objetivos generales de la organización.
	• Si se puede implementar el sistema utilizando la tecnología actual y dentro de las restricciones de coste y tiempo.
	• Si puede integrarse el sistema con otros sistemas existentes en la organización.

Todo sistema debe empezar con esto, evaluar si: ¿Conviene desarrollar el sistema? ¿Contribuye a los objetivos de la organización? 

![[Pasted image 20250703123053.png]]
***Obtención de análisis de requerimientos***

En esta actividad, los ingenieros de software trabajan con los clientes y los usuarios finales del sistema para determinar el dominio de la aplicación, qué servicios debe proporcionar el sistema, el rendimiento requerido del sistema, las restricciones de hardware, etc. La obtención y análisis de requerimientos pueden afectar a varias personas de la organización. El término stakeholder se utiliza para referirse a cualquier persona o grupo que se verá afectado por el sistema.

* **Descubrimientos de requisitos** (entrevistar, escenario. Obtención de requisitos de cada stakeholder) y **análisis** (ponerlos a pruebas para encontrar problemas).
* También es posible de clasificar a partir de Arquitectura del sistema. 
* **Clasificación y organización**: clasificación de "puntos de vista" 
	* stakeholders interactuadores
	* stakeholders indirectos (no usan el sistema pero influyen)
	* stakeholder del dominio (restricciones, estándares)
* **Ordenamiento por prioridades y negociación** (ante desacuerdos entre stakeholders) **de requerimientos**. 
* **Documentación de requerimientos**.

> El término "**stakeholder**" se utiliza para referirse a *cualquier persona o grupo que se verá afectado por el sistema, directa o indirectamente*. Entre ellos, se encuentran los usuarios finales que interactúan con el sistema y todos aquellos en la organización que se pueden ver afectados por sus instalación. 

##### Validación de requerimientos. 

Trata de mostrar que los requerimientos realmente definen el sistema que el cliente desea. Es importante debido a que los errores en el documento de requerimientos pueden conducir a importantes costos al repetir el trabajo cuando son descubiertos durante el desarrollo o después de que el sistema esté en uso. El costo de arreglar un problema en los requerimientos haciendo un cambio en el sistema es mucho mayor que reparar los errores de diseño o los de codificación. Durante el proceso de validación de los requerimientos, se deben llevar a cabo verificaciones sobre requerimientos en el documento de requerimientos. Estas verificaciones comprenden: verificaciones de validez, de consistencia, de completitud, de realismo, para reducir discusiones con el cliente. Pueden utilizarse, en conjunto o de forma individual, varias técnicas de validación de requerimientos:
	• **Revisiones de requerimientos**: Los requerimientos son analizados sistemáticamente por un equipo de revisores.
	• **Construcción de prototipos**: Es este enfoque de validación, se muestra un modelo ejecutable del sistema a los usuarios finales y a los clientes. Éstos pueden experimentar con este modelo para ver si cumple sus necesidades reales.
	• **Generación de casos de prueba**: Los requerimientos deben poder probarse. Si las pruebas para estos se conciben como parte del proceso de validación, a menudo revela los problemas en los requerimientos.

¿Los requisitos verdaderamente definen lo que el cliente desea? 

![[Pasted image 20250703124109.png]]


**Requisitos**
- _Duraderos:_ dominio del sistema y reglas de negocio
- _Volátiles:_ cambian durante el desarrollo de SW
	- Cambiantes: Porque el sistema cambia
	- Emergentes: Los descubrimos en el sistema durante el proceso
	- Consecuentes: De la implementación
	- De compatibilidad

##### Gestión de requerimientos
En casi todos los sistemas los requerimientos cambian con el tiempo. La gestión de requerimientos es el proceso de comprender y controlar los cambios en los requerimientos del sistema. Desde una perspectiva evolutiva, los requerimientos se dividen en 2 clases:

1- **Requerimientos duraderos**: son requerimientos relativamente estables que se derivan de la actividad principal de la organización y que están relacionados directamente con el dominio del sistema.
2- **Requerimientos volátiles**: son requerimientos que probablemente cambian durante el proceso de desarrollo del sistema o después de que éste se haya puesto en funcionamiento. Ej.: políticas gubernamentales. Se clasifican en:
	a) *Req. Cambiantes*: están afectados por el entorno de la organización.
	b) *Req. Emergentes*: emergen al incrementarse la comprensión del cliente en el desarrollo del sistema.
	c) *Req. Consecuentes*: son el resultado de la introducción del sistema informático. El sistema puede cambiar la forma de trabajar en la organización, y esto genera nuevos requerimientos.
	d) *Req. De Compatibilidad*: dependen de otros sistemas presentes en la organización.