Resulta común que los diagramas transiten entre los distintos flujos de trabajo (análisis, diseño,…) evolucionando.

![[Pasted image 20250704174233.png]]
- Colabora a la formación del diagrama de clases del diseño, pueden elaborarse en el mismo periodo e irse retroalimentando mutuamente.
- Usa clases y relaciones estructurales
- Completa métodos, atributos y visibilidad (se añade según destinario y uso), tipo atributos, se añade según si hace falta por contexto.
- Agrego navegabilidad y dependencias.

## Navegabilidad

Posibilidad de navegar unidireccionalmente en una asociación, de un objeto a otro.

![[Pasted image 20250704174415.png]]
- A crea una instancia de B
- A envía mensajes a B (actualizar, obtener info)
- A necesita mantener una conexión con B (Ej: persona → empresa)
--- 
- El extremo de una asociación es un rol y se dice que la navegabilidad es una propiedad del rol. A → (utiliza) B
- “La navegabilidad depende de las reglas del negocio” → ¿Qué nos interesa conocer? Detectar la clase corazón del sistema. (core) (¿Qué clase debe existir para que exista el negocio?, el cliente nunca es core) y accesos cubiertos por métodos y aparecen en especificaciones de CU.
- Diagramas de interacción, comportamiento, secuencia, permiten analizar el flujo de mensajes → métodos.
- A → B → C Si A accede a C, agregar métodos en B que lo permitan.
- La cardinalidad no influye a la hora de determinar la dirección de una navegabilidad.

#### Traspaso de diagrama de clases
![[Pasted image 20250704174457.png]]

A toda clase se le agrega un atributo identificador → El primer atributo de la lista cuando ese no sea obvio, si una clase es abstracta puede no tener el identificador

La generalizaciones se representan igual y suponen que la superclase accede a la subclase