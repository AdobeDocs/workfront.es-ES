---
title: "Prácticas recomendadas de Adobe Workfront Planning"
description: Como líder de operaciones de marketing, puede utilizar Adobe Workfront Planning para organizar el trabajo en todo el ciclo de vida de marketing para todos sus equipos. Estas son algunas prácticas recomendadas que recomendamos al comenzar con Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: d1da3ee59b074dec3e161cf1e0134aba39ad90a4
workflow-type: tm+mt
source-wordcount: '1217'
ht-degree: 0%

---


# Prácticas recomendadas de Adobe Workfront Planning

<!-- add to TOC and mini TOC-->

{{planning-important-intro}}

Como líder de operaciones de marketing, puede utilizar Adobe Workfront Planning para organizar el trabajo en todo el ciclo de vida de marketing para todos sus equipos.

Este artículo documenta algunas prácticas recomendadas que recomendamos al comenzar con Workfront Planning.

## ¿Qué es Workfront Planning?

El módulo Workfront Planning es una de las tres funcionalidades de Workfront distintas pero conectadas que, juntas, crean un sistema de registro de marketing. Las tres capacidades son:

* **Planificación**: las nuevas funciones avanzadas incluidas en Workfront Planning.

* **Flujo de trabajo**: las funciones de administración del trabajo en colaboración que utiliza hoy en día en Workfront (administración de proyectos, administración de recursos, etc.)

* **Automatización e integración**: las completas funciones de integración y automatización que ofrece Workfront Fusion.

Workfront Planning ofrece un alto grado de personalización. Para obtener más información sobre la terminología y el concepto clave de Workfront Planning, consulte [Resumen de planificación de Adobe Workfront](/help/quicksilver/planning/general/planning-overview.md).

## Preguntas que se deben hacer antes de configurar Workfront Planning

Una vez que se haya familiarizado con la terminología y arquitectura de Workfront Planning, podrá empezar a configurar su nuevo entorno.

Algunas de las preguntas que puede hacerse a sí mismo al configurar Planning son las siguientes:

* **¿Deseo utilizar espacios de trabajo para grupos organizativos más grandes? ¿O debería animar a la gente a que configure otras personales?**

  Es posible que descubra que hay un buen uso para ambos. Se recomienda no tener demasiados espacios de trabajo, ya que podrían resultar difíciles de administrar y los flujos de trabajo podrían estar demasiado fragmentados.

  >[!TIP]
  >
  >    Puede tener 1000 espacios de trabajo en una instancia de Workfront.

* **¿Qué tipos de registros personalizados debo crear en cada espacio de trabajo?**

  Los tipos de registro son como los tipos de objetos de Workfront. Piense en los flujos de trabajo y decida qué tipos de registros (objetos de trabajo, objetos de personas, taxonomías, etc.) cada flujo de trabajo puede necesitar.

  Para obtener más información, consulte [Creación de tipos de registros](/help/quicksilver/planning/architecture/create-record-types.md)

* **¿Cómo voy a crear mis registros? ¿Existe alguna lista externa o hoja de cálculo que ya contenga los registros que necesito agregar a Planning y que pueda utilizar? ¿Se añadirán registros gradualmente según las necesidades? ¿O se importarán mediante una integración de Fusion o API personalizada?**

  Para obtener más información, consulte:

   * [Creación de registros](/help/quicksilver/planning/records/create-records.md)
   * [Módulos de Adobe Workfront Planning](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-planning-modules.md)

* **¿Qué campos debo crear para mis registros?**

  Para obtener más información, consulte [Creación de campos](/help/quicksilver/planning/fields/create-fields.md).

* **¿Qué tipos de objetos de Workfront o AEM Assets necesito para conectarme a los tipos de registros de Workfront Planning para poder mostrar dependencias y crear un flujo de trabajo sin problemas para mi organización?**

  Para obtener más información, consulte [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md)

* **¿Qué calendarios y vistas de marketing necesito para contar la historia de mis campañas? ¿Y qué partes interesadas podría poner a disposición estas opiniones para una colaboración sin fisuras?**

  Para obtener más información, consulte [Administrar vistas de registros](/help/quicksilver/planning/views/manage-record-views.md).


## Prácticas recomendadas de Workfront Planning

En esta sección se enumeran varios puntos importantes y negativos, así como las directrices de prácticas recomendadas al configurar Workfront Planning.

Las directrices se organizan en función del objeto o del área que esté configurando.

### Espacios de trabajo

#### Lo que se debe hacer y lo que no se debe hacer en los espacios de trabajo

* Diseñe para el volumen más bajo de espacios de trabajo de nivel de organización

  Por ejemplo, intente crear una sola Workspace para todo el marketing

* No depure los espacios de trabajo periódicamente. Es posible que descubra que puede modificar una existente en lugar de crear una nueva desde cero.

* Cree un nuevo Workspace para un equipo que tenga un movimiento operativo completamente diferente.

  Un espacio de trabajo de &quot;Desarrollo de producto&quot; debe ser distinto de un espacio de trabajo de &quot;Marketing&quot;

