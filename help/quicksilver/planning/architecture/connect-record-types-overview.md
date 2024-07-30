---
title: Información general sobre tipos de registros Connect
description: Una manera de indicar cómo se relacionan los tipos de registros individuales entre sí es conectarlos. Además, puede conectar tipos de registros de Adobe Workfront Planning con tipos de objetos de otras aplicaciones para mejorar la experiencia de los usuarios y mantener el enfoque en una aplicación.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 5c7b60ac5b78bd065ffc270588ec72ab3eb2f41d
workflow-type: tm+mt
source-wordcount: '1021'
ht-degree: 0%

---


<!--update metadata at GA-->
<!--add to TOC and mini TOC when live-->

# Información general sobre tipos de registros Connect

Puede indicar que los tipos de registro individuales están relacionados entre sí o con objetos de otras aplicaciones conectándolos.

Este artículo es una descripción general de cómo se conectan los tipos de registro y describe los tipos de conexiones que se pueden establecer entre los tipos de registro y de objeto.

Para obtener información acerca de los tipos de registros que conecta, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

## Consideraciones sobre la conexión de tipos de registros

* Puede conectar las siguientes entidades en Adobe Workfront Planning:

   * Dos tipos de registros

     Los tipos de registro deben pertenecer al mismo espacio de trabajo.
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

* Después de crear registros individuales para un tipo de registro, puede seleccionar los registros a los que se conecta desde el campo tipo de registro vinculado. Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

* Después de conectar un tipo de registro con otro tipo de registro o con un tipo de objeto de otra aplicación, existen los siguientes escenarios:

   * **Al conectar dos tipos de registro**: se crea un campo de registro vinculado en el tipo de registro desde el que se conecta. Se crea un campo de registro vinculado similar en el tipo de registro al que se conecta.

     Por ejemplo, si conecta el tipo de registro &quot;Campaña&quot; con el tipo de registro &quot;Producto&quot;, se crea un campo de registro vinculado denominado &quot;Producto vinculado&quot; en el tipo de registro Campaña. Se crea un tipo de registro vinculado llamado automáticamente &quot;Campaign&quot; en el tipo de registro Product.

   * **Cuando conecta un tipo de registro con un tipo de objeto de otra aplicación**:

      * Se crea un campo de registro vinculado en el tipo de registro desde el que se conecta. No se crea automáticamente ningún campo de registro vinculado en el tipo de objeto de la otra aplicación.

      * No se puede acceder a los campos de registros de Planning desde objetos de Workfront.
      * Se puede acceder a los campos de registro de planificación desde los recursos del Experience Manager cuando el administrador de Workfront configura la asignación de metadatos mediante la integración entre Workfront y Adobe Experience Manager Assets. Para obtener más información, consulte [Configuración de la asignación de metadatos de recursos entre Adobe Workfront y Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).

   * **Cuando agrega campos vinculados (o de búsqueda) desde el registro u objeto al que se conecta**: un campo vinculado (o de búsqueda) con información del registro al que se conecta se muestra en el registro desde el que se conecta.

     Puede conectar campos de otros tipos de registro u objetos de otra aplicación al tipo de registro de Workfront Planning.

     Los campos vinculados son de sólo lectura y muestran automáticamente información de registros u objetos conectados al conectar los registros o los objetos.

     Por ejemplo, si conecta el tipo de registro &quot;Campaña&quot; con un proyecto de Workfront y selecciona llevar el campo Fecha planificada de finalización del proyecto al registro de Workfront Planning, se crea automáticamente un campo vinculado llamado Fecha planificada de finalización (desde proyecto) para la campaña. Este campo vinculado no se puede editar manualmente. El campo Fecha planificada de finalización (del proyecto) muestra la fecha planificada de finalización de los proyectos vinculados.

     >[!IMPORTANT]
     >
     >Todas las personas con permisos de Vista o superiores en el espacio de trabajo pueden ver la información en los campos vinculados, independientemente de sus permisos o nivel de acceso en la aplicación de los tipos de objetos vinculados.

* Los campos de registros vinculados están precedidos por un icono de relación ![](assets/relationship-field-icon.png).

  Los campos vinculados van precedidos de un icono que identifica el tipo de campo. Por ejemplo, los campos vinculados (o de búsqueda) van precedidos de iconos que indican que un campo es un número, un párrafo o una fecha.

* Los campos de búsqueda van precedidos de un icono que indica el tipo de información que se muestra en el campo.

## Tipos de conexión

Después de establecer una conexión entre dos tipos de registro o entre un registro y un tipo de objeto de otra aplicación, puede agregar registros en los campos de registro conectados.

Según el número de registros que pueda agregar a una conexión, los siguientes son los tipos de conexión entre los que puede elegir al conectar tipos de registros:

* [Uno a varios](#one-to-many-connection-type)
* [Uno a uno](#many-to-one-connection-type)
* [Varios a uno](#many-to-one-connection-type)
* [Muchos a muchos](#many-to-many-connection-type)

<!-- add screen shots for each type of connection below-->

### Tipo de conexión uno a varios

Al seleccionar el tipo de conexión uno a varios entre los tipos de registro, puede conectar posteriormente un registro con varios registros a los que se está conectando.

Por ejemplo, si conecta campañas con proyectos, puede conectar una campaña con varios proyectos. Pero un proyecto solo se puede conectar a una campaña.

Al seleccionar este tipo de conexión, puede cambiarlo posteriormente sólo a un tipo de conexión de varios a varios.

### Tipo de conexión uno a uno

Al seleccionar el tipo de conexión uno a uno entre tipos de registro, puede conectar posteriormente un registro con otro registro al que esté conectándose.

Por ejemplo, si conecta campañas con proyectos, puede conectar una campaña con un proyecto. Un proyecto solo se puede conectar a una campaña.

Al seleccionar este tipo de conexión, puede cambiarlo posteriormente a cualquier otro tipo de conexión.

### Tipo de conexión varios a uno

Al seleccionar el tipo de conexión varios a uno entre los tipos de registro, puede conectar posteriormente muchos registros con un único registro al que se está conectando.

Por ejemplo, si conecta campañas con proyectos, puede conectar varias campañas con un proyecto. Un proyecto se puede conectar a varias campañas.

Al seleccionar este tipo de conexión, puede cambiarlo posteriormente sólo a un tipo de conexión de varios a varios.

### Tipo de conexión &quot;varios a varios&quot;

Al seleccionar el tipo de conexión varios a varios entre los tipos de registro, puede conectar posteriormente muchos registros con varios registros a los que se está conectando.

Por ejemplo, si conecta campañas con proyectos, puede conectar varias campañas con varios proyectos. También puede conectar varios proyectos a varias campañas.

Cuando selecciona este tipo de conexión, no puede cambiarlo después de guardarlo.