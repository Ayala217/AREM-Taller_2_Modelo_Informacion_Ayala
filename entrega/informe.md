#  Informe Técnico del Taller

##  Nombre del Taller
Taller 2 Modelo de Información

##  Integrantes del equipo para la segunda parte del taller
- Juan Sebastián Ayala (juanaysi@unisabana.edu.co)
- Camilo Arciniegas Guerrero (camiloarcgu@unisabana.edu.co)
- Juan Diego Campo (juancamco@unisabana.edu.co)

##  Descripción general del trabajo
Crear Modelos ER y diagramas de contexto para mejorar el entendimiento del negocio cliente que se manejará a lo largo del semestre.
Se siguieron las intrucciones del profesor dadas en clase y también se buscaron más ejemplos en internet para crear el modelo 
y el diagrama.

##  Proceso de desarrollo
Se elaboró el **modelo entidad–relación (ER)** y el **diagrama de contexto**, con el fin de representar la estructura de datos y la interacción del sistema con su entorno. Se identificaron las entidades principales que soportan la operación: Cliente, Pago, Clase y Asistencia, las cuales permiten registrar la compra de clases, la programación de sesiones y el control de asistencia. Asimismo, el diagrama de contexto permitió visualizar la interacción entre los cuatro actores del proceso —clientes, gimnasio, el sistema de registro (Excel) y el banco— y el flujo de información entre ellos. Ambos modelos fueron desarrollados en draw.io para garantizar una representación clara y coherente con el funcionamiento real del gimnasio.


##  Análisis del modelo propuesto
Incluya un análisis sobre:
- Cómo se estructura el modelo entregado
  El modelo entregado se estructura de forma que el cliente puede pagar muchas clases (las que vaya a asistir ese mes) y
  también puede asistir a muchas clases (siempre y cuando sea el mismo mes y no se pase del número que adquirió). 
- Cómo representa las necesidades del cliente
  Las necesidades se representan en sentido de que toca manejar las asistencias y pagos uno por uno, pues esto se puede automatizar muy sencillo
  pero el cliente aún lo hace manualmente.
- Qué supuestos se tomaron
  Se supuso que todos los clientes del gimnasio han firmado autorizaciones de tratamiento de datos personales y exoneración de responsabilidad.

##  Diagrama final entregado
> Diagrama de contexto:
<img width="651" height="297" alt="diagrama-contexto-final drawio" src="https://github.com/user-attachments/assets/9dd4bc6e-0aae-4000-a004-d6810aacf957" />


> Modelo ER:

