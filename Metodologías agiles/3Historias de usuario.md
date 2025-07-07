- Usadas en las metodologías ágiles para especificar y administrar los requisitos.
- Descripción breve del sistema desde la perspectiva del usuario.
- Historia de usuario **≠** CU **≠** requisitos funcionales → Describen qué requiere el usuario, no cómo el sistema satisfará la necesidad.

Los requisitos se administran mediante tarjetas

1. **Card:** Requerimiento escrito en el lenguaje del usuario, tal y como esto lo demuestra → Se obtiene de relevar a los clientes.
2. **Conversation:** Entre el desarrollador y el product owner analizar la card elaborada → la conversación es el futuro medio de validación.

- CU: Participan stakeholders y analistas. Historias: Participa todo el equipo + stakeholders.

3. **Confirmation:** A través de criterios de validación el product owner confirma el desarrollador que ha entendido la necesidad.

- Se dice que la card es una promesa de conversación, porque se conversa con el cliente para validarlo.
- Las historias de usuario son cortas, fáciles de implementar, necesitan poco mantenimiento y permiten dividir el proyecto en pequeñas entregas.
- Ayudan a mantener una relación cercana con el cliente.
- Facilitan estimar el esfuerzo del desarrollo.
- Ideales para proyectos de requisitos volátiles o no muy claros.

![[Pasted image 20250704175510.png]]

Las h. uso se descomponen (dividen) en tareas y las unidades de tamaño adecuadas para su ejecución y gestión.

Las ideas del usuario se van desglosando en temas → épicas → …

La pila de producto se ordena por prioridad. Determinada por el product owner, los más prioritarios se detallan más y las historias de usuario se priorizan sobre las épocas 


### Card
Trata de evitarse la rigidez. Además de los 4 campos (componentes obligatorios) principales puede añadirse lo que sea.
- **Titulo**
- **ID:** identificador numérico
- **Descripción:** Síntesis normalmente narrativa.

![[Pasted image 20250704175917.png]]
- **Estimación:** Tiempo ideal para implementar → El equipo a veces emplea “puntos” _(puntos de historia)_ (si un puntos son 2 días, puede estimársele 2 puntos)
- **Prioridad:** Determinadas por el product owner y el equipo al comparar distintas historias y se les asigna un número mediante los cuales se da el orden en que se implementan
- Un criterio para determinar prioridad es cuándo estos se usarán para ver que priorizar.
- **Validación:** Criterios de calidad (qué chequear), pruebas de aceptación, qué debe cumplir el resultado obtenido y verificaciones del sistema. Criterios deben ser → S (pecific) M(easurable) A(rchievable) R(elevant) T(ime boxed _limitado en tiempo_)
- **Valor:** Se le asigna un valor numérico que se representa cuán importante para el usuario.
- **Riesgo de desarrollo:** ¿Cuán probable es que ocurra un evento que afecte al desarrollo? ¿Cómo lo afectarán? 

Puede especificarse el módulo al que pertenece la historia y de qué otras historias dependen.
Una historia debe ser (método para asegurar la calidad).

INVEST

**I**ndependent ->
**N**egotiable
**V**aluable -> resultado valioso para el cliente.
**E**stimable -> suficientemente concreta para que el cliente pueda hacer estimaciones relevantes.
**S**mall -> de unas semanas, limitadas a la duración. 
**T**estable

### User story mapping (mapeo de historias de usuario)

La necesidad se relata en actividades secuenciales (de forma horizontal) cada una se divide en opciones (de forma vertical).
Los resultado del mapeo con historias de usuario. El hecho de haber mapeado una historia en otras hace que la primera se vuelva una épica.

![[Pasted image 20250704180322.png]]

#### Criterios de aceptación ***SMART***

Se debe cumplir con los siguientes criterio SMART

No deben ser redundantes con la descripción de la historia de usuario. Hay que tener también ciertas consideraciones como, qué se requiere para que funcione (MO: Quiero comprar ticket para espectáculo, entonces el usuario debe estar registrado y el usuario debe seleccionar el espectáculo, siempre seleccionando o completando los datos requeridos y llevar una frecuencia de actualización.) y que no puede ocurrir. También deben estar contadas en el objetivo de la HU, no es las opciones futuras.

Se puede escribir con lenguaje natural o de Gherkin o por comportamiento en escenarios (BDD)

#### Lenguaje de Gherkin

Número de escenario → pues puede haber varias alternativas
En caso de que… (contexto) Entonces…

#### Priorización de historias de usuario

Prioridad es distinto a lo valioso para el cliente. Entonces:
1. ¿Cuán necesario es para el funcionamiento del cliente?
2. ¿Cuándo lo queremos?
3. ¿Es necesaria, recomendable?

Utilizando la escala ***MSCW*** :

**M**ust have (this function)
**S**hould have
**C**ould have
**W**on’t have → maybe later, but isn´t relevant right now

### División de historias de usuario

**División horizontal:** Según tipo de trabajo, tecnología → No es recomendable porque se obtiene historias sin valor de negocio.

**División vertical:** Cómo cliente quiero buscar productos para verlos. _Ej: Cómo cliente quiero buscar según precio para… / como cliente quiero buscar según color para…_

Cuando una HU se divide verticalmente, cada una de las hijas puede tener o no los criterios de aceptación de la madre.