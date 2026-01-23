---
title: Información general sobre el asistente de IA de Adobe Workfront Planning
description: Puede utilizar el asistente de IA para generar, actualizar o eliminar registros en función del contexto de página y la estructura de registros actual. Los comandos del usuario y la ejecución por parte de la IA de esos comandos funcionan juntos para garantizar que los cambios realizados por la IA se reflejen con precisión en su entorno.
author: Alina, Becky
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: 179a20f1ae6ab723963cc78e9573560968500ac5
workflow-type: tm+mt
source-wordcount: '797'
ht-degree: 64%

---


# Información general sobre el asistente de IA de Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> -->


{{planning-important-intro}}

Puede utilizar el asistente de IA para generar, actualizar o eliminar registros en función del contexto de página y la estructura de registros actual. 

Los comandos del usuario y la ejecución por parte de la IA de esos comandos funcionan juntos para garantizar que los cambios realizados por la IA se reflejen con precisión en su entorno.

## Requisitos de acceso

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

## Consideraciones sobre el asistente de IA

* El asistente de IA debe estar habilitado para su organización antes de que esté disponible para los usuarios de su empresa. Para obtener más información, consulte [Descripción general del Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
* Una vez que Workfront ha habilitado el asistente de IA para su organización, estará disponible para el administrador principal de Workfront. Para obtener más información, consulte [Configurar información básica para el sistema](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* El administrador de Workfront debe habilitar el asistente de IA para todos los demás usuarios. Para obtener más información, consulte [Habilitar o deshabilitar el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* El asistente de IA funciona en el contexto de cada página. Las solicitudes que envía para el asistente de IA deben hacer referencia a la funcionalidad que está disponible en la página que ha abierto.

* Las acciones que realiza el asistente de IA en el área de planificación se encuentran en el contexto de los permisos de Workfront Planning y del nivel de acceso de Workfront. Para obtener más información, consulte los siguientes artículos:

   * [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Información general sobre el tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Los cambios realizados por el asistente de IA en nombre del usuario se rastrean en el panel del historial del registro.

* Las medidas adoptadas por el auxiliar de inteligencia artificial son permanentes y podrían ser irreversibles. Por ejemplo, no se puede deshacer la eliminación de un campo. Revise todas las acciones propuestas por el asistente de IA antes de aceptarlas.

* Al crear, actualizar o eliminar un objeto mediante el Asistente de IA, este muestra las acciones deseadas y solicita confirmación. A continuación, puede confirmar o cancelar las acciones.

## Funcionalidad disponible actualmente para el asistente de IA

Actualmente, el asistente de IA está disponible en el área de Planificación de Workfront para las siguientes páginas:

* Página de Workspace
* Página del tipo de registro
* Página de registro

Puede utilizar el asistente de IA para realizar las siguientes acciones en este momento:

* Búsqueda de registros. Puede buscar por la información contenida en cualquier campo de registro.
* Crear registros. Una vez creado el registro, se muestra un ID con un vínculo al nuevo registro. Puede especificar los campos que desea actualizar durante el proceso de creación, como fechas o descripciones.
* Cree registros basados en un documento que haya cargado. Workfront admite los siguientes formatos de documento para el asistente de IA:

  PPTX, PDF, DOCX, XLSX, PPT, DOC, TXT y la mayoría de los formatos de imagen
* Actualizar los campos de los registros que ve en la pantalla
* Eliminar registros
* Restaurar registros que acaba de eliminar


## Busque el asistente de IA en Workfront Planning

Puede localizar el asistente de IA en las siguientes áreas de Workfront Planning:

* La barra de navegación principal, en la esquina superior derecha de la pantalla.
* Dentro del área de detalles de un registro, después de abrirlo en la vista previa o después de abrir la página del registro.

## Acceso al asistente de IA en el área de planificación

1. Inicie sesión en Workfront y, a continuación, haga clic en el icono **Menú principal** ![Menú principal de puntos](assets/dots-main-menu.png) en la esquina superior derecha de la pantalla, o en el icono **Menú principal** ![Menú principal de líneas](assets/lines-main-menu.png) en la esquina superior izquierda, si está disponible.

. Haga clic en **Planificación**. Se abre el área de Planning.

1. Haga clic en una **tarjeta del espacio de trabajo**.

1. (Opcional) Haga clic en una **tarjeta de tipo de registro**.

1. (Opcional) Haga clic en un **registro** para abrir la página **Detalles** del registro.

1. Haga clic en el icono **Asistente de IA** en la esquina superior derecha de la pantalla en la barra de navegación global o en la esquina superior derecha de la página o vista previa del registro.

   ![icono del Asistente de IA](assets/ai-assistant-icon-highlighted.png)

1. En el espacio proporcionado, empiece a escribir comandos para el asistente de IA y, a continuación, haga clic en Intro cuando haya terminado.

   ![Panel del asistente de IA con el cuadro de comandos vacío](assets/ai-assistant-panel-with-empty-command-box.png)

   Por ejemplo, puede escribir una de las siguientes opciones:

   * Cree una campaña con la fecha de inicio del 4 de julio y la fecha de finalización del 30 de julio
   * Actualice el campo Descripción del registro de campaña de verano con la fecha por determinar
   * Eliminar el último registro
   * Restaurar el registro

   Se muestra un indicador visual mientras el asistente de IA procesa los comandos, lo que establece las expectativas del tiempo de respuesta.

   Después de recibir una respuesta correcta, siga los vínculos proporcionados u observe los cambios que aparecen a la izquierda.



