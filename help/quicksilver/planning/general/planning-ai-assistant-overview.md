---
title: Información general sobre el asistente de IA de Adobe Workfront Planning
description: Puede utilizar el asistente de IA para generar, actualizar o quitar registros en función del contexto de página actual y la estructura de registros. Los comandos del usuario y la ejecución por parte de la IA de esos comandos trabajan juntos para garantizar que los cambios realizados por la IA se reflejen con precisión en su entorno.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 53f57953-fb9f-47ef-be18-a7164c844682
source-git-commit: 170edee352f1219986057dbb7d77228f84d855b1
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---


# Descripción general del Asistente de IA de Adobe Workfront Planning

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span> 
-->

{{planning-important-intro}}

Puede utilizar el Asistente de IA para generar, actualizar o quitar registros basados en el contexto de página y la estructura de registros actuales.

Los comandos del usuario y la ejecución por parte de la IA de esos comandos trabajan juntos para garantizar que los cambios realizados por la IA se reflejen con precisión en su entorno.

## Consideraciones sobre el asistente de IA

* El asistente de IA debe estar habilitado para su organización antes de que esté disponible para los usuarios de su empresa. Para obtener más información, consulte [Descripción general del Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md).
* Una vez que Workfront ha habilitado el asistente de IA para su organización, estará disponible para el administrador principal de Workfront. Para obtener más información, vea [Configurar información básica para el sistema](/help/quicksilver/administration-and-setup/get-started-wf-administration/configure-basic-info.md).

* El administrador de Workfront debe habilitar el asistente de IA para todos los demás usuarios. Para obtener más información, consulte [Habilitar o deshabilitar el Asistente para IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

* El asistente de IA funciona en el contexto de cada página. Las solicitudes que envía para el asistente de IA deben hacer referencia a la funcionalidad que está disponible en la página que ha abierto.

* Las acciones que realiza el asistente de IA en el área de Planning se encuentran en el contexto de los permisos de Workfront Planning y del nivel de acceso de Workfront. Para obtener más información, consulte los siguientes artículos:

   * [Información general sobre los permisos de uso compartido en Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md)
   * [Información general sobre el tipo de licencia al usar Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md)

* Los cambios realizados por el asistente de IA en nombre del usuario se rastrean en el panel del historial del registro.

* Puede utilizar comandos para deshacer las acciones. Por ejemplo, puede escribir &quot;Deshacer el último cambio&quot; para revertir el cambio.

## Funcionalidad disponible actualmente para el asistente de IA

Actualmente, el Asistente de IA está disponible en el área de Planificación de Workfront para las siguientes páginas:

* página de Workspace
* Página de tipo de registro
* Página de registro

Puede utilizar el asistente de IA para realizar las siguientes acciones en este momento:

* Buscar registros. Puede buscar por la información contenida en cualquier campo de registro.
* Crear registros. Una vez creado el registro, se muestra un ID con un vínculo al nuevo registro. Puede especificar los campos que desea actualizar durante el proceso de creación, como fechas o descripciones.
* Cree registros basados en un documento que haya cargado. Workfront admite los siguientes formatos de documento para el asistente de IA:

  .pptx, .pdf, .docx, .xlsx, .ppt, .doc, .txt y la mayoría de los formatos de imagen
* Actualizar los campos de los registros que ve en la pantalla
* Eliminación de registros
* Restaurar registros que acaba de eliminar


<!-- ## Locate the AI Assistant in Workfront Planning

You can locate the AI Assistant in the following areas of Workfront Planning:

* The main navigation bar, in the upper-right corner of the screen.
* Inside the details area of a record, after you opened the record in the preview or after you opened the record's page. 

-->

## Acceso al asistente de IA en el área de planificación

1. Inicie sesión en Workfront y, a continuación, haga clic en el icono **Menú principal** ![](assets/dots-main-menu.png) en la esquina superior derecha de la pantalla, o en el icono **Menú principal** ![](assets/lines-main-menu.png) en la esquina superior izquierda, si está disponible.

. Haga clic en **Planificación**. Se abre el área de Planning.

1. Haga clic en una **tarjeta del área de trabajo**.

1. (Opcional) Haga clic en una **tarjeta de tipo de registro**.

1. (Opcional) Haga clic en un **registro** para abrir la página **Detalles** del registro.

1. Haga clic en el icono **Asistente de IA** en la esquina superior derecha de la pantalla en la barra de navegación global <!--or in the upper-right corner of the record's preview or page.-->

   ![](assets/ai-assistant-icon-highlighted.png)

1. En el espacio proporcionado, empiece a escribir comandos para el Ayudante de IA y, a continuación, haga clic en Entrar cuando haya terminado.

   ![](assets/ai-assistant-panel-with-empty-command-box.png)

   Por ejemplo, puede escribir una de las siguientes opciones:

   * Cree una campaña con la fecha de inicio del 4 de julio y la fecha de finalización del 30 de julio
   * Actualice el campo Description del registro de campaña de verano con la fecha por determinar
   * Eliminar el último registro
   * Restauración del registro

   Se muestra un indicador visual mientras el asistente de IA procesa los comandos, lo que establece las expectativas del tiempo de respuesta.

   Después de recibir una respuesta correcta, siga los vínculos proporcionados o observe los cambios a la izquierda.



