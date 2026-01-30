---
title: Información general sobre tipos de registros conectados
description: Una forma de indicar cómo se relacionan entre sí los distintos tipos de registro es conectarlos. Además, puede conectar tipos de registros de Planificación de Adobe Workfront con tipos de objetos de otras aplicaciones para mejorar la experiencia de los usuarios y mantener el enfoque en una aplicación.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 1c04c68b-7a7f-46ae-b750-2b1f79855de4
source-git-commit: 885bdb0e28c2807f14cc3919a3057a4a48b2422d
workflow-type: tm+mt
source-wordcount: '2246'
ht-degree: 15%

---


<!--keep the 30 limit verbiage in yellow til Jan 2026-->

# Información general de tipos de registros conectados

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información acerca de las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).</span>

Puede indicar que los tipos de registro individuales están relacionados entre sí o con objetos de otras aplicaciones conectándolos.

Este artículo es una descripción general de las conexiones de tipo de registro y describe los tipos de conexiones que puede establecer entre los tipos de registro y de objeto.

Para obtener información acerca de los tipos de registros que conecta, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

## Consideraciones sobre la conexión de tipos de registros

* Para que los registros u objetos individuales se conecten entre sí, los tipos de registro deben conectarse primero a los tipos de objeto.

  Puede conectar los tipos de registro y los tipos de objeto entre sí de las siguientes maneras:

   * Manualmente
   * Automáticamente

  >[!NOTE]
  >
  >Puede tener hasta 30 campos conectados para un tipo de registro en Workfront Planning.


* Tenga en cuenta lo siguiente sobre la conexión de tipos de registros y objetos:

   * Puede agregar manualmente un campo Nueva conexión desde un tipo de registro para conectar las siguientes entidades en Workfront Planning:

      * Dos tipos de registro

        De forma predeterminada, puede conectar dos tipos de registros desde el mismo espacio de trabajo. También puede configurar tipos de registros para conectarse con tipos de registros de otros espacios de trabajo, si su organización compró un paquete de Workfront o Planning superior. Para obtener más información, vea [Editar tipos de registros](/help/quicksilver/planning/architecture/edit-record-types.md).
      * Tipo de registro y tipo de objeto de otra aplicación.

     Para obtener información acerca de cómo conectar tipos de registros y objetos, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).

     Después de conectar manualmente los tipos de registros con otros tipos de registros u objetos, puede conectar registros y objetos individuales.

     Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).

   * Se establece automáticamente una conexión entre entidades en los siguientes casos:

      * Cuando se utiliza una automatización para crear registros a partir de la página de un tipo de registro.

        La conexión entre los tipos de registro o el tipo de registro y el tipo de objeto de otra aplicación se crea automáticamente cuando la automatización crea el registro u objeto conectado.

        Para obtener más información, consulte [Configuración de automatizaciones de Adobe Workfront Planning](/help/quicksilver/planning/records/configure-automations-to-create-records.md).

      * Al configurar formularios de solicitud para un tipo de registro para crear un registro o un objeto.

        La conexión entre el tipo de registro y el tipo de objeto de solicitud se crea automáticamente al enviar y aprobar una solicitud de Planning que crea un registro.

        Para obtener más información, consulte [Enviar solicitudes de Adobe Workfront Planning para crear registros](/help/quicksilver/planning/requests/submit-requests.md).

        Puede ver la solicitud original en el campo **Asunto** del área Solicitudes de Workfront <span class="preview">o en el campo Conexión de solicitud original de Workfront Planning.</span>.

   * Puede conectar los tipos de registros de Planificación de Workfront con los siguientes tipos de objetos desde las siguientes aplicaciones:

      * Adobe Workfront:

         * Proyectos
         * Portafolios
         * Programas
         * Compañías
         * Grupo

     <div class="preview">

      * Adobe Workfront:

         * Solicitud original

           El campo Conexión de solicitud original muestra el nombre de la solicitud original que crea un registro después de enviar un formulario de solicitud para Workfront Planning. El nombre de la solicitud se puede ver en el campo Subject de la solicitud de Workfront.

     </div>

      * Adobe Experience Manager Assets:

         * Imágenes
         * Carpetas

      * Adobe GenStudio for Performance Marketing

         * Marcas

        >[!IMPORTANT]
        >
        >Debe tener lo siguiente para conectarse con las marcas Adobe Experience Manager Assets y GenStudio:
        >* Licencia de Adobe Experience Manager Assets
        >* Licencia de Adobe GenStudio for Performance Marketing
        >* La instancia de Workfront de su organización debe incorporarse a Adobe Business Platform o a Adobe Admin Console para conectar los registros de Workfront Planning a Adobe Experience Manager Assets.
        >Para obtener información sobre Adobe Admin Console, consulte las [Preguntas frecuentes sobre la experiencia unificada de Adobe](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Cuando se conectan dos tipos de registro o un tipo de registro y un tipo de objeto de otra aplicación, existen los siguientes escenarios:

   * **Al conectar dos tipos de registros de Planning**: se crea un campo de registro vinculado en el tipo de registro desde el que se conecta. Un campo de registro vinculado similar se crea en el tipo de registro al que se está conectando, sólo cuando se habilita la configuración Crear campo correspondiente en el tipo de registro vinculado en la ficha Nueva conexión.

     Por ejemplo, si conecta el tipo de registro &quot;Campaña&quot; con el tipo de registro &quot;Producto&quot;, se crea un campo de registro vinculado (campo de conexión) denominado &quot;Producto vinculado&quot; en el tipo de registro Campaña. Se crea un tipo de registro vinculado llamado automáticamente &quot;Campaign&quot; en el tipo de registro Product.

     Por ejemplo, existen los siguientes escenarios:

      * Al habilitar la configuración Crear campo correspondiente en el tipo de registro vinculado y conectar el tipo de registro &quot;Campaña&quot; con el tipo de registro &quot;Producto&quot;, se crea un campo de registro vinculado (campo de conexión) que se denomina &quot;Producto vinculado&quot; en el tipo de registro de Campaña. Se crea un tipo de registro vinculado llamado automáticamente &quot;Campaign&quot; en el tipo de registro Product.
      * Cuando deshabilita la configuración Crear campo correspondiente en el tipo de registro vinculado y conecta el tipo de registro &quot;Campaña&quot; con el tipo de registro &quot;Producto&quot;, se crea un campo de registro vinculado (campo de conexión) que denomina &quot;Producto vinculado&quot; en el tipo de registro de Campaña. Un tipo de registro vinculado llamado automáticamente &quot;Campaña&quot; no se crea en el tipo de registro Producto.

     Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).

   * **Al conectar un tipo de registro a un tipo de objeto de otra aplicación**:

      * Se crea un campo de registro vinculado en el tipo de registro desde el que se conecta. No se crea automáticamente ningún campo de registro vinculado en el tipo de objeto de la otra aplicación.
      * No se puede acceder a los campos de registros de planificación desde objetos de Workfront.
      * Los registros de Planning están visibles desde la sección Planning del objeto Workfront. Para obtener más información, consulte [Administrar conexiones de registro desde objetos de Workfront](/help/quicksilver/planning/records/manage-records-in-planning-section.md).
      * Puede crear un campo personalizado de conexión de Planning y adjuntarlo al formulario personalizado de un objeto de Workfront. Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).
      * Se puede acceder a los campos de registro de planificación desde los recursos del Experience Manager cuando la persona con la función de administrador de Workfront configura la asignación de metadatos mediante la integración entre Workfront y Adobe Experience Manager Assets. Para obtener más información, consulte [Configurar la asignación de metadatos de recursos entre Adobe Workfront y Experience Manager Assets](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).
      * No se puede acceder a los campos de registro de planificación desde Marcas en GenStudio for Performance Marketing.

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

   * Debe conectar tipos de registros para poder crear jerarquías en Workfront Planning. Cuando las conexiones de tipo de registro no existen, se crean automáticamente al crear una jerarquía. Para obtener más información, vea [Crear jerarquías de área de trabajo](/help/quicksilver/planning/architecture/create-workspace-hierarchies.md).


