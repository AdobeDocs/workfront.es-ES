---
title: 'Arquitectura de su éxito: modelado de la jerarquía de campañas'
description: Aprenda a traducir sus procesos empresariales complejos en una jerarquía de campañas escalable y controlada mediante "Centros de gravedad" y una arquitectura de espacio de trabajo múltiple.
feature: Workfront Planning
role: Admin
author: Alina
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
exl-id: 02e3b55f-9188-42bf-8d0b-c9fed86c63c4
source-git-commit: 52bf41e146a11a4af4fbebfe5bb20a9765f2bc7b
workflow-type: tm+mt
source-wordcount: '1471'
ht-degree: 1%

---

# Arquitectura de su éxito: modelado de la jerarquía de campañas

<!--see the file again for additional comments from Seth and others-->

{{planning-important-intro}}

Aprenda a traducir sus procesos empresariales complejos en una jerarquía de campañas escalable y controlada mediante centros de gravedad y una arquitectura de varios espacios de trabajo en Adobe Workfront Planning.

Esta guía está destinada a administradores de Workfront y usuarios avanzados que implementan y diseñan la arquitectura de su entorno en Workfront Planning.

## Descripción general de la arquitectura de éxito

A medida que sus operaciones de marketing maduran, también lo hace la complejidad de sus datos. Sin un modelo claro, el sistema de registro de marketing puede convertirse rápidamente en un cajón de basura de registros desconectados, terminología en conflicto y silos de informes.

Cuando crea una arquitectura de éxito, establece un marco para modelar la jerarquía de campañas en Workfront Planning. Pasa del caos de las hojas de cálculo a un modelo controlado y orientado a objetos que garantiza que todos los equipos hablen el mismo idioma y, al mismo tiempo, mantiene la agilidad que necesitan para ejecutarse.

## Cree una jerarquía para definir los niveles de intención

Para mantener la claridad y la escalabilidad, se recomienda comenzar con una ruta principal comprobada al diseñar el flujo de trabajo en Workfront Planning.

A partir de ahí, puede ampliar su estrategia añadiendo más niveles a su arquitectura.

### La ruta principal: cómo pasar de la estrategia a la acción

Si bien las organizaciones pueden ampliar esta jerarquía a medida que evolucionan sus necesidades operacionales, al comenzar con los tres niveles descritos en las secciones siguientes se asegura un fuerte puente entre la estrategia y la ejecución.

A partir de nuestros hallazgos, hemos observado que la mayoría de las implementaciones exitosas de Workfront Planning prosperan en un modelo limpio de tres niveles que abarca tanto Planning como Workfront.

A continuación se indican los niveles de una implementación correcta de Planning y los artefactos que podría considerar crear para ayudarle en el proceso:

* **Nivel 1: Campañas (Workfront Planning)**

   * **Enfoque:** Defina los pilares estratégicos a largo plazo y las iniciativas anuales. Por ejemplo, defina una iniciativa para su organización llamada &quot;Conocimiento global de la marca del año fiscal 2026&quot;. Este es su enfoque para un lapso de tiempo determinado. Cree campañas para apoyar esta iniciativa.

   * **Personas:** Las partes interesadas de este nivel pueden ser un Oficial de marketing, un Vicepresidente de marketing u otros posibles clientes estratégicos.

  Para obtener más información, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

* **Nivel 2: tácticas de canal (planificación de Workfront)**

   * **Enfoque:** Defina los informes operativos que describen el &quot;qué&quot; para canales específicos. Esta es la última capa de la intención estratégica antes de que comience el trabajo. Por ejemplo, cree una táctica de &quot;bombardeo de medios sociales en el primer trimestre&quot;. A continuación, puede emparejarlo con sus campañas.

   * **Personas:** Las partes interesadas principales son un líder de operaciones de marketing, líderes de canal o administradores de campaña.

