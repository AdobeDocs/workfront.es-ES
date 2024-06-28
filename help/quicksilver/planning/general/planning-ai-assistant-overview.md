---
title: "Descripción general del Asistente de IA de Adobe Workfront Planning"
description: Puede utilizar el asistente de IA para generar, actualizar o quitar registros en función del contexto de página actual y la estructura de registros. Los comandos del usuario y la ejecución por parte de la IA de esos comandos trabajan juntos para garantizar que los cambios realizados por la IA se reflejen con precisión en su entorno.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: e1e3b8b9f5497af47e14c0f54dfae8f2134b5159
workflow-type: tm+mt
source-wordcount: '632'
ht-degree: 0%

---


# Descripción general del Asistente de IA de Adobe Workfront Planning

<!-- update TOC and miniTOC when making this live-->

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Workfront Planning y al Asistente de IA de Workfront (beta), que son nuevas ofertas de Adobe Workfront.
>
>En la actualidad, Workfront Planning se encuentra en una fase de acceso anticipado y el Asistente de IA de Workfront se encuentra en una fase beta.
>
>Workfront Planning y el asistente de IA (beta) están abiertos a un número limitado de clientes.
>
>Debe ser cliente de Workfront para utilizar estas funciones.
>
>El representante de cuentas le informará si forma parte de esta fase.
>
>Para obtener más información, consulte [Resumen de planificación de Adobe Workfront](/help/quicksilver/planning/general/planning-overview.md).

Puede utilizar el Asistente de IA para generar, actualizar o quitar registros basados en el contexto de página y la estructura de registros actuales.

Los comandos del usuario y la ejecución por parte de la IA de esos comandos trabajan juntos para garantizar que los cambios realizados por la IA se reflejen con precisión en su entorno.

## Consideraciones sobre el asistente de IA

* El asistente de IA está disponible para los administradores de Workfront de forma predeterminada.

* El administrador de Workfront debe habilitar el asistente de IA para todos los demás usuarios. Para obtener más información, consulte [Habilitar o deshabilitar el Ayudante de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

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

## Acceso al asistente de IA

1. Inicie sesión en Workfront y vaya a **Planificación** área.

1. Haga clic en **tarjeta de workspace**.

1. (Opcional) Haga clic en un **tarjeta de tipo de registro**.

1. (Opcional) Haga clic en un **registro** para abrir el archivo del registro **Detalles** página.

1. Haga clic en **Icono de asistente de IA** en la esquina superior derecha de la pantalla, en la barra de navegación global.

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
