El paradigma OO (Orientado a Objetos) encierra una _completa visión_ de la ingeniería de SW que fortalecen los beneficios de implementar esta tecnología.

_Completa visión =_

- **AROO =** Análisis de requisitos OO (Orientado a Objetos)
- **DOO =** Diseño OO
- **ADOO** = Análisis del dominio OO
- **POO =** Programación OO
- **SGBDOO** = Sistema de gestión de base de datos OO
- **ISOOAC** = Ingeniería de SW OO asistida por computadora
- **PrOO** = Pruebas OO 

### Características
- Reutilización de recursos (_ensamblaje_)
- Estructura (para sistemas evolutivos) inherentemente _descompuesta_ 

![[Pasted image 20250703131356.png]]
### Clasificación
- **Anulación de atributos:** Heredados de manera normal peor notificados según las necesidades de la subclase.
- **Clase abstracta:** Aquella que carece de objetos sino que solo sirve para ser heredada.
- **Herencia múltiple:** Hereda de + de una clase, complica la jerarquía y el control. 

![[Pasted image 20250703131443.png]]
### Encapsulamiento

Contener información en un paquete reutilizable de nombre específico.

_**Supone:**_

- **Alta cohesión** → Grado en que los elementos de un módulo permanecen juntos
- **Bajo acoplamiento** → Forma y grado de interdependencia entre módulos.
- **cohesión** → - acoplamiento

> Las clases se “autoabastecen” porque agrupan todos los datos que requieren y todas las operaciones que puedan afectarlos.

_**Ventajas:**_
- Ocultamiento de información → reduce propagación de efectos colaterales.
- Reutilización de componentes.
- Interfaces entre objetos simplificados.
### Polimorfismo
Operaciones distintas con mismo nombre → - acoplamiento