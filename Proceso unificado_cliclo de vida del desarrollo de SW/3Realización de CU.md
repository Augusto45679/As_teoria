Describe cómo se lleva a cabo un CU en función de las clases y los objetos que interactúan con él.

Cada realización corresponde con un CU → Todo CU tiene su realización (tiene 1 diagrama de clases y su diagrama de colaboración).

- El artefacto que da soporte a la trazabilidad a través de los modelos del proceso unificado es el CU.
- Una realización es un concepto abstracto, no un conjunto de diagramas ni documentación.
- _**Realización de diagrama de clases:**_ Relación entre CU a través de clases
- _**Realización de diagrama de colaboración:**_ Diagrama de clases + comunicación entre clases, siempre la interacción es en el patrón (actor, presentación, lógica de app, entidad)

### Paquete del análisis
Usadas para ordenar las partes del modelo del análisis → Encapsulamiento
### Descripción de la arquitectura
Todos los artefactos del modelo del análisis se integran en una única descripción → Vistas
### Producto y proceso

**Producto =** Resultado de un proceso
**Proceso =** Marco de trabajo el cual busca establecer orden y organización

_**Ingeniería de Software**_
**Capas**

![[Pasted image 20250704125340.png]]
**Fases**

- **Definición →** ¿ Qué funcionalidades, información se procesará, rendimiento, comportamiento, interfaces, requerimientos, criterios de control?
- **Desarrollo**
- **Mantenimiento →** Corrección, mejoras
- **Actividades Protectoras →** Garantía de calidad, gestión de riesgos (¿Qué puede fallar?), Reutilización

_**Todo proceso tiene**_

- **Actividades del marco de trabajo -** Tareas
- Hitos y entregables
- Puntos de garantía de calidad
- **Actos de protección**

**Estrategias de proceso**

- **Prototipos**
- **Reutilización →** _Bajo nivel:_ El módulo pertenece al mismo sistema (herencia, etc.) **o _Alto nivel:_ El módulo pertenece a otro sistema (bibliotecas, paquetes, etc.)