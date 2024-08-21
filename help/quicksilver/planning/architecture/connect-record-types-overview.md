---
title: Información general sobre tipos de registros conectados
description: Una manera de indicar cómo se relacionan los tipos de registros individuales entre sí es conectarlos. Además, puede conectar tipos de registros de Adobe Workfront Planning con tipos de objetos de otras aplicaciones para mejorar la experiencia de los usuarios y mantener el enfoque en una aplicación.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 1ad86cd55459d92650ac7a24c41765e579f8bb94
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 0%

---


<!--update metadata at GA-->
<!--add mini TOC when live, already added to big TOC to get the link-->

# Información general de tipos de registros conectados

<!--REMOVE THE CONTENT BELOW FROM THE "CONNECT RECORD TYPES" ARTICLE WHEN YOU TURN THIS ARTICLE LIVE- THIS IS THE SAME CONTENT AS THERE, DUPLICATED-->

Puede indicar que los tipos de registro individuales están relacionados entre sí o con objetos de otras aplicaciones conectándolos.

Este artículo es una descripción general de las conexiones de tipo de registro y describe los tipos de conexiones que puede establecer entre los tipos de registro y de objeto.

Para obtener información acerca de los tipos de registros que conecta, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

## Consideraciones sobre la conexión de tipos de registros

Hay dos pasos para establecer conexiones en Workfront Planning:

1. Primero, debe establecer una conexión entre dos tipos de registro o un tipo de registro y un tipo de objeto de otra aplicación. Para obtener información acerca de cómo conectar tipos de registros, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).
1. En segundo lugar, puede conectar un registro individual de un tipo con registros de otro tipo después de conectar los dos tipos de registros. Para obtener información acerca de cómo conectar registros, vea [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

Tenga en cuenta lo siguiente sobre la conexión de tipos de registros:

* Puede conectar las siguientes entidades en Adobe Workfront Planning:

   * Dos tipos de registros.

     De forma predeterminada, puede conectar dos tipos de registros desde el mismo espacio de trabajo. También puede configurar tipos de registros para conectarse con tipos de registros de otros espacios de trabajo. Para obtener más información, consulte [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).
   * Tipo de registro y tipo de objeto de otra aplicación.

* Puede conectar los tipos de registros de Workfront Planning con los siguientes tipos de objetos desde las siguientes aplicaciones:

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
     >Debe tener una licencia de Adobe Experience Manager Assets y la instancia de Workfront de su organización debe incorporarse a Adobe Business Platform o a Adobe Admin Console para conectar los registros de Workfront Planning a Adobe Experience Manager Assets.
     >
     >Si tiene preguntas acerca de la incorporación a Adobe Admin Console, consulte las [Preguntas frecuentes sobre la experiencia unificada de Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Después de crear registros para los tipos de registros conectados, puede vincularlos entre sí a través del campo de registro conectado.  Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

* Después de conectar un tipo de registro con otro tipo de registro o con un tipo de objeto de otra aplicación, existen los siguientes escenarios:

   * **Al conectar dos tipos de registros de Planning**: se crea un campo de registro vinculado en el tipo de registro desde el que se conecta. Se crea un campo de registro vinculado similar en el tipo de registro al que se conecta.

     Por ejemplo, si conecta el tipo de registro &quot;Campaña&quot; con el tipo de registro &quot;Producto&quot;, se crea un campo de registro vinculado (campo de conexión) denominado &quot;Producto vinculado&quot; en el tipo de registro Campaña. Se crea un tipo de registro vinculado llamado automáticamente &quot;Campaign&quot; en el tipo de registro Product.

   * **Cuando conecta un tipo de registro con un tipo de objeto de otra aplicación**:

      * Se crea un campo de registro vinculado en el tipo de registro desde el que se conecta. No se crea automáticamente ningún campo de registro vinculado en el tipo de objeto de la otra aplicación.
      * No se puede acceder a los campos de registros de Planning desde objetos de Workfront.
      * Se puede acceder a los campos de registro de planificación desde los recursos del Experience Manager cuando el administrador de Workfront configura la asignación de metadatos mediante la integración entre Workfront y Adobe Experience Manager Assets. Para obtener más información, consulte [Configuración de la asignación de metadatos de recursos entre Adobe Workfront y Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
      * Los registros de Planning se pueden ver desde la pestaña Planning del objeto Workfront. Para obtener más información, consulte [Administrar registros en la sección Planificación de objetos de Adobe Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).

   * **Cuando se agregan campos de búsqueda desde el registro u objeto al que se conecta**: además de crear un campo de registro vinculado, también puede conectarse a campos desde el registro conectado o el tipo de objeto que se denominan campos de búsqueda. Un campo vinculado (o de búsqueda) con información del registro al que se está conectando se muestra en el registro desde el que se está conectando.

     Puede conectar campos de otros tipos de registro u objetos de otra aplicación al tipo de registro de Workfront Planning.

     Los campos vinculados son de sólo lectura y muestran automáticamente información de los registros conectados.

     Puede hacer referencia a campos de búsqueda de otros tipos de registro u objeto en fórmulas, filtros o agrupaciones.

     Por ejemplo, si conecta el tipo de registro &quot;Campaña&quot; con un proyecto de Workfront y selecciona llevar el campo Fecha planificada de finalización del proyecto al registro de Workfront Planning, se crea automáticamente un campo vinculado llamado Fecha planificada de finalización (desde proyecto) para la campaña. Este campo vinculado no se puede editar manualmente. El campo Fecha planificada de finalización (del proyecto) muestra la fecha planificada de finalización de los proyectos vinculados.

     >[!IMPORTANT]
     >
     >Todas las personas con permisos de Vista o superiores en el espacio de trabajo pueden ver la información en los campos de búsqueda, independientemente de sus permisos o nivel de acceso en la aplicación de los tipos de objetos vinculados o sus permisos en otros espacios de trabajo.

     Los campos de registros vinculados están precedidos por un icono de relación ![](assets/relationship-field-icon.png).

     Los campos vinculados van precedidos de un icono que identifica el tipo de campo. Por ejemplo, los campos vinculados (o de búsqueda) van precedidos de iconos que indican que un campo es un número, un párrafo o una fecha.

<!--## Connection types

After you establish a connection between two record types or between a record and an object type from another application, you can add records in the connected record fields. 

Depending on how many records you can add to a connected record field, the following are the connection types you can choose from when connecting record types: 

* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)

>[!WARNING]
>
>These options are not available when connecting the following: 
>* Two records from different workspaces
>
>* A record type and Experience Manager assets

### Many-to-many connection type

![](assets/many-to-many-connection-picker.png)

When you create a many-to-many connection between record types, you can then select multiple records in the connection field from both record types. 

For example, if you create a many-to-many connection between campaigns and projects, you can select multiple projects for each campaign, and multiple campaigns for each project. 

A real-life example of a many-to-many relationship type is the relationship between movies and actors. Each movie can have multiple actors, and each actor can play in multiple movies. 

When you select this connection type, you cannot change the connection type after you save it. 

### One-to-many connection type

![](assets/one-to-many-connection-picker.png)


When you create a one-to-many connection between record types, you can then select multiple records in the connection field in the current record type, but the corresponding connection field in the record type you connect to will allow selecting only one record. The connected record field that is automatically created on the second record type is automatically set to a many-to-one relationship type. 

For example, if you create a one-to-many connection between campaigns and projects, you can select multiple projects for each campaign, but each project can be connected to only one campaign.

A real-life example of a one-to-many relationship type is the relationship between libraries and books: a library has many books in its inventory; but one particular book can only be in one library at a given point in time. 

When you select this connection type, you can later change it only to a many-to-many connection type. 

### Many-to-one connection type

![](assets/many-to-one-connection-picker.png)


When you create a many-to-one connection between record types, you can then connect each record in the current record type with only one record from the connected record type. The connected record field that is automatically created on the second record type is automatically set to a one-to-many relationship type. 

For example, if you connect campaigns with projects and you choose this type of connection, you can add only one project to a campaign. But you can add multiple campaigns to one project. 

A real-life example of a many-to-one relationship type is the relationship between many movies and one actor: one actor can be in many movies, but each movie can only have a specific actor once in its cast. 

When you select this connection type, you can later change it only to a many-to-many connection type.

### One-to-one connection type

![](assets/one-to-one-connection-picker.png)

When you create a one-to-one connection between record types, in both record types you can connect each record only with one record from the other record type.

For example, if you connect campaigns with projects and you choose this type of connection, you can connect one campaign with one project. One project can be connected only to one campaign. 

A real-life example of a one-to-one relationship is the one existing between a person and their country's unique identifier (like a Social Security Number, Passport ID, local identification ID): each person has only one unique identifier for a country and each unique identifier can be linked to only one person. 

When you select this connection type, you can later change it to any other connection type. 

-->



