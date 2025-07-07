# Diagrama de transición de estados (state machine)

Representan el _ciclo de vida de un objeto de clases_ **≠** clase → las clases son solo patrones, los que guardan información e interactúan con los objetos.

- Todo objetos puede tener su diagrama de estados, sin embargo, solo se hace diagramas de los + relevantes.
- **Estado:** Determinado por los valores de los atributos de un objeto.
- Un diagrama de estados está conformado por máquinas de estados.
- Un diagrama se corresponde con un único objeto, se ignora lo que ocurre con los estados de los demás.
 
![[Pasted image 20250704173459.png]]

#### Estados
Se enuncian con adjetivos. Un estado puede en sí mismo ser un máquina de estados, es decir, puede contener otros estados. El súper estado se vincula a otros como si no tuviera subestados.

>💡  Todo estado debe tener una transición de entrada y salida

![[Pasted image 20250704173815.png]]

![[Pasted image 20250704173822.png]]

- Siempre hay 1 estado inicial (que se vincula a 1 único estado) y 1 o más estados finales
- A él estado final se vinculan aquellos estados en los que el objeto podría estar permanentemente.

### Transiciones

![[Pasted image 20250704173847.png]]
- Representan eventos = evento disparador / trigger
- Todas las transiciones excepto las del estado final (estas no usan ninguna etiqueta), **evento disparador = CU →** balanceo → Los estados deben aparecer en la especificación de CU.
- Las auto transiciones se incluyen dependiendo de si ponen acciones del sistema y si aclaran o no el diagrama.

#### Evento disparador (trigger)
Caso de uso que provoca la transición
- Conviene aclarar actor (enunciados como requisitos funcionales)
#### Condición de guarda (guard)
Debe darse para que se efectúe la transición
- Comúnmente se usa cuando un CU puede provocar una transición u otra según esta condición
#### Acción del sistema (effect)
Acciones relevantes pueden ser extensiones a otros CU
- Cuando un dato puede obtenerse de datos ya creados, no se incluyen acciones del sistema.


# Diagrama de paquetes
**Paquete**: Organizar elementos estructurales agrupándolos con el fin de ordenar y encapsular.

- Un elementos es exclusivo de un paquete. Si eliminamos este último, también eliminamos el otro.
![[Pasted image 20250704174112.png]]

- Todo caso de uso y clase debe estar un solo paquete.

#### Relaciones entre paquetes

![[Pasted image 20250704174128.png]]


- Dependencia: *un elemento requiere, usa uno de otro paquete*
- El agrupamiento abstrae los CU de su vínculo con el actor.
- A veces, cuando muchas clases usan una clase que solo existe para servicios, se crea un paquete llamado “servicios”.
- Un paquete puede contener otro paquete y otras clases.