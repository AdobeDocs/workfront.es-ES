---
title: Resumen de la sección Historial
description: Puede revisar los cambios realizados en el registro y registrados por el sistema en el panel derecho de un registro en Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 8258589f-a7c3-4d77-9abe-c99e9184bd21
source-git-commit: e54142e189cd4f407161401203a7f13c752ad404
workflow-type: tm+mt
source-wordcount: '446'
ht-degree: 4%

---

# Resumen de la sección Historial

{{maestro-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

Puede colaborar en registros de Adobe Workfront Planning agregando comentarios o respuestas en el panel derecho de un registro. También puede ver otros cambios realizados en el registro y registrados por el sistema en esta área.

El panel derecho de un registro muestra las siguientes secciones:

* **Comentarios**: Muestra comentarios y respuestas que los usuarios agregan a los registros. Para obtener más información sobre la administración de comentarios en registros de Workfront Planning, consulte [Administrar comentarios de registro](/help/quicksilver/maestro/records/manage-record-comments.md).
* **Historial**: Muestra los cambios registrados por el sistema que los usuarios realizan en los campos de registro.

## Busque la sección Historial de un registro

{{step1-to-maestro}}

El último espacio de trabajo al que se accede se abre de forma predeterminada.

1. Elija una vista de tabla de la **Ver** menú desplegable.
1. Haga clic en el nombre de un registro en la vista de tabla.

   Se abre la página del registro. El área Comentarios se abre de forma predeterminada en el panel derecho.
1. Haga clic en **Mostrar historial** icono ![](assets/show-history-icon.png). Todos los cambios realizados en los campos del registro se muestran en el panel derecho, empezando por el más reciente.
1. (Opcional) Haga clic en **Ocultar historial** icono ![](assets/hide-history-icon.png) para cerrar el panel derecho.

## Consideraciones sobre la sección Historial

Puede revisar los cambios realizados en los campos de registro en la sección Historial del panel derecho de la página de un registro.

![](assets/history-area-in-comments.png)

* Workfront Planning registra la siguiente información en la sección Historial:

   * Cualquier cambio de campo

   * Los valores antiguos y nuevos de los campos, cuando cambian los valores. Los valores antiguos se muestran en formato tachado.

   * El nombre completo del usuario que realizó el cambio

   * Una marca de fecha y hora de cuándo se produjo el cambio.

* Los campos de los siguientes tipos siempre muestran el valor antiguo (en formato tachado) y el nuevo:

   * Texto
   * Párrafo
   * Divisa
   * Fecha
   * Número
   * Porcentaje
   * Selección única

* Los campos de los siguientes tipos muestran el valor antiguo en formato tachado sólo si se ha quitado al menos uno de los valores múltiples:

   * Selección múltiple
   * Campos de registro vinculados
   * Personas

  Si el cambio solo agrega valores al campo, el valor antiguo no se muestra y solo se muestra el nuevo valor de campo.

* Los campos de tipo casilla de verificación nunca muestran el valor antiguo en formato tachado. Si se edita el campo, solo se muestra el estado actual en el momento en que se realizó el cambio.

  Para obtener más información sobre los campos de Workfront Planning, consulte [Creación de campos](/help/quicksilver/maestro/fields/create-fields.md).

* Los cambios en los campos de los siguientes tipos no se muestran en la sección Historial:

   * Campos vinculados (búsqueda)
   * Fórmula
   * Creado por
   * Fecha de creación
   * Última modificación realizada por
   * Fecha de la última modificación

* Si se quita un campo del sistema, las actualizaciones realizadas en ese campo permanecen en la sección Historial. No hay ninguna indicación de que el campo se haya eliminado en la sección Historial de un registro.
