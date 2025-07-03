
Sirve para 
* Visualizar
- Especificar → Modelos no ambiguos
- Construir → Código a partir de modelo (ingeniería directa) o ingeniería inversa para documentar y mejorar, o simular funcionamiento
- Documentar → Generar registros

**UML** es un lenguaje de enfoque orientado a objetos.

### Elementos estructurales

1. **Clase**
	Conjunto de objetos (el objeto cliente representa todos los clientes) que comparten los mismos atributos, operaciones (métodos), relaciones y semántica. 
	- - atributo público
	- '#' atributo protegido
	- - atributo privado 
	![[Pasted image 20250703130227.png]]
2. **Caso de uso**
	Porción de funcionalidad, descripción de un conjunto de secuencias de acciones que un sistema ejecuta y que produce un resaltado observable de interés para un actor particular.
3. **Interfaz**
	Colección de operaciones (signatura, iconos de operaciones ≠ implementación) que especifican un servicio de una clase o un componente
4. **Colobaración**
	Interacción, sociedad de roles y otros elementos que cooperan sinérgicamente
5. **Estereotipos**
	Etiquetas para catalogar elementos. Son símbolo o se escriben entre << …. >>

### Elemento de comportamiento 

1. **Interacción** 
	Mensajes entre objetos que desencadenan acciones ![[Pasted image 20250703130929.png]]
2. **Maquina de estados**
	Secuencia de estados por las que pasa un objeto o una interacción → Especificación de un comportamiento (por ejemplo una clase) a través de estados, transiciona entre estos eventos y actividades.
	![[Pasted image 20250703130959.png]]
3. **Actividad** 
	Secuencia de pasos que ejecuta un proceso computacional 
	![[Pasted image 20250703131043.png]]

#### Agrupación 
Mecanismo de propósito general para agrupar por paquetes de grupos

![[Pasted image 20250703131156.png]]

## Relaciones

![[Pasted image 20250703131233.png]]
## Diagrama

Representación gráfica con significado, usado para contemplar un sistema desde distintas perspectivas

- Diagrama de paquetes → relaciones entre subsistemas

## Reglas de UML

Reglas semánticas para lograr modelos bien formados

UML tiene reglas que restringen:

- **Nombres** → Cada uno tiene sintaxis y semántica específica
- **Alcance** → Contexto en que se encuentra determina el significado de un nombre
- **Visibilidad** → Qué signos se usan, como se ven los signos
- **Integridad** → Cómo se relacionan los elementos apropiada y consistentemente
- **Ejecución** → Pautas para simuladores y modelos dinámicos

Modelos que capturan sólo lo esencial y no provocan confusiones. Abreviados, incompletos, inconsistente

