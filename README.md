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

## Testing

### Presupuesto, Recursos, Tiempo y Actividades Clave

Cuando estamos desarrollando un software, tratamos de que esté listo para una fecha indicada. Pero la realidad es que muchas veces se alarga la espera por cuestiones humanas.

El ciclo de vida del software es:

1. Definición de necesidades
2. Análisis
3. Diseño
4. Codificación
5. Pruebas
6. Validación
7. Mantenimiento y evolución

Cada una de estas etapas puede tener sus pruebas.

**Ejemplo**: Análisis -> "El usuario puede iniciar sesión".

- ¿Cuántos usuarios pueden iniciar sesión?
- ¿Qué debería hacer el software tanto si inicia como si no inicia sesión?

Debemos tomar en cuenta estos detalles.

**Ejemplo**: Diseño -> Crear la pantalla de login/registro, formulario.

- ¿Cuántos caracterés aceptará para el nombre? ¿Cuántos para el apellido?
- ¿Solo aceptará letras o también otros símbolos como "#$%123"? ¿Pueden estar los campos vacíos?
- ¿Qué pasará si los datos son correctos? ¿Qué pasará si son incorrectos?

**Ejemplo**: Código -> Podemos tener módulos, funciones y bases de datos. Además de tener:

- Front end -> Normalmente tarda más que el backend y no podemos terminarlo de construir sin que el backend esté construido.
- Back end -> Podemos probar apis, bases de datos.

**Ejemplo**: Pruebas -> Podemos hacer pruebas de cómo se envía la información a la interfaz, de cómo el usuario interactura con el software, de los distintos dispositivos usando el software. Las pruebas están comprobando los requerimientos del cliente.

Las pruebas de validación o de aceptación son en donde el cliente nos dirá que aprueba lo que hemos desarrollado. Una buen práctica es mostrar nuestros avances para tener su feedback. Una mala práctica es esperar hasta el final.

### Estrategia de pruebas

Todos los testers necesitan saber por dónde comenzar.

2 buenas preguntas:

1. ¿Qué problema tenemos actualmente?
2. ¿O qué problemas debemos evitar?

Escenarios y contextos de las pruebas:

- Seguridad
- Arquitectura
- Performance
- Usabilidad
- Escalabilidad

### Testing en desarrollo de software

No es lo mismo el testing que el checking

Testing: exploración de una idea. Aprender cómo sucede un flujo, cómo se generan datos, y que esto te genere nuevos resultados. Esto nunca termina.

Cheking: es cuando ya concoces algo y solamente verificas que siga ocurriendo. Es bueno para verificar.

Es importante no confundir estos 2 términos.

Las estrategias de cheking son:

- Solo se ejecutan si ... sucede algo más. *(ejemplo)*
- Se ejecutan cada que ... inserto nuevo código o datos. *(ejemplo)*
- Se ejecutan de manera programada.

#### Errores comunes durante la ejecución

- Pruebas duplicadas
- Pruebas similares
- Pruebas sin valor agregado
- Pruebas caducadas

Distinguir entre testing y cheking te lleva hacia la automatización.

La automatización de pruebas consiste en el uso de **software especial** para controlar la ejecución de pruebas y la comparación entre los resultados obtenidos y los resultados esperados. Sin embargo, se trata de un **cheking repetitivo y atuomatizado**.

#### Desventajas del cheking mal empleado

- Pobre cobertura de pruebas
- Falta de actualización
- Mal manejo de versiones

#### Ventajas de cheking bien empleado

- Correr pruebas en paralelo o en múltiples plataformas
- Reducción de error humano
- Probar gandes cantidades de datos

Por otro lado, cuando ya queremos hablar de  **Integración continua y Liberación Continua**, entonces la **automatización** es la solución definitiva para la eficiencia del equipo de desarrollo digital y equipos DevOps.

### Testing ágil

Testing ágil involucra a todos los miembros de un equipo ágil multifuncional, en el cual el rol del tester es el de un experto multifuncional, que garantiza se entregue valor de negocio deseado al cliente a un ritmo sostenible y continuo.

- El testing es de "todo el equipo"
- El Testing puede ser independiente (opcional)
- Integración continua
- Desarrollo guiado por pruebas (Test Driven Development - TDD)
- Desarrollo guiado por comportamiento (Behaviour Driven Development - BDD)
- Desarrollo guiado por pruebas de aceptación (Acceptance Test Driven Development - ATDD)