* No cree un espacio de trabajo único para cada pequeña cosa. Considere los espacios de trabajo como un sistema de registro que puede beneficiar a toda una organización y permitir a todos asignar flujos de trabajo y colaborar, en lugar de un espacio privado para realizar un seguimiento de las solicitudes personales.

* No cree espacios de trabajo únicos para cada equipo o proceso dentro de una organización.

  La organización de marketing debe esforzarse por mantener un solo espacio de trabajo para mantener la visibilidad y permitir que los datos se acumulen en el nivel de planificación global.

  Evite crear espacios de trabajo similares o duplicados para equipos que sigan procesos similares (por ejemplo, marketing de EMEA VS marketing de APAC), especialmente cuando estos equipos puedan realizar trabajos que se resuman en una campaña estratégica común.

#### ¿Cómo se deben utilizar las secciones de Workspace?

* Cree y etiquete secciones para ayudar a los usuarios a comprender cómo organiza el ciclo de vida operativo.

  Por ejemplo, puede crear una sección llamada &quot;Registros principales&quot; en la que coloque sus campañas, tácticas y entregas.

* Agrupar los tipos de registros &quot;me gusta&quot;.

  Puede crear una sección llamada &quot;Geografías&quot; que contenga tipos de registros como: Región, País y Ciudad.

#### ¿Cómo debo administrar los permisos de Workspace?

* Restrinja el acceso de &quot;Administrar&quot; a un grupo selecto de personas de confianza, que no eliminarán accidentalmente un tipo de registro o que, de lo contrario, crearán campos y tipos de registro innecesarios.

  >[!TIP]
  >
  >Durante nuestro programa beta, hemos descubierto que muchos clientes sienten que concederían el acceso de &quot;Administrar&quot; a los administradores del grupo.

* No agregue el área de Planning a la plantilla de diseño de usuarios con una licencia estándar.

* No permita que los usuarios con una licencia estándar creen espacios de trabajo personales. Esto les proporciona un espacio seguro para aprender la herramienta y sentirse cómodos con ella. Esto no desordenará la experiencia para otros y puede mejorar la productividad personal del usuario.

  >[!TIP]
  >
  >    Aconsejarles que no compartan sus espacios de trabajo personales como práctica recomendada.


### Tipos de registro

#### Un campo de selección único o múltiple frente a un tipo de registro vinculado

* No genere un nuevo tipo de registro si el objeto se va a utilizar en varios tipos de registros más

  Por ejemplo, una campaña puede tener una conexión con varias audiencias de Target y una táctica puede tener una conexión con una sola audiencia de Target.

* No genere un nuevo tipo de registro si el objeto necesita almacenar valores de metadatos adicionales que puedan ser útiles en las búsquedas.

  Por ejemplo, un tipo de registro de canal como &quot;Correo electrónico&quot; puede almacenar una lista de entregables de soporte, ya sea como metadatos nativos o como conexión con un tipo de registro independiente &quot;Entregables&quot;.

* No agregue un nuevo tipo de registro si los datos que está almacenando sólo necesitan tener un ámbito de un único tipo de registro. Utilice un campo de selección en su lugar.

  Por ejemplo, un tipo de registro de campaña puede tener un campo de selección único denominado Tamaño de campaña, que solo es relevante cuando se asocia directamente con una campaña específica.

#### ¿Cómo debo etiquetar mis tipos de registros?

No cree ni etiquete tipos de registros que representen una sola construcción o sustantivo, como &quot;Campañas&quot;

:no_entry_sign: No cree un tipo de registro que se represente mejor como una capa de vista; por ejemplo, &quot;Calendario&quot; es una mala opción para un tipo de registro, ya que no es el tipo de registro en sí, sino una vista de registros.

### ¿Cuántas capas de jerarquía debo crear?

Vistas

...

Flujo de trabajo

...

### Administración de campos

Campo principal

Utilice valores de campo principal únicos para facilitar la búsqueda y la &quot;selección&quot; de esos registros al realizar conexiones.

Al realizar una conexión, los usuarios buscarán por los valores del campo Principal y, si no son únicos, los usuarios no sabrán cuál elegir.

Evite utilizar valores no únicos como campo principal porque puede crear confusión para los usuarios que tienen que buscar en el campo principal al utilizar el menú selector de conexiones.



De Chris O&#39;Neal:

Otra área en la que hay que tener en cuenta son los casos de uso que son (o no) los mejores usos de Planning. Por ejemplo, el debate sobre la administración de recursos que tuvimos hoy.



Alina&#39;s anota:

Ejemplo de artículo Prácticas recomendadas de ExL: https://experienceleague.adobe.com/en/docs/commerce-operations/implementation-playbook/best-practices/planning/sites-stores-store-views

Información adicional de Field Readiness de Lauren S.: https://fieldreadiness-adobe.highspot.com/spots/5fd14ae8b7b7390523f57346