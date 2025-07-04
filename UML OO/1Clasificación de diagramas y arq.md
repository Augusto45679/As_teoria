Para leer este diagrama que está clasificado en tipos de vista (estática, dinámica, despliegue) y dentro de cada vista con los diagramas que se balancea (ej; vista estatica-> d.Clases) luego del diagrama viene la funcionalidad de dicho diagrama, o sea, una descripción. Luego de la descripción viene (lo ultimo, las hojas) de cada diagrama son los recursos que utiliza. 

![[Pasted image 20250703194807.png]]

## Mecanismos comunes

Los agregados a las reglas base y se hacen mediante patrones consistentes entre modelos

- **Especificaciones:** Explicación textual de los detalles de una gráfica. Ej. Especificación de CU
- **Adornos:** Agregados gráficos o textuales que aportan significado
- **Divisiones comunes:** Los objetos son instancias de clases, esta paridad se da con muchos elementos de UML. Las divisiones comunes permiten distinguir los elementos de sus instancias. Ej. Clases vs objetos (nombres subrayados).

## Mecanismos de extensibilidad

Para una extensión controlada y particularidades de lenguajes de programación.

- **Estereotipos:** *extensiones de vocabulario que permiten crear nuevos bloques de construcción a partir de los bloques estándar, específicos para el problema y el lenguaje*.

![[Pasted image 20250703200417.png]]
- **Valores etiquetados:** Etiquetas para añadir información o notas. _Va con lo de versión_
- **Restricción:** Etiquetas que imponen reglas o notas. _Va con lo de restricción_ 

![[Pasted image 20250703200502.png]]

## Arquitectura

“El proceso unificado es centrado en la arq.”

Artefacto para manejar distintos puntos de vistas de un sistema conjunto de “decisiones significativas” sobre la estructura lógica del sistema.

- Organización del sistema
- Selección de elementos estructurales y sus interfaces
- Comportamiento de elementos estructurales
- Composición de elementos estructurales
- Estilo arquitectónico (el estático, dinámico, interfaces)

Debe ser: _**robusta, flexible, mantenible y estable**_

La arquitectura es un conjunto de modelos organizados (en vistas) y consistentes que permiten tomar las dichas decisiones. Se realiza una descripción de Arq. que permite comprender la estructuración de los diagramas.

### Arq. genérica de UML

![[Pasted image 20250703200741.png]]

### Arq. del proceso unificado (descripión de la Arq.)

![[Pasted image 20250703200802.png]]
### Diagramos usudos

![[Pasted image 20250703200824.png]]