**Ejemplo de historias**:

Sesión de usuario: Nueva característica -> El usuaro puede **agregar** una foto a su perfil

- Sesión de usuario
  - Componentes
    - Hay foto
    - No hay foto
    - Actualizaciones
    - Eliminar
    - Editar
  - Integraciones
    - Repositorio
    - Accesos internos
    - Accesos externos
  - Aceptación de usuario
    - Formatos de imagen (jpe, jpeg, png)
    - Resolución y/o peso máximo

### Niveles de pruebas

- Pruebas de componentes -> Por ejemplo botontes o formularios
- Pruebas de integración -> Cómo se comunican los componentes en toda la app y cómo viajan los datos
- Prueba de sistema -> Hay que tomar en cuenta el contexto
- Prueba de aceptación -> Cuando le vamos a entregar el producto al cliente

### Tipos de pruebas

Independientemente de la profundidad de la prueba, aquí nos enfocaremos en las técnicas que vamos a emplear para tratar de encontrar los defectos.

1. Pruebas funcionales: Se entiende como las Funcionalidades del Sistema como "lo que el sistema hace".
2. Pruebas no funcionales: El objetivo de esta es probar "como funciona el sistema". -> UX y usabilidad, por ejemplo.
3. Pruebas estructurales: Para poder llevar a cabo estas pruebas, normalmente el tester debe tener conocimientos acerca de la tecnología y el stack que se está empleando.
4. Pruebas de manejo de cambios: Es probar nuevamente un componente ya probado para verificar que no ha sido impactado por actualizaciones.

### Pruebas estáticas y dinámicas

> **Las pruebas dinámicas** se enfocan principalmente en comportamientos externos visibles durante la ejecución del software.
> **Las pruebas estáticas** se basan en la examinación manual de los elementos que conforman la construcción del software.

Elementos:

- Contratos, planes y calendario del proyecto, así como su presupuesto.
- El análisis de requerimientos
- Especificaciones o reglas de negocio
  - Técnicos
  - Seguridad
- Las definiciones de:
  - Historias de usuario
  - Criterios de Aceptación
  - Mockups
- El diseño de la arquitectura
- Las pruebas (Testware), puntos de verificación CI
- Guías de usuario
- Evaluación/revisión del código

Beneficios:

- Detectar y corregir defectos de manera más eficiente
- Identificar y priorizar la ejecución de pruebas en etapas posteriores
- Prevenir defectos
  - Que no son fácilmente detectables durante las pruebas dinámicas
  - Durante la etapa de análisis y diseño
- Cubrir aspectos como:
  - Inconsistencias, ambigüedades, contradicciones, definiciones inexactas, requerimientos redundantes
- Reducir el retrabajo e incrementar la productividad
- Reducir el costo y el tiempo
- Mejorando la comunicación entre todos los miembros del equipo

### Definición y diseño de pruebas

¿Qué hace un tester?

1. Encontrar problemas
2. Documentar problemas
3. Comunicar problemas

Si no encuentras problemas antes de que el producto sea entregado el cliente, entonces su testing es ineficiente.

Si cuando encuentras problemas, no sabes documentar y reproducir los pasos correctos, el testing genera retrabajo y sube el costo.

Si como representate de la calidad del producto no sabes argumentar y proteger los intereses del negocio o los clientes, entonces el testing no agrega valor.