## Tipos de conexión

Después de establecer una conexión entre dos tipos de registro o entre un registro y un tipo de objeto de otra aplicación, puede agregar registros en los campos de registro conectados.

>[!WARNING]
>
>Las opciones descritas en esta sección no están disponibles al conectar lo siguiente:
>
>* Dos registros de diferentes espacios de trabajo
>
>* Un tipo de registro y recursos de Experience Manager
>
>* Un tipo de registro y una marca Adobe GenStudio

Puede elegir si desea conectar un registro a varios registros a la vez o un registro a la vez entre sí.

A continuación se indican los tipos de conexión entre los que puede elegir al conectar tipos de registros:

* Cuando la configuración **Crear campo correspondiente en el tipo de registro vinculado** está deshabilitada, puede elegir entre:

   * [Selección múltiple](#multi-select-connection-type)
   * [Selección única](#single-select-connection-type)

* Cuando la configuración **Crear campo correspondiente en el tipo de registro vinculado** esté habilitada, podrá elegir entre:

   * [Muchos a muchos](#many-to-many-connection-type)
   * [Uno a muchos](#one-to-many-connection-type)
   * [Muchos a uno](#many-to-one-connection-type)
   * [Uno a uno](#many-to-one-connection-type)

### Tipo de conexión de selección múltiple

![Tipo de conexión de selección múltiple](assets/multi-select-connection-picker.png)

Al crear una conexión de selección múltiple entre tipos de registro, puede seleccionar varios registros conectados en el campo de conexión del tipo de registro original.

Por ejemplo, si crea una conexión de selección múltiple entre campañas y proyectos, puede seleccionar varios proyectos para una campaña. No se crea un tipo de registro conectado a Campaign para el tipo de objeto Project.

Después de seleccionar este tipo de conexión, no podrá cambiarlo después de guardarlo en ninguno de los tipos siguientes:

* Selección única
* Uno a muchos
* Muchos a uno
* Uno a uno

### Tipo de conexión de selección única

![Tipo de conexión de selección única](assets/single-select-connection-picker.png)

Cuando crea una conexión de selección única entre tipos de registro, puede seleccionar un registro del campo de conexión del tipo de registro original.

Por ejemplo, si crea una conexión de selección única entre campañas y compañías, puede seleccionar una compañía para una campaña. No se crea un tipo de registro conectado a Campaign para el tipo de objeto Company.

Después de seleccionar este tipo de conexión, no podrá cambiarlo después de guardarlo en ninguna de las siguientes opciones:

* Uno a muchos
* Uno a uno

<!--
* [Many to many](#many-to-many-connection-type)
* [One to many](#one-to-many-connection-type)
* [Many to one](#many-to-one-connection-type)
* [One to one](#many-to-one-connection-type)
-->

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
