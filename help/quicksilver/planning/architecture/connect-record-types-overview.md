---
title: Información general sobre tipos de registros conectados
description: Una forma de indicar cómo se relacionan entre sí los distintos tipos de registro es conectarlos. Además, puede conectar tipos de registros de Planificación de Adobe Workfront con tipos de objetos de otras aplicaciones para mejorar la experiencia de los usuarios y mantener el enfoque en una aplicación.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: bfb0fd2956ffb9384a09882864668d5dba33a53b
workflow-type: tm+mt
source-wordcount: '1553'
ht-degree: 25%

---

# Información general de tipos de registros conectados

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>   -->

Puede indicar que los tipos de registro individuales están relacionados entre sí o con objetos de otras aplicaciones conectándolos.

Este artículo es una descripción general de las conexiones de tipo de registro y describe los tipos de conexiones que puede establecer entre los tipos de registro y de objeto.

Para obtener información acerca de los tipos de registros que conecta, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

## Consideraciones sobre la conexión de tipos de registros

Hay dos pasos para establecer conexiones en Workfront Planning:

1. Establezca una conexión entre dos tipos de registro o un tipo de registro y un tipo de objeto de otra aplicación.

   Para obtener información acerca de cómo conectar tipos de registros, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

1. Conectar un registro individual de un tipo con registros de otro tipo después de conectar los dos tipos de registros. Para obtener información acerca de cómo conectar registros, vea [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

Tenga en cuenta lo siguiente sobre la conexión de tipos de registros:

* Puede conectar las siguientes entidades en Planificación de Adobe Workfront:

   * Dos tipos de registros. 

     De forma predeterminada, puede conectar dos tipos de registros desde el mismo espacio de trabajo. También puede configurar tipos de registros para conectarse con tipos de registros de otros espacios de trabajo. Para obtener más información, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).
   * Tipo de registro y tipo de objeto de otra aplicación.