* **Nivel 3: Proyectos (Planning y Workfront)**

   * **Enfoque:** Ejecute en las experiencias o actividades exactas que eventualmente logren su iniciativa. Algunos de los entregables son específicos, como publicaciones sociales, correos electrónicos o páginas web.

   * **Implementación:** Puede crear Tácticas en Planning y vincularlas directamente a **Proyectos** en Workfront, donde las entregas individuales se administran como tareas y problemas.

   * **Persona:** Las principales partes interesadas aquí son creativos, colaboradores individuales, cualquier persona responsable de hacer el trabajo para apoyar la iniciativa.

### Expansión estratégica: cómo añadir más niveles

Una vez establecida la ruta principal, puede elegir añadir capas adicionales después de considerar cuidadosamente su complejidad empresarial específica.

Puede resultar útil crear los siguientes elementos adicionales:

* **Planes de canal:** Una capa entre campañas y tácticas para agrupar estrategias interfuncionales. Por ejemplo, un plan llamado &quot;Estrategia digital&quot;.

* **Actividades:** Si trabaja en un entorno de menor volumen (podría tener 5000 o menos entregas al año), es posible que algunos equipos prefieran realizar el seguimiento de experiencias individuales como registros de Workfront Planning antes de que se conviertan en proyectos de Workfront.

>[!IMPORTANT]
>
>Si su organización produce más de 5000 actividades al año, debe transferir el seguimiento de entregables individuales a Workfront.
>
>La administración de registros de experiencia de gran volumen en Planning puede llevar a la acumulación de datos que oscurece la visibilidad estratégica.
>Recomendamos esta guía general para lograr la máxima eficiencia:
>
>* Utilizar la planificación para el &quot;por qué&quot; y el &quot;qué&quot;
>* Utilice Workfront para el &quot;cómo&quot; de gran volumen.

## Comprender los centros de gravedad para construir su arquitectura

Un sistema de registro de marketing de nivel empresarial no se crea en un solo espacio de trabajo. Utiliza una arquitectura &quot;radial&quot; en la que los tipos de registros se administran en sus centros de gravedad naturales.

Para obtener más información, consulte [Despliegue su hogar estratégico: un Launchpad de 30 días](/help/quicksilver/planning/best-practices.md/30-day-launchpad.md).

Para crear la arquitectura con el enfoque radial, debe crear lo siguiente:

* Un centro de taxonomía
* Un espacio de trabajo de planificación estratégica
* Radios funcionales

### Cree el centro de taxonomía como sus clasificaciones

Primero debe establecer un espacio de trabajo centralizado para las clasificaciones globales a fin de definir los conceptos principales que todos los miembros de su organización deben comprender. Por ejemplo, cree los siguientes tipos de registros en un espacio de trabajo central: Marcas, Regiones, Productos, Personas.

Para obtener más información, consulte [Crear tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md).

Establezca lo siguiente al crear sus clasificaciones:

* **Ubicación principal:** Elija un área de trabajo principal. Este espacio de trabajo debe ser la fuente fiable para los tipos de registros que cree.

* **Ventaja:** Al distribuir estas definiciones al resto de la empresa, se soluciona aclarar que conceptos como &quot;Región: EMEA&quot; significan lo mismo para todos los equipos.

### Cree el espacio de trabajo de Planning estratégico como centro ejecutivo

El centro ejecutivo es donde se ejecutan las campañas de alto nivel (y cualquier plan de canal).

* **Ubicación principal:** Este es el centro de gravedad ejecutivo, que proporciona un entorno sin ruido para la toma de decisiones estratégicas.

* **Ventaja:** El liderazgo puede administrar el portafolio de campañas sin escuchar el ruido táctico diario.

### Defina los radios funcionales como espacios de trabajo de sus equipos

Las unidades funcionales (Social, Creative, Correo electrónico) tienen sus propios espacios de trabajo para administrar sus tácticas.

