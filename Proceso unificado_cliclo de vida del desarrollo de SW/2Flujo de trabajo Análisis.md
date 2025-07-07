**Fin:** Construir arquitectura del sistema = Tomar las decisiones fundamentales del sistema.

La arquitectura tiene una estructura lógica: análisis, refinamiento (aspectos internos) y estructura miento de requisitos (mejor compresión de estos, descripción mantenible centrado en CU). Y también se pregunta ¿Qué hará el sistema? 

![[Pasted image 20250704123659.png]]

![[Pasted image 20250704123926.png]]
![[Pasted image 20250704124040.png]]

Modelo de análisis: estructura miento de requisitos. Ordenando y dividiendo en paquetes (el de más nivel es el del sistema del análisis) jerarquizados. 

![[Pasted image 20250704124448.png]]

## Clases de análisis (componentes)

Retratan requisitos funcionales, definen atributos de alto nivel, se relacionan por relaciones conceptuales.
El objetivo de esta clasificación es distribuir las tareas del equipo.

- **Interfaz**    
    Comunicación entre el sistema y el actor (humano / dispositivo / otro sistema)
    - Interacciones: Mostrar información (GUI) solicitudes del actor al sistema y viceversa
    - Requisitos en el límite del sistema
    - Terminal boba
- **Control**
    Coordinación entre objetos que interactúan
    - Transacciones, derivaciones (salida del flujo normal), cálculos compejos
    - Aspectos dinámicos
    - No es persistente → solo se crea y existe cuando se ejecuta
    - Comprende el negocios y sus reglas
    - Se ocupan y asocian a cada uno de los CU

- **Entidad**
    Información y comportamientos estáticos (persistentes)
    - Parecido a un modelo de dominio, solo que las primeras modelan el problema y las segundas la solución.
    - Modeladas en diagrama de clases

![[Pasted image 20250704124712.png]]

![[Pasted image 20250704172724.png]]

![[Pasted image 20250704172730.png]]

![[Pasted image 20250704172735.png]]
