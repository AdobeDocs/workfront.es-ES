---
title: Introducción a Adobe Workfront Planning Designer
description: Con Adobe Planning Designer, puede generar un nuevo espacio de trabajo, con tipos de registro y campos en Workfront Planning, agregar objetos a un espacio de trabajo o ver el historial de cambios en los registros.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
hidefromtoc: true
hide: true
source-git-commit: bf34bfa2059d227eca3faa3d719adcf4d711e457
workflow-type: tm+mt
source-wordcount: '851'
ht-degree: 23%

---


# Introducción a Adobe Workfront Planning Designer

{{planning-important-intro}}

Con Adobe Planning Designer, puede generar un nuevo espacio de trabajo, con tipos de registro y campos en Workfront Planning, agregar objetos a un espacio de trabajo o ver el historial de cambios en los registros.

>[!IMPORTANT]
>
>En este momento, Planning Designer solo está disponible para los usuarios que participan en la fase beta cerrada.

## Requisitos de acceso <!--edit theses-->

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Paquetes de Adobe Workfront</p></td> 
   <td> 
<p>Cualquier paquete de Workfront y Planning</p>
<p>Cualquier paquete de flujo de trabajo y planificación</p>
   </td> </tr>

</tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Permisos de administración en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inscripción en el programa Beta cerrado para Planning Designer

<!--edit this Or create a new article under Beta programs?? -->

Actualmente, puede solicitar participar en el programa Beta cerrado para Planning Designer.

## Consideraciones sobre Planning Designer

<!--these are from the AI Assistant - edit these-->

* Para utilizar Planning Designer, primero debe habilitar el asistente de IA para su organización. Se debe habilitar lo siguiente para que el asistente de IA esté disponible para todos los miembros de la organización:

   * El asistente de IA debe estar habilitado para su organización antes de que esté disponible para los usuarios de su empresa. Para obtener más información, consulte [Descripción general del Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
   * Una vez que Workfront ha habilitado el asistente de IA para su organización, estará disponible para el administrador principal de Workfront. Para obtener más información, consulte [Configurar información básica para el sistema](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

   * El administrador de Workfront debe habilitar el asistente de IA para todos los demás usuarios. Para obtener más información, consulte [Habilitar o deshabilitar el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

   * El asistente de IA funciona en el contexto de cada página. Las solicitudes que envía para el asistente de IA deben hacer referencia a la funcionalidad que está disponible en la página que ha abierto.

* Para utilizar Planning Designer, un administrador del sistema debe activarlo en el área Preferencias del sistema de la configuración.

* Las acciones que realiza el asistente de IA en el área de planificación se encuentran en el contexto de los permisos de Workfront Planning y del nivel de acceso de Workfront. Para obtener más información, consulte los siguientes artículos:

   * [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Información general sobre el tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Los cambios realizados por el asistente de IA en nombre del usuario se rastrean en el panel del historial del registro.

* Puede utilizar comandos para deshacer las acciones. Por ejemplo, puede escribir “Deshacer el último cambio” para revertir el cambio.

* Al crear, actualizar o eliminar un objeto mediante el Asistente de IA, este muestra las acciones deseadas y solicita confirmación. A continuación, puede confirmar o cancelar las acciones.

—>

## Funcionalidad disponible actualmente para Planning Designer

<!--edit these- they are from the Ai Assistant: 

Currently, the AI Assistant is available in the Planning area of Workfront for the following pages:

* Workspace page
* Record type page
* Record page

You can use the AI Assistant to perform the following actions, at this time:

* Search for records. You can search by information contained in any record fields. 
* Create records. An ID with a link to the new record displays after the record is created. You can specify the fields you want to update during the creation process, like dates or description. 
* Create records based on a document that you upload. Workfront supports the following document formats for the AI Assistant:

    PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT, and most image formats
* Update fields for the records you see on the screen
* Delete records
* Restore records that you just deleted

-->

Puede utilizar Planning Designer o el asistente de IA para realizar cualquiera de las siguientes acciones:

* Creación y configuración de espacios de trabajo

* Crear tipos de registro

* Campos de diseño o campos de fórmula

* Crear, eliminar, duplicar y restaurar registros

* Editar, actualizar y anexar un campo en un registro

* Vincular registros a otros registros

* Acceder a historial de cambios de registro

* Creación de vistas personalizadas

* Crear registros importando un documento. La creación de registros a partir de un documento importado sólo está disponible en Planning Designer y no en el asistente de IA. <!--add information about supported files-->

  <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

## Localice Planning Designer en Workfront Planning

Puede acceder a Planning Designer desde la página principal de Workfront Planning.

<!--add screen shot-->

También puede utilizar el Asistente de IA para aprovechar la misma funcionalidad que proporciona Planning Designer.

## Habilitar Planning Designer para su organización

Como administrador de Workfront, primero debe habilitar Planning Designer para su organización.

<!--add steps here-->

## Creación o actualización de objetos mediante Planning Designer

Puede crear o actualizar objetos en Workfront Planning mediante Planning Designer o el Asistente de IA, a menos que se especifique lo contrario.

1. Inicie sesión en Workfront y, a continuación, haga clic en el icono **Menú principal** ![Menú principal de puntos](assets/dots-main-menu.png) en la esquina superior derecha de la pantalla, o en el icono **Menú principal** ![Menú principal de líneas](assets/lines-main-menu.png) en la esquina superior izquierda, si está disponible.

1. Haga clic en **Planificación**. Se abre el área de Planning.

1. Haga clic en **Diseñar con IA**.

1. En el espacio proporcionado, empiece a escribir comandos para el asistente de IA y, a continuación, haga clic en Intro cuando haya terminado.

   <!--add screen shot-->

   Por ejemplo, puede escribir una solicitud similar a las siguientes:

   * Cree y configure un espacio de trabajo con cinco tipos de registros para administrar campañas

   * Cree campañas de marketing para cada mes del año actual

   * Agregue un campo de campaña para Estado para el área de trabajo Diseño de marketing

   * Eliminar todos los registros de un estado de obsoleto

   * Actualizar todas las campañas de Planning a un estado de Activo

   * Conectar campañas a personas en el espacio de trabajo de diseño de marketing

   * Mostrar el historial de cambios de la campaña &quot;San Valentín&quot;

   * Crear una vista de cronología para las campañas en el área de trabajo Diseño de marketing

   * Crear registros importando un documento. La creación de registros a partir de un documento importado sólo está disponible en Planning Designer y no en el asistente de IA.

   <!--* Generate thumbnail and over image for a record (not available yet, maybe Q2) -->

   Se muestra una vista previa visual con un ejemplo de lo que el Ayudante puede generar.

1. Después de recibir una respuesta correcta, siga los vínculos proporcionados en la línea de comandos para crear, actualizar o revisar el objeto de la solicitud.




