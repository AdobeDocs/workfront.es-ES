---
title: 'Modelo de éxito: modelado de la jerarquía de campañas'
description: Aprenda a traducir sus procesos empresariales complejos en una jerarquía de campañas escalable y controlada mediante "Centros de gravedad" y una arquitectura de espacio de trabajo múltiple.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: 77ef50ebd583f0a46324e5cbdc4feea9d21f4280
workflow-type: tm+mt
source-wordcount: '1056'
ht-degree: 0%

---


# Modelo de éxito: modelado de la jerarquía de campañas



## Meta

Aprenda a traducir sus procesos empresariales complejos en una jerarquía de campañas escalable y controlada mediante &quot;Centros de gravedad&quot; y una arquitectura de espacio de trabajo múltiple.



## Información general

A medida que sus operaciones de marketing se escalan, también lo hace la complejidad de sus datos. Sin un modelo claro, el sistema de registro de marketing (MSOR) puede convertirse rápidamente en un &quot;cajón de la basura&quot; de registros desconectados, terminología en conflicto y silos de informes.



El &quot;Modelo de éxito&quot; es un marco para modelar la jerarquía de campañas en Workfront Planning (WFP). Le permite pasar del &quot;caos de la hoja de cálculo&quot; a un modelo controlado y orientado a objetos que garantiza que todos los equipos hablen el mismo idioma y, al mismo tiempo, mantiene la agilidad que necesitan para ejecutarse.



## La jerarquía: encontrar sus niveles de intención

Para mantener la claridad y la escalabilidad, se recomienda comenzar con una **ruta principal** de eficacia probada. Si bien las organizaciones pueden ampliar esta jerarquía a medida que evolucionan sus necesidades operativas, el inicio de estos tres niveles garantiza un puente sólido entre la estrategia y la ejecución.



### La ruta principal: estrategia para la acción

La mayoría de las implementaciones exitosas prosperan en un modelo limpio de tres niveles que abarca tanto la planificación como el flujo de trabajo:



1. **Nivel 1: Campañas (Módulo de planificación)**

   * **Enfoque:** Pilares estratégicos a largo plazo e iniciativas anuales (por ejemplo, &quot;Conocimiento global de la marca del año fiscal 2026&quot;).

   * **Persona:** CMO, vicepresidenta de marketing, posibles clientes estratégicos.

2. **Nivel 2: tácticas de canal (módulo de planificación)**

   * **Enfoque:** Los informes operativos que definen el &quot;qué&quot; para canales específicos (por ejemplo, &quot;Blitz de medios sociales del primer trimestre&quot;). Esta es la última capa de la intención estratégica antes de que comience el trabajo.

   * **Persona:** Operaciones De Marketing, Posibles Clientes Del Canal Y Administradores De Campañas.

3. **Nivel 3: Proyectos De Flujo De Trabajo (Módulo De Flujo De Trabajo)**

   * **Enfoque:** La ejecución real de &quot;Experiencias&quot; o &quot;Actividades&quot; (por ejemplo, publicaciones sociales específicas, correos electrónicos o páginas web).

   * **Implementación:** Las tácticas en Planning se vinculan directamente a **Proyectos** en el módulo Flujo de trabajo, donde los entregables individuales se administran como tareas y problemas.

   * **Persona:** creativos, colaboradores individuales.



### Expansión estratégica: añadir más niveles

Una vez establecida la ruta principal, las organizaciones pueden elegir añadir capas adicionales después de considerar cuidadosamente su complejidad empresarial específica:



* **Planes de canal:** Una capa entre *Campañas* y *Tácticas* para agrupar estrategias interfuncionales (por ejemplo, &quot;Estrategia digital&quot;).

* **Actividades del PMA:** En entornos de menor volumen (por lo general, &lt;5.000 entregables/año), algunos equipos prefieren realizar un seguimiento de las &quot;experiencias&quot; individuales como registros del PMA antes de que se conviertan en proyectos.


>[!TIP]
>
>**Sugerencia crucial: El umbral de 5000 entregas**
>
>Si su organización produce más de 5000 actividades al año, debería **descargar siempre** el seguimiento de entregables individuales al **módulo de flujo de trabajo**. La administración de registros de &quot;experiencia&quot; de gran volumen en Planning puede llevar a la acumulación de datos que oscurece la visibilidad estratégica. Utilice Planning para los módulos &quot;Por qué&quot; y &quot;Qué&quot; y Flujo de trabajo para el módulo de gran volumen &quot;Cómo&quot;.



## Arquitectura: Centros de Gravedad

Un MSOR de nivel empresarial no está integrado en un solo espacio de trabajo. Utiliza una arquitectura de &quot;concentrador y radio&quot; donde los tipos de registros se administran en sus **centros de gravedad** naturales.



### &#x200B;1. Centro de taxonomía (clasificaciones)

Establezca un espacio de trabajo centralizado para sus &quot;clasificaciones globales&quot; (por ejemplo, marcas, regiones, productos, personas).

* **Ubicación principal:** Este espacio de trabajo es el &quot;Source de la verdad&quot; para estos objetos.

