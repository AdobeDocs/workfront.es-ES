---
title: 'Guía: Escalado administrado, después de la primera victoria'
description: Obtenga información sobre cómo implementar Adobe Workfront Planning después de la primera implementación exitosa
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 28913661935d5a030cb33dd204fcb3c08daf0b26
workflow-type: tm+mt
source-wordcount: '2025'
ht-degree: 0%

---


# Guía de estrategias: escalado administrado, después de la primera victoria

**Versión**: 1.0

**Contexto**: &quot;Hemos llegado a nuestro primer caso de uso y ahora todos queremos entrar&quot;.



## &#x200B;1. La &quot;trampa del éxito&quot;

A veces puede parecer que la fase más peligrosa de la adopción del PMA es inmediatamente después del primer caso de uso exitoso o POC. El entusiasmo es alto, pero el miedo a la &quot;deuda técnica&quot; y a la &quot;expansión administrativa&quot; puede conducir a dos respuestas igualmente dañinas:

1. **Gobernanza excesiva**: Bloqueando el sistema tan fuertemente que los nuevos equipos vuelven a las hojas de cálculo.

2. **Gobernanza cero**: Permite que cada equipo cree sus propios campos y tipos de registros, recreando la expansión descontrolada de metadatos que se encuentra en entornos heredados.



## &#x200B;2. La filosofía básica: el PMA como &quot;motor de la reconciliación&quot;

En lugar de intentar evitar que los equipos sean diferentes, posicionamos WFP como el lugar donde esas diferencias se **hacen visibles para que se puedan reconciliar**.



* **Administración de la velocidad de adopción**: Es natural tener cuidado al expandir la aplicación a una nueva herramienta antes de &quot;limpiar&quot; los entornos existentes. Al elegir **Simplificar primero** proporciona una base altamente controlada, puede retrasar el tiempo de obtención del valor para los equipos listos para alinearse. Creemos que la manera más efectiva de llevar a cabo este cambio es reconocer que la visibilidad de **es el paso 1**. El impulso hacia una herramienta compartida y lista para la empresa (que se aleje de la expansión descontrolada de los PPT y las hojas de cálculo) es lo que en última instancia desbloquea los objetivos a largo plazo.



  **Recomendación**: En lugar de un mandato de &quot;Limpiar primero&quot;, recomendamos asignar una porción menor de recursos a mantenimiento continuo y una porción significativamente mayor a la solución de necesidades comerciales urgentes. Por ejemplo, dedicar un año exclusivamente a &quot;limpiar&quot; taxonomías no genera mucho valor incremental. Sin embargo, al ofrecer **visibilidad entre equipos** (por ejemplo, a través de un calendario empresarial unificado o una hoja de ruta de GTM consolidada), se obtiene el valor transformativo que necesitan las partes interesadas, al tiempo que se proporciona la estructura de datos unificada que necesita para gobernar el entorno a lo largo del tiempo.

* **Reconocer la realidad**: Los equipos independientes desarrollan naturalmente sus propios procesos, que a menudo permanecen ocultos en hojas de cálculo en silo. La transición al PMA no crea un lío; arroja luz sobre el que ya existe. Al hacer que estos procesos sean visibles en un entorno compartido, los pone en el único lugar donde finalmente se pueden abordar y mejorar.

* **La señal de progreso**: Cuando un equipo pide sus propios campos, no se &quot;expande&quot;, sino que es **Adopción**. Significa que ven al PMA como su espacio de trabajo.

* **Administrar deuda, no ocultarla**: Es natural preocuparse por el esfuerzo necesario para limpiar las taxonomías divergentes más adelante. Sin embargo, la alternativa (forzar estándares estrictos demasiado pronto) a menudo lleva a los equipos de vuelta a hojas de cálculo donde sus procesos (y su deuda) permanecen ocultos. Al permitir que los equipos comiencen en WFP con sus clasificaciones actuales, está trasladando esa deuda a un entorno visible y controlado. Esto hace que la reconciliación final sea una tarea iterativa en lugar de un único y abrumador proyecto de migración.



## &#x200B;3. El modelo de gobernanza de &quot;carriles en la carretera&quot;

Escalar sin deuda definiendo &quot;rutas globales&quot; y &quot;áreas de juego locales&quot;.



### A. Las vías mundiales

* **Objetos controlados**: objetos que todos los equipos deben usar para los informes de empresa (por ejemplo, `Strategic Pillar`, `Region`, `Fiscal Quarter`).

