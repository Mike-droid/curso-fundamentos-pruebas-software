# Curso de Fundamentos de Pruebas de Software

## Introducción al curso

### Introducción

### ¿Qué son las pruebas y por qué deberíamos hacerlas?

Si brindamos una mala experiencia de usuario, estos no usarán nuestra aplicación.

Como principio de **ética**, nuestra aplicación ***NO*** debe llegar con errores al usuario final.

Un prueba es el proceso de *evaluar un producto*, aprendiendo a través de *la exploración y experimentación*. Esto incluye:

- Cuestionar
- Estudiar
- Modelar
- Observar
- Inferir
- Checar salidas de datos
- Etc.

Entre menos entiendas el producto que estás desarrollando, *más errores* va a tener.

Nunca tendrás un software 100% libre de errores. Tienes que estar actulizando tu software con el tiempo debido a la rápidez con que avanza la tecnología.

Las pruebas las puedes tener que hacer por razones como:

- Costo
- Prestigio
- Legales
- Mejorar el software en sí
- Seguridad (*y esta es MUY importante*)

3 razones muy buenas para hacer pruebas:

1. Tenemos un problema o el resultado no es el esperado
2. Costo alto o fuera de presupuesto
3. Implicaciones legales o de estándares tecnológicos

**Definición del testing según la IEEE:**
El proceso de funcionamiento de un sistema o componente bajo ciertas condiciones, observar o registrar los resultados, y hacer una evaluación de algún aspecto del sistema o componente.

### Proceso de pruebas del software y los estándares internacionales

Cuando estamos haciendo software debemos tener:

- Recursos => Si no estás preparado, las carencias se irán mostrando como defectos.
- Metodologías => Aquí establecemos el criterio o la estrategía de cómo vamos a llevar a cabo las pruebas.
- Herramientas => Contar con las herramientas adecuadas permitirá acelerar la identificación, documentación y comunicación de los problemas.

Según IBM, el 64% de los errores del proyecto se producen en la etapa de diseño y análisis (y las pruebas son Requisitos, Diseño, Código, Pruebas y Explotación).

Es importante saber lo que el cliente quiere, pues de no ser así haremos un producto que no cumpla las necesidades del cliente.

#### Calidad de software

- Calidad del producto
  - Calidad del producto -> Lo que la gente requiere
    - Requerimientos
    - Diseño
    - Código
    - El sistema
  - Calidad del proceso -> Cómo lo hace la gente
    - Estándares
    - Procedimientos
    - Procesos del proyecto

Recuerda: **POR ÉTICA DEBES TENER UN PRODUCTO DE CALIDAD, ES DECIR, ALGO QUE FUNCIONA.**

Estándares:

- ISTQB (International Software Testing Qualifications Board)
- IEEE (Institute of Electrical and Electronics Engineers)
- TPI (Testing Process Improvement)

### Ciclo de vida del software

A lo largo del ciclo de vida del software se realizan distintas pruebas para garantizar que este cumpla con los requerimientos para los que fue diseñado y de la misma forma se encuentren procesos de mejora y optimización a medida que se desarrolla el software.

- Es necesario hacer pruebas en todas las fases del desarrollo de software ya que un error encontrado en una etapa tardía puede generar costos muy elevados.
- Errores detectados lo antes posible reducen los costos y son mucho más fáciles de corregir.
- El ciclo de vida permite que los errores se detecten lo antes posible y por lo tanto, permite a los desarrolladores concentrarse en la calidad del software, en los plazos de implementación y en los costos asociados.

El ciclo de vida básico de un software consta de los siguientes procedimientos:

1. Definición de objetivos -> En esta fase se define el alcance general del software y su papel dentro de una estrategia global o dentro del ecosistema que va a funcionar.
2. Análisis de los requisitos y su viabilidad -> Se trata de recopilar la mayor cantidad de información posible para evaluar la viabilidad del producto, encontrar posibles restricciones y analizar todos los requisitos del cliente.
3. Diseño (Alto y Bajo nivel) -> *Alto nivel*: Se trata de realizar un diseño básico que valide la arquitectura de la aplicación. *Bajo nivel*: Es una definición detallada de la estructura de la aplicación basada en el diseño general.
4. Programación -> Es la implementación de un lenguaje de programación para crear las funciones definidas durante la etapa de diseño.
5. Pruebas de verificación -> Aunque en todas las fases anteriores se hacen pruebas en esta fase se cubren: pruebas de componentes, integrales y de sistema.
6. Prueba beta (o validación) -> Se hace para garantizar que el software cumple con las especificaciones originales o también se hacen las pruebas de aceptación.
7. Implementación -> Se realiza una prueba del sistema implementado para encontrar posibles fallas en la Implementación.
8. Mantenimiento -> Se hace para todos los procedimientos correctivos (mantenimiento correctivo) y a las actualizaciones secundarias del software (mantenimiento continuo), junto con la actualización de las pruebas.
9. Volver al paso #1

