---
title: Utilizar el colaborador del coordinador del proyecto
content-type: reference
description: Aprenda a utilizar el Coordinador de proyectos, un colaborador de IA incorporado que supervisa el estado del proyecto y realiza un seguimiento de las tareas vencidas.
author: Becky
feature: Work Management, Projects
source-git-commit: 13403cc11448a0611ad0996ed21e1745277e9c05
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 8%

---
# Utilizar el colaborador del coordinador del proyecto

{{highlighted-preview-article-level}}

El coordinador del proyecto es un colaborador de IA incorporado que supervisa el proyecto y notifica a las partes interesadas la información importante sobre el estado.

El uso de un coordinador de proyectos no requiere que configure un agente fuera de Workfront.

Para obtener instrucciones sobre cómo configurar un coordinador de proyecto, consulte [Configurar un coordinador de proyecto](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) en el artículo Configurar colaboradores de IA.

Para obtener información sobre los colaboradores de IA en general, consulte [Configuración de colaboradores de IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Seleccionar, Prime o Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p></td>
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Debe tener permiso de administración en los proyectos para asignar un coordinador de proyectos.</td> 
  </tr>
  </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Resumen del coordinador del proyecto

El coordinador del proyecto supervisa el proyecto y ayuda a que el trabajo siga su curso. Cuando se asigna a un proyecto, envía actualizaciones de proyecto según una programación configurada por el administrador. Las actualizaciones pueden incluir:

* Resumen del progreso
* Estado del proyecto
* Tareas o aprobaciones vencidas o en riesgo
* Faltan campos o asignaciones

El coordinador del proyecto también puede realizar comentarios sobre el proyecto y sus tareas.

El administrador configura la frecuencia con la que se envían las actualizaciones, la hora a la que se envían y quién las recibe.

También puede ejecutar el Coordinador de proyectos bajo demanda mencionándolo en una actualización del proyecto. El coordinador del proyecto se ejecuta cuando se menciona, aunque no esté programado para ejecutarse en ese momento.

>[!NOTE]
>
>El comportamiento del coordinador del proyecto puede cambiar antes de la disponibilidad general.

## Agregar el coordinador del proyecto a un proyecto

Un administrador debe crear primero el Coordinador de proyectos y agregar el campo **Coordinador de proyectos** al encabezado del proyecto en la plantilla de diseño. Luego aparece el campo en el encabezado del proyecto.

Para obtener más información, consulte [Personalización de los encabezados de los objetos mediante una plantilla de diseño](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-object-headers.md).

Para asignar un coordinador de proyecto a un proyecto:

1. Vaya al proyecto para el que desea asignar un coordinador de proyecto.
1. En el encabezado del proyecto, haga clic en el campo **Coordinador del proyecto**.
1. Seleccione el coordinador del proyecto que desee asignar.

   La ventana muestra una descripción del coordinador del proyecto seleccionado, así como las acciones que realiza el coordinador del proyecto.
1. Haga clic en **Aplicar**.

## Ejecute el coordinador del proyecto mencionándolo

Además de las actualizaciones programadas, puede almacenar en déclencheur al coordinador del proyecto en cualquier momento @mentioning en una actualización del proyecto. El coordinador del proyecto se ejecuta en cuanto se menciona, aunque no esté programado para ejecutarse en ese momento.

Para mencionar al Coordinador del Proyecto:

1. Vaya al proyecto que tiene asignado el coordinador del proyecto.
1. Abra el área **Actualizaciones** del proyecto.
1. En el campo de actualización, escriba **@** y seleccione el Coordinador del proyecto.
1. Añada el mensaje y, a continuación, publique la actualización.

   El coordinador del proyecto ejecuta y publica su respuesta.

>[!NOTE]
>
>Se debe asignar al proyecto el coordinador del proyecto antes de que pueda almacenarlo en déclencheur con un @mention.

## Configuración del coordinador del proyecto

Para obtener instrucciones sobre cómo configurar el coordinador del proyecto, consulte [Configurar el coordinador del proyecto](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md#configure-a-project-coordinator) en el artículo Configurar colaboradores de IA.