* **Administrado por**: El administrador central de código/operaciones de marketing.

* **Regla**: estos campos son &quot;Compartidos&quot; y obligatorios.



### B. Patios de recreo locales (radios)

* **Objetos experimentales**: campos o tipos de registros específicos de las necesidades tácticas de un equipo (por ejemplo, `Influencer Handle` de un equipo social o `URL Slug` de un equipo web).

* **Administrado por**: El jefe de equipo (con orientación básica).

* **Regla**: los equipos pueden innovar aquí. Si un campo &quot;Local&quot; es adoptado por más de 3 equipos, se &quot;Promociona&quot; a un carril global.



## &#x200B;4. La Paradoja De La Gobernanza: Los Equipos Primero, Las Normas Siguientes

Un desafío común en escalar WFP es decidir qué es lo primero: **Gobernanza empresarial** o **Alineación operativa del equipo**.



Creemos que la manera más efectiva de navegar por esto es reconocer que el valor empresarial se basa en una calle bidireccional:

1. **Los equipos necesitan relevancia**: la empresa solo obtiene valor cuando sus equipos se están ejecutando activamente. Por lo tanto, el gobierno debe **servir a los equipos** proporcionando una estructura que permita satisfacer sus necesidades operativas conocidas.

2. **La empresa necesita visibilidad**: el liderazgo solo puede tomar decisiones informadas cuando los datos están lo suficientemente limpios como para agregarse. Por lo tanto, los equipos deben **servir a la empresa** proporcionando los metadatos viables mínimos requeridos para la visibilidad del portafolio.



El objetivo de &quot;Escalado administrado&quot; es encontrar la intersección de estas dos necesidades: estandarizar lo suficiente como para proporcionar visibilidad, pero no tanto como para demorar la ejecución del equipo.



### A. Alinear prioridades: datos frente a visualización

Al escalar, reconozca que la definición de &quot;Valor&quot; difiere entre las personas:

* **Administrador/Propietario del producto**: Valores **taxonomías y clasificaciones unificadas**. Su objetivo es una arquitectura de datos limpia que admita la escalabilidad a largo plazo.

* **La parte interesada/líder**: Valores **visualización y insight** (por ejemplo, un calendario global o una cronología de Portfolio). Su objetivo es el &quot;Momento del rayo&quot; que hace que los datos sean procesables.



**La estrategia**: usa la necesidad de visualización de la parte interesada como el *incentivo* para que el equipo cumpla con la necesidad del administrador de estándares de datos. Se obtiene la taxonomía unificada al entregar el &quot;Super Calendario&quot; que exige el liderazgo.



### B. La fase de observación &quot;basada en los servicios&quot;

Durante la ampliación temprana, la función del administrador es facilitar este intercambio entre los equipos y la empresa.

* **Priorizar la operación sobre la estandarización**: es mejor que los equipos planifiquen activamente en espacios de trabajo en silo que que que se detengan debido a la falta de definiciones globales. Esta actividad es el &quot;dato sin procesar&quot; necesario para crear estándares sanos en el mundo real.

* **Identificar los &quot;mínimos de visibilidad&quot;**: trabaje con el liderazgo para identificar los 3-5 campos que *deben* estar limpios para los informes de empresa (por ejemplo, `Strategic Alignment`, `Start Date`, `Budget`). Concéntrese en su energía de aplicación SOLAMENTE aquí.



### B. Armonización retroactiva (gobernanza como servicio)

Una vez que surge un patrón de &quot;necesidades conocidas&quot; entre los equipos, la empresa puede pasar a consolidar esos patrones en un servicio global.

1. **Observar patrones exitosos**: identifique las taxonomías &quot;ganadoras&quot; que los equipos ya han creado y adoptado.

2. **El protocolo de enlace colaborativo**: reúna a los campeones del equipo para refinar sus éxitos locales y convertirlos en un estándar empresarial compartido.

3. **Implementar as a Service**: Despliegue las nuevas rutas globales no como una &quot;restricción&quot;, sino como una forma de simplificar la creación de informes y la alineación entre equipos para las personas que realizan el trabajo.



**Comida para llevar clave**: la gobernanza debe ser una respuesta al éxito operativo, no un requisito previo para él.



## &#x200B;5. Mecánica de la escala: el modelo de crecimiento basado en patrones

La aplicación de esta filosofía requiere un enfoque reflexivo de la estructura de datos. Para evitar la &quot;expansión descontrolada de la gobernanza&quot;, resista el impulso de crear campos globales para cada solicitud individual. En su lugar, use la **Ruta de madurez del campo** para permitir que el uso real guíe los estándares de su empresa:



1. **Nivel 1: Experimento local**: El equipo A crea un campo personalizado en su área de trabajo.

2. **Nivel 2: Reconocimiento de patrones**: El administrador observa que los equipos B y C están usando o solicitando un campo similar.

3. **Nivel 3: Estandarización empresarial**: El administrador crea una sola versión estandarizada de ese campo como tipo de registro en la **Taxonomía global Workspace** y la asocia a los equipos.



### La mecánica de la &quot;jubilación suave&quot;

Debido a que WFP no tiene actualmente una función nativa de &quot;Archivo&quot; para los campos, la retirada de un campo local requiere un proceso deliberado de &quot;Baja en software&quot; para conservar los datos históricos sin saturar la interfaz de usuario:



1. **Migración de datos**: use una vista de tabla (o Fusion) para copiar de forma masiva valores del campo local &quot;Sombra&quot; en el nuevo campo de carril global. Asegúrese de que los datos se validen y limpien durante este movimiento.

2. **Cambiar nombre para obsoleto**: cambie el nombre del campo local con un prefijo como `[DEPRECATED]` o `z_` (por ejemplo, `z_Language (Old)`). Esto lleva el campo al final de los selectores de campos e indica a los usuarios que ya no es el &quot;Source de la verdad&quot;.

3. **Eliminación de formulario**: **Este es el paso más crítico.** Quite el campo obsoleto de todos los **Registros de Forms**. Esto evita que se introduzcan nuevos datos y mantiene los datos antiguos visibles en las vistas de tabla o informes existentes si es necesario.

4. **Período de &quot;ocaso&quot;**: mantenga el campo obsoleto (con prefijo y sin formato) durante 30-60 días para asegurarse de que no se pierdan datos durante la migración. Después de este periodo, si los datos se reconcilian completamente en la ruta global, el campo local se puede eliminar del espacio de trabajo.



## &#x200B;6. Evitar la &quot;deriva básica&quot; (la regla de abstracción)

Para evitar que Planning se llene de elementos tan confusos como el Principal:

* **Capa de abstracción**: cada campo de WFP debe responder a una **pregunta estratégica**. Si un campo solo se utiliza para el seguimiento táctico (por ejemplo, &quot;¿se aprobó esta prueba?&quot;), manténgalo en Principal.

* **Primero consolidación**: Si un equipo desea un nuevo campo de metadatos, invítelo a comprobar primero la taxonomía global. Esto requiere que se conceda a los posibles clientes **acceso de solo lectura** al área de trabajo de taxonomía global (consulte la sección 7). Al asignar sus necesidades tácticas a un campo estratégico existente, evita la duplicación innecesaria y mantiene la integridad de la creación de informes.



## &#x200B;7. Modelo de visibilidad de &quot;acceso de solo lectura&quot;

Resuelve la sensación &quot;Siloed&quot; sin el ruido del trabajo &quot;Siloed&quot;.

* **El problema**: Los equipos de los radios se sienten aislados porque solo ven sus propios registros.

* **Corrección**: Conceda a los equipos **acceso de solo lectura a los espacios de trabajo designados como &#39;Principales&#39; para esos tipos de registros compartidos**.

* **El resultado**: pueden ver el contexto empresarial más amplio para inspirarse y alinearse, pero su espacio de trabajo local permanece limpio y centrado en sus tareas específicas.



## &#x200B;8. Gestión del crecimiento mediante talleres

La ampliación del PMA es tanto un desafío cultural como un desafío técnico. Utilice talleres específicos para salvar la &quot;brecha de gobernanza&quot;.



### A. El taller de descubrimiento &quot;Desastre necesario&quot;

* **Audiencia**: líderes de marketing regional y campeones de operaciones.

* **Objetivo**: Documentar la &quot;realidad aislada&quot; actual (los datos operativos fragmentados).

* **El mensaje**: &quot;No estamos aquí para eliminar sus campos. Estamos aquí para entender cómo se vinculan a la estrategia global&quot;.

* **Resultado**: un borrador de asignación de campos tácticos locales a rutas estratégicas globales.



### B. Sesión de alineación sobre &quot;Visibilidad estratégica&quot;

* **Audiencia**: partes interesadas de alto nivel en marketing (liderazgo).

* **Objetivo**: replantea la ansiedad de &quot;Simplificar primero&quot;.