* **Ubicación principal:** Estos espacios de trabajo son los centros de gravedad individuales para la ejecución del equipo local.

* **Ventaja:** Los equipos consumen las campañas globales y las clasificaciones de los concentradores, a la vez que mantienen sus propios objetos locales.

  Por ejemplo, el equipo puede agregar el tipo de registro de campaña del espacio de trabajo central al espacio de trabajo de su equipo, pero crear campañas relevantes solo para su espacio de trabajo. Algunos ejemplos de campañas son &quot;Medios de comunicación&quot; o &quot;Derechos de uso&quot;.

## Utilizar un enfoque de gobernanza basado en sustantivos

Para garantizar que su arquitectura se mantenga bajo presión, siga el principio de gobernanza basada en sustantivos.

Le recomendamos lo siguiente al crear sus entidades en Workfront Planning:

* **Use sustantivos, no verbos:** Asigne un nombre a los tipos de registro después de las cosas que está rastreando (asígneles el nombre &quot;Campaña&quot; o &quot;Táctica&quot;), no a las acciones que se van a realizar (no asígneles el nombre &quot;Campaña&quot; o &quot;Planificación&quot;).

* **Normalizar nomenclatura:** Utilice los mismos nombres en todos los espacios de trabajo. Esto le permite agregar datos en todo el portafolio para la creación de informes ejecutivos.

## ¿Qué sucede con los portafolios y programas existentes?

Una pregunta común para las organizaciones maduras es cómo gestionar los portafolios y programas que ya han creado en Workfront. En el pasado, estos objetos se utilizaban a menudo para imitar la planificación estratégica.

Ahora, le recomendamos que cambie ese enfoque a Workfront Planning, que naturalmente se ajusta al enfoque estratégico de la planificación.

### Reemplazar portafolios y programas por tipos de registro

En muchas organizaciones, los portafolios se utilizan para representar marcas de alto nivel o unidades de negocio, mientras que los programas representan temas estratégicos.

En Workfront Planning, se pueden modelar mejor como tipos de registro en su centro de taxonomía.

Al tratar una marca o una unidad empresarial como un tipo de registro, puede vincularlas a una campaña o táctica en toda la empresa, lo que proporciona una creación de informes mucho más flexible que una estructura estática de Portfolio - Programa.

### Uso de una estrategia de puente de creación de informes

Aunque Workfront Planning es el futuro de la intención estratégica, sus informes nativos a través del panel de lienzo aún están madurando.

Muchas organizaciones aún dependen de las sólidas capacidades de creación de informes vinculadas a sus estructuras heredadas de Portfolio y programas en Workfront.

Recomendamos lo siguiente:

* No elimine sus portafolios y programas.
* Utilice las automatizaciones de Planning para crear un puente entre los tipos de registros y los portafolios y programas.

  Cuando se crea una táctica o una campaña en Workfront Planning, ese registro puede generar un Portfolio o programa correspondiente en Workfront.

  Para obtener más información, vea [Crear objetos mediante automatizaciones de registros de Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

Esto le permite:

* Disfrute de la visualización estratégica superior de Workfront Planning mediante el uso de cronologías y calendarios.

* Mantenga sus informes heredados en Workfront para las partes interesadas que aún no estén listas para pasar al lienzo.

## Prácticas recomendadas y sugerencias

### Dos

* **Siga el enfoque de la ruta principal:** Establezca su flujo de campaña a táctica a proyecto antes de agregar más complejidad.

* **Designar espacios de trabajo principales:** Asegúrese de que cada tipo de registro tenga un espacio de trabajo principal (tenga en cuenta que es su centro de gravedad) que actúa como agregador para los informes.

* **Priorice los formularios de solicitud para el proceso de admisión:** Use formularios de registro para grupos con menos sofisticación en Workfront Planning para garantizar la integridad de los metadatos.

  >[!CAUTION]
  >
  >Aunque los usuarios avanzados pueden beneficiarse de la entrada directa de datos en las vistas de tabla, esto debe abordarse con precaución.
  >Los cambios masivos en una tabla pueden crear fácilmente dolores de cabeza de datos para otras partes interesadas.

### No lo hagas

* **No use generalizaciones:** Por ejemplo, en lugar de hablar de un entorno &quot;principal&quot;, consulte específicamente Workfront y el objeto Proyecto cuando hable de la ejecución.

* **No complicar en exceso:** Cada nivel adicional de jerarquía agrega un impuesto de administración. Agregue únicamente niveles que respondan a una pregunta comercial que no pueda responder en este momento.

* **No crear silos:** Asegúrese de que los tipos de registros se compartan entre espacios de trabajo para que los equipos no vuelvan a escribir los mismos datos.


<!--original content:


## Goal 

Learn how to translate your complex business processes into a scalable, governed campaign hierarchy using "Centers of Gravity" and a multi-workspace architecture. 

 

## Overview 

As your marketing operations scale, so does the complexity of your data. Without a clear blueprint, your Marketing System of Record (MSOR) can quickly become a "junk drawer" of disconnected records, conflicting terminology, and reporting silos. 

 

The "Blueprint of Success" is a framework for modeling your campaign hierarchy in Workfront Planning. It moves you from "spreadsheet chaos" to a governed, object-oriented model that ensures every team speaks the same language while maintaining the agility they need to execute. 

 

## The Hierarchy: Finding Your Levels of Intent 

To maintain clarity and scalability, we recommend starting with a proven **Core Path**. While organizations can expand this hierarchy as their operational needs evolve, beginning with these three levels ensures a strong bridge between strategy and execution. 

 

### The Core Path: Strategy to Action 

Most successful implementations thrive on a clean, three-tier model that spans both Planning and Workflow: 

 

1. **Level 1: Campaigns (Planning Module)** 

    * **Focus:** Long-term strategic pillars and annual initiatives (e.g., "FY26 Global Brand Awareness").  

    * **Persona:** CMO, VP of Marketing, Strategic Leads. 

2. **Level 2: Channel Tactics (Planning Module)** 

    * **Focus:** The operational briefs defining the "what" for specific channels (e.g., "Q1 Social Media Blitz"). This is the final layer of strategic intent before work begins. 

    * **Persona:** Marketing Ops, Channel Leads, Campaign Managers. 

3. **Level 3: Workflow Projects (Workflow Module)** 

    * **Focus:** The actual execution of "Experiences" or "Activities" (e.g., specific social posts, emails, web pages).  

    * **Implementation:** Tactics in Planning link directly to **Projects** in the Workflow module, where individual deliverables are managed as tasks and issues. 

    * **Persona:** Creatives, Individual Contributors. 

 

### Strategic Expansion: Adding More Levels 

Once the core path is established, organizations may choose to add additional layers after careful consideration of their specific business complexity: 

 

* **Channel Plans:** A layer between *Campaigns* and *Tactics* to group cross-functional strategies (e.g., "Digital Strategy"). 

* **Workfront Planning Activities:** In lower-volume environments (typically <5,000 deliverables/year), some teams prefer to track individual "Experiences" as Workfront Planning records before they become projects. 


>[!TIP]
>
>**Crucial Tip: The 5,000 Deliverable Threshold** 
>
>If your organization produces more than 5,000 activities per year, you should **always** offload individual deliverable tracking to the **Workflow module**. Managing high-volume "Experience" records in Planning can lead to data accumulation that obscures your strategic visibility. Use Planning for the "Why" and "What," and the Workflow module for the high-volume "How." 

 

## Architecture: Centers of Gravity 

An enterprise-grade MSOR isn't built in a single workspace. It uses a "Hub-and-Spoke" architecture where record types are managed in their natural **Centers of Gravity**. 

 

### 1. The Taxonomy Hub (Classifications) 

Establish one centralized workspace for your "Global Classifications" (e.g., Brands, Regions, Products, Personas). 

* **Primary Location:** This workspace is the "Source of Truth" for these objects. 

* **The Benefit:** By syndicating these definitions to the rest of the business, you solve "Semantic Drift"—ensuring that "Region: EMEA" means the same thing to every team. 

 

### 2. The Strategic Planning Workspace (Executive Center) 

This is where high-level **Campaigns** (and any **Channel Plans**) live.  

* **Primary Location:** This is the executive center of gravity, providing a noise-free environment for strategic decision-making. 

* **The Benefit:** Leadership can manage the portfolio without seeing the day-to-day tactical mess. 

 

### 3. Functional Spokes (Team Workspaces) 

Functional units (Social, Creative, Email) have their own workspaces to manage their **Tactics**. 

* **Primary Location:** These workspaces are the center of gravity for local team execution.  

* **The Benefit:** Teams "consume" the global campaigns and classifications from the hubs, while maintaining their own local objects (like *Media Outlets* or *Usage Rights*). 

 

## Noun-Based Governance: Speak One Language 

To ensure your blueprint holds up under pressure, follow the principle of **Noun-Based Governance**.  

 

* **Use Nouns, Not Verbs:** Name your record types after the "things" you are tracking (`Campaign`, `Tactic`), not the "actions" (`Campaigning`, `Planning`). 

* **Standardize Nomenclature:** Use the same names across all workspaces. This allows you to aggregate data across the entire portfolio for executive reporting. 

 

## What About Existing Portfolios and Programs? 

A common question for mature organizations is how to handle the Portfolios and Programs they've already built in the **Workflow module**. In the past, these objects were often used to mimic strategic planning. 

 

### 1. Portfolios & Programs → Record Types 

In many organizations, **Portfolios** are used to represent high-level Brands or Business Units (BUs), while **Programs** represent strategic themes. 

* **The Shift:** These are best modeled as **Record Types** in your **Taxonomy Hub**. By treating "Brand" or "Business Unit" as a record type, you can link them to any campaign or tactic across the entire enterprise, providing much more flexible reporting than a static Portfolio/Program structure. 

 

### 2. The "Reporting Bridge" Strategy 

While Workfront Planning is the future of strategic intent, its native reporting via **Canvas Dashboards** is still maturing. Many organizations still rely on the robust reporting capabilities tied to their legacy Portfolio and Program structures in the Workflow module. 

* **The Recommendation:** Don't delete your Portfolios and Programs yet. Instead, use **Fusion automations** to create a bridge.  

* **How it Works:** When a Tactic or Campaign is created in Workfront Planning, Fusion can automatically mirror that record into a corresponding Portfolio or Program in the Workflow module. This allows you to: 

    1. Enjoy Workfront Planning's superior **strategic visualization** (Timelines/Calendars). 

    2. Maintain your **legacy reporting** in the Workflow module for stakeholders who aren't yet ready to move to Canvas. 

## Best Practices & Tips 

### Do: 

* **Stick to the Core Path first.** Establish your Campaign-to-Tactic-to-Project flow before adding more complexity. 

* **Designate Primary Workspaces.** Ensure each record type has one "home" workspace (its center of gravity) that acts as the aggregator for reporting. 

* **Prioritize Forms for Intake.** Use record forms for groups with less sophistication in Workfront Planning to ensure metadata integrity. While Power Users may benefit from direct data entry in Table views, this should be approached with caution—bulk changes in a table can easily create data headaches for other stakeholders. 
 

### Don't: 

* **Don't say "Core".** Refer specifically to the **Workflow module** and the **Project** objects when talking about execution. 

* **Don't over-complicate.** Every additional level of hierarchy adds a "management tax." Only add levels that answer a business question you can't currently answer. 

* **Don't create silos.** Ensure your record types are shared across workspaces so teams aren't re-typing the same data.
-->