[Archivo de Google Sheets](https://docs.google.com/spreadsheets/d/1DScBhWbA8qfRsare8SSJ2AOGAj_zjuPJ-Pe4RyN2IQg/edit?usp=sharing)

## Gestión, monitoreo y control

### Caja Blanca, Gris y Negra

La caja se refiere al contenido del software.

- Negra -> No conocemos su código ni arquitectura ni cómo fue construido. Solamente la noción de la interfaz.
- Blanca -> Puedo ver todo lo que hay dentro, incluso puedo ser parte del equipo que desarrolló el software.
- Gris -> No conozco el código, pero veo cómo se transmiten los datos.

*Técnicas de pruebas*:

- Caja negra
  - Partición de equivalencia
  - Valores límite
  - Tabla de decisiones
  - Transición de estados
  - Casos de uso
- Caja gris
  - Casos de negocio
  - Pruebas End to End
  - Pruebas de integración
- Caja blanca
  - Cobertura de declaración
  - Cobertura de decisiones

Las prubeas "End to End" consisten en: Yo como usuario hago cosas y la información se verá reflejada no en mí, sino en otra parte de front end.

Las pruebas de integración son las respuestas y la comunicación de cómo fluyen los datos entre diferentes servicios.

### Gestión, monitoreo y control: Monitoreo y Seguimiento

La gestión de pruebas tiene varias etapas:

- Planeación de pruebas
  - > Definición de Objetivos de las pruebas, alcance de las mismas, las técnias de pruebas que se llevarán a cabo, junto con las estimación y definición de fechas de entrega, así como los criterios de salida.
- Monitoreo y control de pruebas
  - > Durante el Monitoreo se va midiendo y comparando los resultados de las métricas, y entonces durante el CONTROL se toman acciones para alcanzar el objetivo del plan y los criterios de salida
- Análisis de pruebas
  - > Cuando estamos analizando las pruebas para nuestro proyecto, necesitamos determinar qué debemos probar, obviamente basados en las prioridades de cobertura
- Diseño de pruebas
  - Diseño de casos de alto nivel
  - Diseñar y priorizar las pruebas
  - Identificar los datos de pruebas
  - Identificar el entorno de pruebas - infraestructura y herramientas
  - Hacer una trazabilidad entre pruebas y sus condiciones
- Implementación de pruebas
  - > Para poder prepararnos para hacer las pruebas, primero tenemos que asegurarnos que tenemos todo lo necesario para ello
- Ejecución de pruebas
- > Durante esta etapa, las suites de pruebas se ejecutan de acuerdo con el programa de ejecución de las pruebas
- Finalización de las pruebas
  - Defectos con el estatus correcto
  - Reporte para comunicar los resultados de las pruebas
  - Finalizar y archivar ambiente de pruebas y sus datos
  - Entregar el Testware al equipo de mantenimiento de pruebas
  - Analizar lecciones aprendidas para futuras versiones
  - Recopilar la información para ayudar a mejorar la madurez del proceso de prueba

### Roles y Responsibilidades

1. Especialista en pruebas manuales -> se enfoca en la estrategia, definición, ejecución y cobertura de pruebas para cumplir los requerimientos, echando mano de cualquier técnica para obtener información suficiente y así cumplir con las asignaciones correspondientes.
2. Especialista en pruebas técnicas -> trabaja muy de cerca con el tester manual, mientras que el tester manual define las pruebas, el tester técnico acelera la capacidad de ejecución de las pruebas. Esto lo hace implementando herramientas que permitan la automatización de pruebas, o la correcta selección de datos de pruebas, o el monitoreo de la ejecución de las pruebas.
3. Líder del equipo de pruebas -> generalmente dentro de sus responsabilidad es volverse un facilitador de servicios, información y herramientas para el equipo de pruebas, para poder estimar presupuestos, recursos y tiempos respecto al plan de desarrollo de software.
4. Ingeniero de calidad -> ya no solamente está al pendiente del producto y los procesos, comienza a involucrarse más con el negocio, ayudando tanto a testers como cualquier otro miembro del equipo a llevar cabo pruebas que reduzcan, en todas las etapas del ciclo de vida del software, el error humano.

### Roles y responsabilidades en acción

ndependientemente del rol, un tester participa de todas las etapas del proceso de desarrollo de software, colaborando para asegurar la máxima calidad del producto. Su perfil conjuga un conjunto de habilidades con el conocimiento del negocio, de la aplicación bajo prueba y de cómo planificar, diseñar, ejecutar y administrar las pruebas.

> Un tester investiga un producto de software con el objetivo de obtener información acerca de su calidad y del valor que representa para quienes lo utilizan.

*Habilidades de un tester*:

- Capacidad de abstracción y modelado para entender y simular el comportamiento del sistema bajo prueba.
- Comunicación para interactuar con todos los miembros del equipo.
- Pensamiento lateral para generar ideas e imaginar los problemas que podrían existir.
- Pensamiento crítico para observar y evaluar, hacer deducciones y vincular lo observado con los requerimientos de calidad de la empresa.
- Pragmatismo. Ser lo suficiente abierto para poner en práctica las ideas de los demás o propias, adecuar las técnicas y el esfuerzo al alcance del proyecto.
- Trabaja en equipo, sabe interactuar para lograr el mayor beneficio entre todos los involucrados.