* **El mensaje**: &quot;No necesitamos una taxonomía perfecta para comenzar. Estamos usando WFP como entorno para *crear* la taxonomía perfecta&quot;.

* **Resultado**: la aprobación para avanzar con WFP como motor de reconciliación mientras Core permanece en su estado actual.



### C. El escaparate &quot;Spoke-to-Global&quot;

* **Audiencia**: nuevos equipos explorando WFP.

* **Objetivo**: Reduzca la sensación de &quot;en silo&quot;.

* **El mensaje**: &quot;¿Ve cómo el trabajo local del equipo A alimenta automáticamente al Workspace principal designado? También puede tener la misma visibilidad para su trabajo&quot;.

* **Resultado**: Inclusión de nuevos departamentos que ven el beneficio de estar &quot;conectados&quot; sin perder su independencia local.



### D. Horario de oficina de &quot;asistencia continua&quot;

* **Audiencia**: Todos los usuarios de WFP (actuales y potenciales).

* **Objetivo**: proporcione un entorno recurrente de bajo riesgo para la resolución de problemas y la orientación táctica.

* **El mensaje**: &quot;No hay preguntas erróneas. Estamos aquí para ayudarle a resolver sus desafíos de planificación específicos en tiempo real&quot;.

* **Resultado**: mayor confianza del usuario, resolución más rápida de la fricción técnica e identificación de nuevos patrones que podrían justificar la estandarización global.



## &#x200B;9. Plantilla para escalas: funciones y responsabilidades

El éxito en un modelo de escalado administrado requiere algo más que una simple configuración de la herramienta; requiere una clara distribución de funciones entre los equipos Global y Spoke.



### A. Arquitecto empresarial (CdE central/operaciones de marketing)

* **Enfoque**: Integridad empresarial, rendimiento del sistema y **taxonomía de datos unificados**.

* **Funciones**:

   * Administra la **Taxonomía global Workspace**.

   * Facilita la **ruta de madurez del campo** (promoviendo los éxitos locales a los estándares globales).

   * Mantiene las vistas **Workspace principal** para los informes ejecutivos.

   * Encabeza la **auditoría semántica** mensual en todos los espacios de trabajo.



### B. El Campeón de Radios (Propietario del Proceso de Equipo)

* **Enfoque**: relevancia del equipo y velocidad de adopción.

* **Funciones**:

   * Actúa como único punto de contacto para el equipo funcional.

   * Es propietario de la estructura del espacio de trabajo local y de los experimentos de campo personalizados.

   * Garantiza que el equipo use **la puerta de enlace controlada** (Forms) para la entrada de datos.

   * Participa en **protocolo de enlace colaborativo** durante la armonización.



### C. Patrocinador ejecutivo (liderazgo en marketing)

* **Enfoque**: alineación estratégica, visibilidad de OKR y **visualización de portafolio (por ejemplo, Calendario global)**.

* **Funciones**:

   * Define las **OKR de marketing** de la empresa en el área de trabajo de taxonomía global.

   * Campeona el valor de &quot;Etapa de visibilidad 1&quot; para otros líderes.

   * Refuerza la asignación de recursos al 80/20 (valor sobre limpieza).



### D. El responsable de la habilitación (administración de cambios)

* **Enfoque**: Cambio cultural y desarrollo de habilidades.

* **Funciones**:

   * Aloja **Horario de oficina** y **Talleres de descubrimiento** que se repiten.

   * Mantiene la vitrina interna &quot;Historia de éxito&quot;.

   * Identifica los puntos de fricción técnica que debe resolver Enterprise Architect.



## &#x200B;10. Lista de comprobación para escalar el siguiente equipo

* [ ] **Identificar al Campeón**: ¿Quién es el &quot;Propietario del proceso&quot; o el &quot;Campeón&quot; de este nuevo equipo?

* [ ] **Defina el &quot;Delta local&quot;**: ¿Qué campos 2-3 necesita este equipo que el Estándar global no proporciona actualmente?

* [ ] **Asignar a rutas globales**: ¿Qué campos globales existentes pueden satisfacer el 80% de sus necesidades?

* [ ] **Conceder visibilidad global**: Proporcióneles acceso de solo lectura a los espacios de trabajo primarios y al espacio de trabajo de taxonomía global relevantes el día 1.

* [ ] **Establecer transferencia**: ¿Cómo &quot;alimenta&quot; su trabajo los espacios de trabajo primarios relevantes? (por ejemplo, a través de un tipo de registro global o una búsqueda específica).