* **Ventaja:** Al distribuir estas definiciones al resto de la empresa, se resuelve &quot;Desviación semántica&quot;, lo que garantiza que &quot;Región: EMEA&quot; signifique lo mismo para todos los equipos.



### &#x200B;2. El Workspace de Planificación Estratégica (Centro Ejecutivo)

Aquí es donde se activan las **Campañas** de alto nivel (y cualquier **plan de canal**).

* **Ubicación principal:** Este es el centro de gravedad ejecutivo, que proporciona un entorno sin ruido para la toma de decisiones estratégicas.

* **Ventaja:** El liderazgo puede administrar el portafolio sin ver el lío táctico cotidiano.



### &#x200B;3. Radios funcionales (espacios de trabajo de equipo)

Las unidades funcionales (Social, Creative, Correo electrónico) tienen sus propios espacios de trabajo para administrar sus **tácticas**.

* **Ubicación principal:** Estos espacios de trabajo son el centro de gravedad para la ejecución del equipo local.

* **El beneficio:** equipos &quot;consumen&quot; las campañas globales y las clasificaciones de los concentradores, al tiempo que mantienen sus propios objetos locales (como *Medios de comunicación* o *Derechos de uso*).



## Gobernanza basada en nombres: hablar un idioma

Para asegurarte de que tu modelo se mantenga bajo presión, sigue el principio de **Gobernanza basada en nombres**.



* **Usar sustantivos, no verbos:** Asigne un nombre a los tipos de registro después de las &quot;cosas&quot; que está rastreando (`Campaign`, `Tactic`), no a las &quot;acciones&quot; (`Campaigning`, `Planning`).

* **Estandarizar nomenclatura:** Use los mismos nombres en todos los espacios de trabajo. Esto le permite agregar datos en todo el portafolio para la creación de informes ejecutivos.



## ¿Qué sucede con los portafolios y programas existentes?

Una pregunta común para las organizaciones maduras es cómo administrar los portafolios y programas que ya han creado en el **módulo de flujo de trabajo**. En el pasado, estos objetos se utilizaban a menudo para imitar la planificación estratégica.



### &#x200B;1. Portafolios y programas → tipos de registros

En muchas organizaciones, **Portafolios** se usan para representar marcas de alto nivel o unidades de negocio (UB), mientras que **Programas** representan temas estratégicos.

* **El cambio:** Estos se modelan mejor como **Tipos de registro** en su **centro de taxonomía**. Al considerar &quot;Marca&quot; o &quot;Unidad de negocio&quot; como un tipo de registro, puede vincularlos a cualquier campaña o táctica en toda la empresa, lo que proporciona una creación de informes mucho más flexible que una estructura estática de Portfolio/Programa.



### &#x200B;2. Estrategia de &quot;Reporting Bridge&quot;

Aunque Workfront Planning es el futuro de la intención estratégica, sus informes nativos a través de **paneles de lienzo** todavía están madurando. Muchas organizaciones aún dependen de las sólidas capacidades de creación de informes vinculadas a sus estructuras heredadas de Portfolio y Programa en el módulo Flujo de trabajo.

* **La recomendación:** Aún no elimine sus portafolios y programas. En su lugar, use **automatizaciones de Fusion** para crear un puente.

* **Cómo funciona:** Cuando se crea una táctica o campaña en WFP, Fusion puede reflejar automáticamente ese registro en un Portfolio o programa correspondiente en el módulo Flujo de trabajo. Esto le permite:

   1. Disfrute de la excelente **visualización estratégica** del PMA (cronogramas/calendarios).

   2. Mantenga sus **informes heredados** en el módulo de flujo de trabajo para las partes interesadas que aún no estén listas para pasar al lienzo.

## Prácticas recomendadas y consejos

### Haga:

* **Primero manténgase en la ruta principal.** Establezca su flujo de campaña táctica a proyecto antes de agregar más complejidad.

* **Designar espacios de trabajo principales.** Asegúrese de que cada tipo de registro tenga un espacio de trabajo &quot;principal&quot; (su centro de gravedad) que actúe como agregador para los informes.

* **Dar prioridad a Forms para la admisión.** Use formularios de registro para grupos con menos sofisticación en WFP para garantizar la integridad de los metadatos. Aunque los usuarios avanzados pueden beneficiarse de la entrada directa de datos en las vistas de tabla, esto debe abordarse con precaución: los cambios masivos en una tabla pueden crear fácilmente problemas de datos para otras partes interesadas.


### No haga lo siguiente:

* **No digas &quot;Core&quot;.** Consulte específicamente el **módulo de flujo de trabajo** y los objetos **Proyecto** cuando hable sobre la ejecución.

* **No se complique en exceso.** Cada nivel adicional de jerarquía agrega un &quot;impuesto de administración&quot;. Agregue únicamente niveles que respondan a una pregunta comercial que no pueda responder en este momento.

* **No cree silos.** Asegúrese de que los tipos de registros se compartan entre espacios de trabajo para que los equipos no vuelvan a escribir los mismos datos.