Si hacemos las pruebas durante cada fase del ciclo de vida del software tendremos al final del ciclo un producto validado y robusto de acuerdo a las necesidades del cliente.

### Proceso de pruebas del software: Calidad y Defectos

La calidad es una percepción entre lo deseado, lo analizado y lo que vamos a entregar. Pero esta definición puede cambiar de
persona en persona, así que la calidad la define el cliente.

> El grado con el que un sistema, componente o proceso cumple con los requisitos especificados y las necesidades o expectativas
del cliente o usuario.

IEEE.Std.610-1990

*Verificación*: En cada una de las etapas hay que revisar que se cumpla lo que el cliente pidió.

*Validación*: Al final, antes de entregarle al cliente, validamos que lo que entregamos cumple con todos sus requerimientos.

Conceptos importantes negativos:

- *Anomalía*: Cualquier condición insatisfactoria.
- *Defecto*: No desempeña funciones.
- *Fallo*: Incapacidad dentro de márgenes.
- *Error*: Acción humana incorrecta.

> El **error** humano cometido inyecta un defecto en el software que, ocasionalmente, se observa como una **anomalía** a causa de
un comportamiento  incorrecto, no acorde a lo especificado, que finalmente provoca el **fallo** del sistema de software.

### Principios del testing moderno

El tester debería de enfocarse en la calidad del producto, del proceso.

El desarrollador debería enfocarse en desarrollar la aplicación.

Entonces el tester ayudará al desarrollador con las mejores herramientas de desarrollo.

#### 7 principios del testing moderno

> Los testers podemos comenzar a pasar de ser los dueños de las pruebas o la calidad, a ser los embajadores de la calidad del producto.

1. Nuestra prioridad es mejorar el negocio.
2. Nosotros aceleramos al equipo, usamos modelos como **Lean Thinking** y **Teoría de las Restricciones** para ayudar a identificar, priorizar y mitigar cuellos de botella en el sistema.
3. Somos la fuerza para la mejora continua, ayudando al equipo a **adaptarse y optimizar** para tener éxito, en lugar de proporcionar una red de seguridad para detectar fallas.
4. Nos preocupamos profundamente acerca de la **historia de calidad** en el equipo, y asesoramos, lideramos y nutrimos el equipo para llevarlos a una cultura de calidad más madura.
5. Nosotros creemos que el cliente es el único capaz de **juzgar y evaluar** la calidad de nuestro producto.
6. Nostros usamos **datos de manera extensa y profunda** para entender los casos de uso del cliente y entonces cerrar huecos entre hipótesis del producto e impacto del negocio.
7. Expandimos las habilidades de testing y el conocimiento en **todo el equipo**; entendemos que esto reduce o elimina la necesidad de un especialista dedicado al testing.

### Especialidades del testing

- Manual Tester -> Nos ayuda a definir los casos de prueba, a establecer estrategia. Planea y organiza.
  - Skill: Pensamiento lateral
- Automation tester -> Agilia el trabajo y las actividades.
  - Skill: Programación
- Security Tester -> Evita que roben y alteren datos, que personas no autorizadas entren a sitios restringidos.
  - Skill: Protocolos y estándares
- Data Science Tester -> Organiza datos, analiza.
  - Skill: Análisis y limpieza de datos
- SDET -> Software Development Engineer in Test. Sabe hacer pruebas para todo el proceso del software.
  - Skill: Integración continua
- DevOps -> Conoce todo lo anterior
  - Skill: Entrega continua
- QA Engineer -> Quality Assurance, enfocado en el producto y en el proceso.
  - Skill: Procesos de calidad
- QE -> Quality Engineer, es como un coach y acompaña en las políticas de la empresa.
  - Skill: Soluciones y estrategias de calidad

Y probablemente habrá más.
