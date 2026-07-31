---
content-type: release-notes
title: Actividad de la versión del cuarto trimestre de 2026 para Adobe Workfront Planning
description: Esta es la actividad de lanzamiento del producto Adobe Workfront Planning para el cuarto trimestre de 2026.
author: Becky
feature: Product Announcements
role: Admin
recommendations: noDisplay, noCatalog
source-git-commit: 6b8fc9e010c850625deb3927483f79da190e3f33
workflow-type: tm+mt
source-wordcount: '601'
ht-degree: 3%

---

# Actividad de la versión del cuarto trimestre de 2026 para Adobe Workfront Planning

Este artículo describe las funciones que se lanzarán para Workfront Planning durante la versión del cuarto trimestre de 2026.

Para obtener una lista de todas las características publicadas para Adobe Workfront Planning, consulte [Actividad de la versión de Adobe Workfront Planning: índice de artículo](/help/quicksilver/product-announcements/product-releases/planning-release-activity/planning-release-activity-article-index.md).

## Arrastrar y soltar filas en la vista de tabla

>[!NOTE]
>
>Vista previa: 30 de julio de 2026>Versión rápida de producción: 13 de agosto de 2026>Producción para todos: 15 de octubre de 2026

Se ha mejorado visualmente la experiencia de arrastrar y soltar filas en la vista de tabla.

Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).


## Campos de registro conectados dependientes

>[!NOTE]
>
>Vista previa: 30 de julio de 2026>Versión rápida de producción: 13 de agosto de 2026>Producción para todos: 15 de octubre de 2026

Los administradores de Workspace ahora pueden definir dependencias entre tipos de registros conectados. Por ejemplo, si se garantiza un campo de Región, solo se muestran los valores vinculados a la Información geográfica seleccionada. Esto se configura directamente en la configuración del campo de conexión: al agregar una conexión desde un tipo de registro geográfico a un tipo de registro dependiente (como Región), una nueva configuración permite a los administradores de espacio de trabajo marcarlo como dependiente del tipo de registro geográfico, utilizando las relaciones ya establecidas entre esos tipos de registro.

Una vez configurado, cualquier tipo de registro que haga referencia a ambos campos (como una campaña) verá el efecto inmediatamente: al seleccionar un valor geográfico, el selector de regiones se reduce a solo las regiones realmente vinculadas a esa región geográfica. Esto aplica la estructura de registros automáticamente, eliminando las combinaciones que no coinciden y reduciendo la limpieza manual.

Esta actualización incluye las siguientes funciones:

* Hemos agregado la nueva sección Configuración de conexión en la pestaña Nueva conexión, al conectar tipos de registro
* Hemos añadido la opción Hacer esta conexión dependiente en la nueva sección


Para obtener más información, consulte [Administrar conexiones dependientes](/help/quicksilver/planning/architecture/manage-dependent-connections.md).




## Mostrar el nuevo indicador de comentario de un registro en la vista de tabla

>[!NOTE]
>
>Vista previa: 30 de julio de 2026>Versión rápida de producción: 13 de agosto de 2026>Producción para todos: 15 de octubre de 2026

Se ha agregado un nuevo indicador que muestra cuándo hay comentarios no leídos en un registro. El indicador se muestra en la esquina superior derecha del campo principal del registro en la vista de tabla.

Para obtener más información, consulte [Administrar comentarios de registro](/help/quicksilver/planning/records/manage-record-comments.md).

## Color de registro personalizable y codificación de color basada en la conexión

>[!NOTE]
> 
>Vista previa: 23 de julio de 2026>Versión rápida de producción: 13 de agosto de 2026>Producción para todos: 15 de octubre de 2026

Los registros ahora admiten paletas de color personalizables que permiten actualizar los colores asignados automáticamente a los nuevos registros a colores estándar o personalizados.

En esta mejora se incluyen los siguientes cambios: 

* Se ha añadido la opción Color a las siguientes áreas:
  * El icono Campos de la vista de tabla. 
  * La sección Estilo de barra del área Configuración de una vista de cronología y calendario

    Cuando la opción Color está activada, el color asignado a un nuevo registro se muestra en todas partes donde el registro se muestra en estas vistas. 

* Se agrega un círculo de color a la página Detalles del registro. 
* Ahora puede agregar campos de registro de selección única, múltiple y conectada a la codificación de color de las barras en las vistas de cronología y calendario al colorear por valores de campo. 
* Puede habilitar la visualización del color, además del nombre y la imagen de un registro al crear campos de registro conectados. 
* La sección Color del área de Configuración también se ha optimizado eliminando la opción &quot;Ninguno&quot;.  

Para obtener más información, consulte [Crear registros](/help/quicksilver/planning/records/create-records.md). 

## La planificación de Designer ahora requiere la aceptación del acuerdo de Beta

>[!NOTE]
>Vista previa y producción para todos los clientes: 20 de julio de 2026>[!BADGE Programa inadecuado]{type=Neutral}

La planificación de Designer ahora requiere un acuerdo de Beta aceptado para su uso. Su empresa no tiene que firmar un acuerdo de IA. Esto está disponible para todos los clientes.

Para ello, hemos trasladado la opción de Planning Designer a la sección Configuración en la sección Inclusión en las pruebas beta de IA.

Al iniciar Planning Designer sin un acuerdo de Beta aceptado, ahora se solicitará la aceptación antes de que se abra el generador de espacios de trabajo.

Para obtener más información, consulte [Introducción a Adobe Workfront Planning Designer](/help/quicksilver/planning/general/planning-ai-designer.md).