* Puede conectar los tipos de registros de Planificación de Workfront con los siguientes tipos de objetos desde las siguientes aplicaciones:

   * Adobe Workfront:

      * Proyectos
      * Portafolios
      * Programas
      * Compañías
      * Grupos

   * Adobe Experience Manager Assets:

      * Imágenes
      * Carpetas

     >[!IMPORTANT]
     >
     >Debe tener una licencia de Adobe Experience Manager Assets y la instancia de Workfront de su organización debe incorporarse a Adobe Business Platform o a Adobe Admin Console para conectar los registros de Planificación de Workfront a Adobe Experience Manager Assets.
     >
     >Si tiene preguntas acerca de la incorporación a Adobe Admin Console, consulte las [Preguntas frecuentes sobre Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Después de crear registros para los tipos de registro, puede vincularlos entre sí a través del campo de registro conectado.

  Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

* Después de conectar un tipo de registro a otro tipo de registro o a un tipo de objeto de otra aplicación, se dan los siguientes escenarios:

   * **Al conectar dos tipos de registros de Planning**: se crea un campo de registro vinculado en el tipo de registro desde el que se conecta. Se crea un campo de registro vinculado similar en el tipo de registro al que se conecta <!--<span class="preview">, only when you enable the Create corresponding field on linked record type setting on the New connection tab.</span>-->.

     Por ejemplo, si conecta el tipo de registro &quot;Campaña&quot; con el tipo de registro &quot;Producto&quot;, se crea un campo de registro vinculado (campo de conexión) denominado &quot;Producto vinculado&quot; en el tipo de registro Campaña. Se crea un tipo de registro vinculado llamado automáticamente &quot;Campaign&quot; en el tipo de registro Product.

     <!--<div class="preview">
        
        For example, the following scenarios exist: 
        * When you enable the Create corresponding field on linked record type setting and you connect the "Campaign" record type with the "Product" record type, a linked record field (connection field) that you name "Linked Product" is created on the Campaign record type. A linked record type automatically named "Campaign" is created on the Product record type.
        * When you disable the Create corresponding field on linked record type setting and you connect the "Campaign" record type with the "Product" record type, a linked record field (connection field) that you name "Linked Product" is created on the Campaign record type. A linked record type automatically named "Campaign" is not created on the Product record type.
        </div>-->

     Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).

   * **Al conectar un tipo de registro a un tipo de objeto de otra aplicación**:

      * Se crea un campo de registro vinculado en el tipo de registro desde el que se conecta. No se crea automáticamente ningún campo de registro vinculado en el tipo de objeto de la otra aplicación.
      * No se puede acceder a los campos de registros de planificación desde objetos de Workfront.
      * Los registros de Planning se pueden ver desde la pestaña Planning del objeto Workfront. Para obtener más información, consulte [Administrar conexiones de registro desde objetos de Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
      * Puede crear un campo personalizado de conexión de Planning y adjuntarlo al formulario personalizado de un objeto de Workfront. Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
      * Se puede acceder a los campos de registro de planificación desde los recursos del Experience Manager cuando la persona con la función de administrador de Workfront configura la asignación de metadatos mediante la integración entre Workfront y Adobe Experience Manager Assets. Para obtener más información, consulte [Configurar la asignación de metadatos de recursos entre Adobe Workfront y Experience Manager Assets](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


   * **Cuando se agregan campos de búsqueda desde el registro u objeto al que se conecta**: además de crear un campo de registro vinculado, también puede conectarse a campos desde el registro conectado o el tipo de objeto que se denominan campos de búsqueda. Un campo vinculado (o de búsqueda) con información del registro al que se está conectando se muestra en el registro desde el que se está conectando.

     Puede conectar campos de otros tipos de registro u objetos de otra aplicación al tipo de registro de Workfront Planning.

     Los campos vinculados son de sólo lectura y muestran automáticamente información de los registros conectados.

     Puede hacer referencia a campos de búsqueda de otros tipos de registro u objeto en fórmulas, filtros o agrupaciones.

     Por ejemplo, si conecta el tipo de registro “Campaña” a un proyecto de Workfront y selecciona llevar el campo Fecha planificada de finalización del proyecto al registro de Planificación de Workfront, se crea automáticamente un campo vinculado denominado Fecha planificada de finalización (de proyecto) para la campaña. Este campo vinculado no se puede editar manualmente. El campo Fecha planificada de finalización (de proyecto) muestra la fecha planificada de finalización de los proyectos vinculados.

     >[!IMPORTANT]
     >
     >Todas las personas con permisos de Vista o superiores en el espacio de trabajo pueden ver la información en los campos de búsqueda, independientemente de sus permisos o nivel de acceso en la aplicación de los tipos de objetos vinculados o sus permisos en otros espacios de trabajo.

     Los campos de registros vinculados están precedidos por un icono de relación ![Icono de campo de relación](assets/relationship-field-icon.png).

     Los campos vinculados van precedidos de un icono que identifica el tipo de campo. Por ejemplo, los campos vinculados (o de búsqueda) van precedidos de iconos que indican que un campo es un número, un párrafo o una fecha.

     >[!TIP]
     >
     >La información del campo de fecha de los objetos de Workfront se muestra en formato de 24 horas en Workfront Planning, independientemente de cómo se muestre en Workfront.
     >
     >Por ejemplo, si la fecha planificada de inicio de un proyecto se muestra como las 3:00 p.m. en Workfront, se mostrará como 15:00 en Workfront Planning en un campo de búsqueda importado.


## Tipos de conexión

Después de establecer una conexión entre dos tipos de registro o entre un registro y un tipo de objeto de otra aplicación, puede agregar registros en los campos de registro conectados.

>[!WARNING]
>
>Estas opciones no están disponibles al conectar lo siguiente:
>
>* Dos registros de diferentes espacios de trabajo
>
>* Un tipo de registro y recursos de Experience Manager

Puede elegir si desea conectar un registro a varios registros a la vez o un registro a la vez entre sí.

Según el número de registros que pueda agregar a un campo de registro conectado <!--and the environment you use to create the connected fields-->, los siguientes son los tipos de conexión entre los que puede elegir al conectar tipos de registros:

<!--replace the list of 4 connection types at the bottom of this commented-out section with this entire section, whenw e release to preview: 

<div class="preview">

* In the Preview environment: 

    * When the Create corresponding field on linked record type setting is disabled, you can choose from: 

        * [Multi-select](#multi-select-connection-type)
        * [Single-select](#single-select-connection-type)

</div>

* <span class="preview">In the Preview environment, when the Create corresponding field on linked record type setting is enabled,</span> or in the Production environment, you can choose from:

    * [Many to many](#many-to-many-connection-type)
    * [One to many](#one-to-many-connection-type)
    * [Many to one](#many-to-one-connection-type)
    * [One to one](#many-to-one-connection-type) 

<div class="preview">

### Multi-select connection type

![Multi-select connection type](assets/multi-select-connection-picker.png)

When you create a multi-select connection between record types, you can then select multiple connected records in the connection field from the original record type. 

For example, if you create a multi-select connection between campaigns and projects, you can select multiple projects for one campaign. A Campaign connected record type is not created for the Project object type.

After you select this connection type, you cannot change the connection type after you save it to any of the following types:

    * Single-select
    * One to many
    * Many to one
    * One to one

### Single-select connection type

![Single select connection type](assets/single-select-connection-picker.png)

When you create a single-select connection between record types, you can then select one record in the connection field from the original record type. 

For example, if you create a single-select connection between campaigns and companies, you can select one company for one campaign. A Campaign connected record type is not created for the Company object type.

After you select this connection type, you cannot change the connection type after you save it to any of the following:

    * One to many
    * One to one

</div>

-->

* [Muchos a muchos](#many-to-many-connection-type)
* [Uno a muchos](#one-to-many-connection-type)
* [Muchos a uno](#many-to-one-connection-type)
* [Uno a uno](#many-to-one-connection-type)

### Tipo de conexión &quot;varios a varios&quot;

![Selector de conexión de varios a varios](assets/many-to-many-connection-picker.png)

Al crear una conexión de varios a varios entre tipos de registro, puede seleccionar varios registros en el campo de conexión de ambos tipos de registro.

Por ejemplo, si crea una conexión de varios a varios entre campañas y proyectos, puede seleccionar varios proyectos para cada campaña y varias campañas para cada proyecto.

Un ejemplo de la vida real de un tipo de relación de varios a varios es la relación entre películas y actores. Cada película puede tener varios actores, y cada actor puede reproducir en varias películas.

Cuando selecciona este tipo de conexión, no puede cambiarlo después de guardarlo.

### Tipo de conexión uno a varios

![Selector de conexión de uno a varios](assets/one-to-many-connection-picker.png)


Al crear una conexión uno a varios entre tipos de registro, puede seleccionar varios registros en el campo de conexión del tipo de registro actual, pero el campo de conexión correspondiente del tipo de registro al que se conecta sólo permitirá seleccionar un registro. El campo de registro conectado que se crea automáticamente en el segundo tipo de registro se establece automáticamente en un tipo de relación de varios a uno.

Por ejemplo, si crea una conexión &quot;uno a varios&quot; entre campañas y proyectos, puede seleccionar varios proyectos para cada campaña, pero cada proyecto se puede conectar a una sola campaña.

Un ejemplo real de un tipo de relación &quot;uno a varios&quot; es la relación entre bibliotecas y libros: una biblioteca tiene muchos libros en su inventario; pero un libro en particular solo puede estar en una biblioteca en un momento determinado.

Al seleccionar este tipo de conexión, puede cambiarlo posteriormente sólo a un tipo de conexión de varios a varios.

### Tipo de conexión varios a uno

![Selector de conexión de varios a uno](assets/many-to-one-connection-picker.png)


Al crear una conexión varios a uno entre tipos de registro, puede conectar cada registro del tipo de registro actual con un único registro del tipo de registro conectado. El campo de registro conectado que se crea automáticamente en el segundo tipo de registro se establece automáticamente en un tipo de relación de uno a varios.

Por ejemplo, si conecta campañas con proyectos y elige este tipo de conexión, solo puede agregar un proyecto a una campaña. Sin embargo, puede agregar varias campañas a un proyecto.

Un ejemplo en la vida real de un tipo de relación de varios a uno es la relación entre muchas películas y un actor: un actor puede estar en muchas películas, pero cada película solo puede tener un actor específico una vez en su reparto.

Al seleccionar este tipo de conexión, puede cambiarlo posteriormente sólo a un tipo de conexión de varios a varios.

### Tipo de conexión uno a uno

![Selector de conexión uno a uno](assets/one-to-one-connection-picker.png)

Cuando se crea una conexión uno a uno entre tipos de registro, en ambos tipos de registro sólo se puede conectar cada registro con un registro del otro tipo.

Por ejemplo, si conecta campañas con proyectos y elige este tipo de conexión, puede conectar una campaña con un proyecto. Un proyecto solo se puede conectar a una campaña.

Un ejemplo real de una relación uno a uno es la que existe entre una persona y el identificador único de su país (como un número de la seguridad social, ID de pasaporte o ID de identificación local): cada persona tiene un único identificador para un país y cada identificador único se puede vincular a una sola persona.

Al seleccionar este tipo de conexión, puede cambiarlo posteriormente a cualquier otro tipo de conexión.