![modelo-final-er drawio](https://github.com/user-attachments/assets/499e131d-4c6f-4cfe-a356-7321e778e04d)

##  Tabla de actores, entidades o componentes (si aplica)

| Nombre del elemento              | Tipo                 | Descripción                                                                 | Responsable                |
|-----------------------------------|----------------------|-----------------------------------------------------------------------------|----------------------------|
| Cliente                           | Entidad              | Persona inscrita en el gimnasio con datos básicos como nombre, teléfono y correo. | Recepción / Administración |
| Pago                              | Entidad              | Registro de pagos realizados por los clientes, incluyendo fecha y clases compradas. | Recepción                  |
| Clase                             | Entidad              | Clase ofrecida por el gimnasio con información de fecha, hora y capacidad. | Entrenador / Administración |
| Asistencia                        | Entidad asociativa   | Registro de la asistencia de un cliente a una clase específica, incluyendo evidencia fotográfica. | Entrenador                 |
| Clientes                          | Actor         | Imparte la clase y valida la asistencia de los clientes. | Gimnasio                    |
| Entrenador                  | Actor      | Herramienta utilizada para almacenar y actualizar información administrativa y control de clases restantes. | Gimnasio             |
| Personal administrativo del gimnasio                  | Actor      | Recibe el pago, registra información en el sistema y gestiona el cierre mensual. | Gimnasio             |


##  Investigación complementaria
### Tema investigado:

###¿Qué es el diagrama ERD?

El modelo Entidad–Relación se creó como una forma de organizar ese proceso. Al trabajar con entidades, atributos y relaciones, el ERD permite “dibujar” de forma sencilla y gráfica la estructura del sistema. De esta forma, se puede observar claramente cómo se relacionan los datos y qué papel tiene cada uno de los elementos de la relación.

A pesar de elaboraciones posteriores y de las nuevas metodologías que han ido surgiendo, el ERD se mantiene como una de las herramientas más utilizadas. Su valor radica en que hace pensar antes de programar, estructurar antes de implantar. A su vez, permite comunicar a los que analizan el negocio con los que desarrollan el sistema, haciendo que ambos lleguen a “hablar” el mismo idioma a la hora de organizar la información.[1]

### Contexto en casos reales de la industria

**1. Comercio digital**

Un ejemplo de empresa que utiliza el modelo ERD para la estructuración de sus sistemas es Amazon, pues lo utilizan para estructurar y organizar millones de registros de productos, clientes y pedidos. Este diseño les permite identificar puntos críticos donde el sistema debe maximizar su eficiencia para dar con el mejor rendimiento en la aplicación.[2]

**2. Sector Bancario**

Las Entidades financieras  operan con arquitecturas de datos altamente complejas que deben soportar millones de transacciones diarias, múltiples canales digitales y regulaciones financieras. En este contexto, el modelado conceptual mediante ERD se convierte en una etapa fundamental antes de implementar cualquier sistema transaccional.[3]

**3. Sector Sanitario**

De forma similar a las entidades financieras, las organizaciones de salud necesitan operar con una gran cantidad de operaciones diarias, tales como consultas de historias clínicas, agendamiento de citas...etc. Por lo que también implementan el modelo ERD en las fases de diseño para obtener una estructura óptima del sistema.
  
### Resumen:

El modelo ERD surgió cuando se comenzó a darse cuenta de que no tenía mucho sentido diseñar bases de datos y sistemas de negocio sin antes comprender bien qué tipo de información se estaba manejando y cómo se relacionaba entre sí. A medida que los sistemas iban creciendo y volviéndose más complejos, también iban creciendo los errores y la desorganización si no había una estructura clara desde el principio. Por eso se necesitaba separar la idea del sistema de la parte técnica, y el ERD vino a surgir como una forma fácil y visual de hacerlo.

Con el tiempo, este modelo dejó de ser solo una teoría y pasó a ser utilizado en diferentes ámbitos como el sector bancario, la salud o el comercio digital, donde es fundamental manejar bien los datos. De esta forma, una mala estructuración puede llevar a sistemas ineficientes y afectar procesos críticos de una organización.

Gracias a la investigación realizada, se pudo aplicar de forma adecuada el modelo ERD  en el caso de la Clínica Salud Viva, pues se logró identificar correctamente las entidades principales, sus relaciones y los flujos de información entre actores y sistemas para construir tanto el ERD como el diagrama de contexto. En siguiente lugar, esa misma base conceptual fue de gran ayuda para el modelo ERD y de contexto para el caso real del gimnasio, de forma que se definieron con claridad las entidades y su comportamiento dentro de la lógica de negocio. En definitiva, la investigación fue clave para desarrollar ambos casos de forma correcta y con certeza de que se estaba modelando bajo los estándares de ERD. 


##  Referencias
[1] P. P.-S. Chen, “The Entity-Relationship Model—Toward a Unified View of Data,” ACM Transactions on Database Systems, vol. 1, no. 1, pp. 9–36, Mar. 1976. [En línea]. Disponible en: https://doi.org/10.1145/320434.320440

[2] Using DynamoDB as a data store for an online shop, Amazon Web Services, 2025. [En línea]. Disponible: https://docs.aws.amazon.com/amazondynamodb/latest/developerguide/data-modeling-online-shop.html

[3] E. Cadavid Rodríguez et al., Desarrollo de una aplicación web adaptativa para el despliegue de información asociada a la capa aplicativa del modelo de referencia de la arquitectura actual y objetiva de la empresa Bancolombia, Universidad de Antioquia, Mar. 2021. [En Línea]. Disponible: https://hdl.handle.net/10495/23110

---

_Este documento hace parte de la entrega del taller X del curso AREM (Arquitectura Empresarial) - Universidad de La Sabana._
