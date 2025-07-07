Un modelo es una representación, en cierto medio, de algo en el mismo u otro medio. El modelo capta los aspectos importantes de lo que estamos modelando, desde cierto punto de vista y simplifica u omite el resto.
Un modelo de sistema software está construido en el lenguaje de modelado UML, tiene semántica y notación y puede adoptar varios formatos que incluyen texto y gráficos. El modelo pretende ser más fácil de usar para ciertos propósitos que el sistema final. Un sistema de software puede ser representado por múltiples modelos, cada modelo ofrece una visión parcial del sistema. No hay que confundir los modelos con el sistema.
***SIRVEN PARA***
• Captar y enumerar exhaustivamente los requisitos y el dominio de conocimientos, de forma que todos los implicados puedan entenderlos y estar de acuerdo con ellos.
• Pensar el diseño de un sistema.
• Capturar decisiones del diseño en una forma notable a partir de los requisitos.
• Generar productos aprovechables para el trabajo.
• Organizar, encontrar, filtrar, recuperar, examinar y corregir la información en grandes sistemas.
• Explorar económicamente múltiples soluciones.
• Domesticar los sistemas complejos.

---
#### **Modelo**

* Representación de una realidad (abstracta) parcial de forma simplificada.
* Representación de un medio(mismo de realidad o uno distinto)
* Representación semántica y notación (presentación visual que no aporta significado e incluye info textual e hipervínculos)
* Representación de un modelo de SW, se construye en un lenguaje de modelado.
	En un sistema los modelos son llamados artefactos

UML: unified modeling language

* ***Objetivos***: 
	* Comprender el problema → Captar y enumerar exhaustivamente los requisitos y el dominio de conocimiento para que los implicados puedan entenderlos y ponerse de acuerdo y fraccionar el problema en interacciones.
	- Pensar el diseño y explorar varias soluciones.
	- Toma de decisiones.
	- Cálculo de costos (tiempo y dinero) → Explorar costos de muchas soluciones.
	- Organizar, encontrar, filtrar, recuperar, examinar y corregir la información de grandes sistemas.
	- **CLASIFICACIÓN**: 
		1. Guías de pensamiento → Explorar opciones;  *los modelos de alto nivel construidos al principio del proyecto, sirven para enfocar el proceso del pensamiento de los participantes y destacar determinadas opciones*.
		2. Especificaciones abstractas de estructura esencial: los modelos en el análisis o las etapas preliminares del diseño se centran en los conceptos y mecanismos claves del sistema.
		3. Especificaciones completas de todo el sistema:  un modelo de implementación incluye suficiente información para construir el sistema.
		4. Prototipos
		5. Descripciones completas o parciales
* ***Contexto***: 
	Se usa para auxiliar un flujo de trabajo específico. A este se denomina contexto. Ej: Diagrama de clases conceptuales → Contexto: Análisis de sistemas.
	* Hay puntos donde un modelo puede interpretarse de muchas formas, allí se pueden contemplar varios modelos de ejecución
	- La especificación se modela por separado de la implementación.
	- Los modelos describen instancias. Una cosa es descripción o instancia en referencia a otra cosa, por que algunos pueden ser ambas según la perspectiva. Se los llaman metadatos. 

Metamodelo: especifica reglas de un lenguaje de modelado para un modelo bien formado. 

### Metamodelo de captura de requisitos 

Un metamodelo es la descripción de un modelo. Un lenguaje de modelado describe modelos; por lo tanto, puede ser descrito por un metamodelo. Un metamodelo procura hacer un lenguaje exacto, definiendo su semántica, pero hay una tensión para permitir las extensiones para nuevas situaciones. La forma real del metamodelo es importante para la implementación de las herramientas, y el intercambio de modelos. El metamodelo UML define la estructura de los modelos UML.

El metamodelo está dividido en **tres paquetes principales**.
• El paquete de fundamentos define la estructura estática de UML.
• El paquete de elementos de comportamiento define la estructura dinámica de UML.
• El paquete de administración del modelo define la estructura organizativa de los modelos de UML.

![[Pasted image 20250703125759.png]]
*Un modelo completo debe tener valores en todos sus elementos (algo real por cada caso abstracto) → a veces null es un valor válido.*

