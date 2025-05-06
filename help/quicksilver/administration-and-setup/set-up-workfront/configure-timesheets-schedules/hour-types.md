---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Administrar tipos de horas
description: Puede asociar tipos de horas con sus entradas de horas. Los tipos de horas son etiquetas que se utilizan para definir las entradas de horas.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 3827e834a71084f14a99cb27aadefd97327b02d7
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 9%

---

# Administrar tipos de hora

<!--Audited: 05/2025-->

<!--Audited: 07/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

Los tipos de horas son etiquetas que se utilizan para definir las entradas de horas. Puede asociar tipos de horas con sus entradas de horas.

Existen dos conjuntos de tipos de horas:

* Tipos de horas específicos de un proyecto: se trata de proyectos, tareas y problemas con sesión iniciada. Los tipos de horas específicos del proyecto se pueden asociar con las entradas de horas en cualquier lugar de [!DNL Adobe Workfront] donde pueda registrar las horas de los proyectos, las tareas y los problemas.

  Al registrar el tiempo en [!DNL Workfront], los tipos de horas específicos del proyecto que están disponibles dependen de las opciones de configuración establecidas en los niveles del sistema, del proyecto y del usuario.

  Siempre están disponibles los siguientes tipos de horas predeterminados específicos del proyecto:

   * Horas del proyecto
   * Hora de tarea
   * Hora del problema

  El administrador de [!DNL Workfront] determina qué tipos de horas específicas del proyecto están disponibles, tal como se describe en [Definir tipos de horas y disponibilidad](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Si habilita cualquier tipo de hora específico de proyecto en el sistema [!DNL Workfront], debe habilitarse al menos un tipo de hora específico de proyecto en cada proyecto del sistema. No puede habilitar un tipo de hora específico del proyecto en el sistema y no tiene tipos de horas específicos del proyecto disponibles en el nivel de proyecto.

* Tipos de horas generales: las horas generales no se pueden asociar a un proyecto, tarea o problema y se registran directamente en una hoja de horas.

Para obtener información sobre cómo registrar horas y asociarlas a tipos de horas, consulte [Registrar tiempo](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: estándar</p>
   <p>O</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Administrador del sistema</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipos de horas integrados

Workfront incluye un conjunto de tipos de horas integrados. Estos tipos de horas no se pueden editar ni ocultar.

Los tipos de horas que se incluyen con [!DNL Workfront] son:

* **[!UICONTROL Tiempo de enfermedad]**: un tipo de hora general que no puede asociarse con entradas de horas en un proyecto, tarea o problema. Las horas por enfermedad no pueden contabilizarse como ingresos.
* **[!UICONTROL Tiempo de vacaciones]**: tipo de hora general que no puede asociarse con entradas de horas en un proyecto, tarea o problema. El tiempo de vacaciones no puede contabilizarse como ingresos.
* **[!UICONTROL Gastos generales]**: un tipo de hora general que no puede asociarse con entradas de horas en un proyecto, tarea o problema. Puede contar como ingresos en el proceso de planificación del proyecto.
* **[!UICONTROL Hora del proyecto]**: un tipo de hora general que solo se puede asociar con entradas de horas en un proyecto.
* **[!UICONTROL Tiempo de tarea]**: un tipo de hora general que solo se puede asociar con entradas de hora en una tarea.
* **[!UICONTROL Hora del problema]**: un tipo de hora general que solo puede asociarse con entradas de hora en un problema.

## Crear tipos de horas

Como administrador de [!DNL Workfront], puede crear nuevos tipos de horas para su organización en los niveles de sistema y de proyecto. Después, los usuarios pueden definir qué tipos de horas están disponibles para proyectos y usuarios específicos. Para obtener más información, consulte [Definir tipos de horas y disponibilidad](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Para crear nuevos tipos de horas:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Hoja de horas y horas**, luego haga clic en **Tipos de horas**.

1. En la sección **Tipos de horas**, haga clic en **+ Nuevo tipo de hora**.
1. En el cuadro de diálogo **Nuevos tipos de horas**, especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Introduzca un nombre de tipo de hora fácilmente reconocible en el sistema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td>Agregue una descripción para su tipo de hora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Scope]</td> 
      <td> <p>Seleccione si el tipo de hora es un tipo de hora general o específico del proyecto en el menú desplegable <strong>Ámbito</strong>.</p> <p>Los tipos de horas generales solo están visibles en las plantillas de horas y no pueden asociarse a proyectos, tareas o problemas.</p> <p><b>IMPORTANTE</b>: si tiene un tipo de hora personalizado que es [!UICONTROL Específico del proyecto] y lo cambia a [!UICONTROL General], todas las horas de tareas, problemas y proyectos existentes se establecen en sus tipos predeterminados del sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Contar como ingresos]</td> 
      <td><p>Seleccione esta opción si desea que la entrada de horas asociada con este tipo de hora afecte a los cálculos de ingresos.</p>
      <p>El tiempo por enfermedad y el tiempo de vacaciones no se pueden contar como ingresos.</p>
      <p><b>NOTA</b></p>
      <p>Cuando los tipos de hora generales se cuentan como ingresos, la tasa de coste asociada al perfil del usuario que registra la hora se asocia al coste de la hora.  
      </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **[!UICONTROL Crear tipo de hora].**

## Desactivar tipos de horas

Puede desactivar los tipos de horas si ya no desea que los usuarios asocien sus horas a ellos. Al desactivar los tipos de horas, se ocultan en cualquier lugar de [!DNL Workfront] donde los tipos de horas sean visibles.

Para desactivar un tipo de hora:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Hoja de horas y horas]**, luego haga clic en **[!UICONTROL Tipos de horas]**.

1. Seleccione el tipo de hora que desea desactivar.

1. Haga clic en **[!UICONTROL Desactivar]**.

   ![Botón Desactivar](assets/deactivate-button.png)
