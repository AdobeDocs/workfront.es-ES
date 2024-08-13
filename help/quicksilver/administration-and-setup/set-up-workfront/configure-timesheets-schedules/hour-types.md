---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Administrar tipos de horas
description: Puede asociar tipos de horas con sus entradas de horas. Los tipos de horas son etiquetas que se utilizan para definir las entradas de horas.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 822c4e13ab62d129d0a7c603105251e52578576d
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 1%

---

# Administrar tipos de horas

<!--Audited: 07/2024-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

Puede asociar tipos de horas con sus entradas de horas. Los tipos de horas son etiquetas que se utilizan para definir las entradas de horas.

Existen dos conjuntos de tipos de horas:

* **Tipos de horas específicas de un proyecto**: Se trata de problemas, tareas y proyectos con sesión iniciada. Los tipos de horas específicos del proyecto se pueden asociar con las entradas de horas en cualquier lugar de [!DNL Adobe Workfront] donde pueda registrar las horas de los proyectos, las tareas y los problemas.

  Al registrar el tiempo en [!DNL Workfront], los tipos de horas específicos del proyecto que están disponibles dependen de las opciones de configuración establecidas en los niveles del sistema, del proyecto y del usuario.

  Siempre están disponibles los siguientes tipos de horas predeterminados específicos del proyecto:

   * Horas del proyecto
   * Hora de tarea
   * Hora del problema

  El administrador de [!DNL Workfront] determina qué tipos de horas específicas del proyecto están disponibles, tal como se describe en [Definir tipos de horas y disponibilidad](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

  >[!NOTE]
  >
  >Si habilita cualquier tipo de hora específico de proyecto en el sistema [!DNL Workfront], debe habilitarse al menos un tipo de hora específico de proyecto en cada proyecto del sistema. No puede habilitar un tipo de hora específico del proyecto en el sistema y no tiene tipos de horas específicos del proyecto disponibles en el nivel de proyecto.

* **Tipos de horas generales**: las horas generales no pueden asociarse a un proyecto, tarea o problema y se registran directamente en una hoja de horas.

Para obtener información sobre cómo registrar horas y asociarlas a tipos de horas, consulte [Registrar tiempo](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de [!UICONTROL Adobe Workfront]</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p>
   <p>Actual: [!UICONTROL plan]</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront].</p> <p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Tipos de horas integrados

Workfront incluye un conjunto de tipos de horas integrados. Estos tipos de horas no se pueden editar y no se pueden ocultar.

Los tipos de horas que se incluyen con [!DNL Workfront] son:

* **[!UICONTROL Tiempo de enfermedad]**: un tipo de hora general que no se puede asociar con entradas de horas en un proyecto, tarea o problema. Las horas por enfermedad no se pueden contar como ingresos.
* **[!UICONTROL Tiempo de vacaciones]**: tipo de hora general que no se puede asociar con entradas de horas en un proyecto, tarea o problema. El tiempo de vacaciones no puede contarse como ingresos.
* **[!UICONTROL Gastos generales]**: un tipo de hora general que no se puede asociar con entradas de horas en un proyecto, tarea o problema. Sin embargo, pueden contabilizarse como ingresos en el proceso de planificación del proyecto.
* **[!UICONTROL Hora del proyecto]**: un tipo de hora general que solo se puede asociar con entradas de horas en un proyecto.
* **[!UICONTROL Tiempo de tarea]**: un tipo de hora general que solo se puede asociar con entradas de hora de una tarea.
* **[!UICONTROL Hora del problema]**: un tipo de hora general que solo se puede asociar con entradas de hora de un problema.

## Crear tipos de horas

Como administrador de [!DNL Workfront], puede crear nuevos tipos de horas para su organización en los niveles de sistema y de proyecto. Después de crear tipos de horas en los niveles del sistema y del proyecto, los usuarios pueden definir qué tipos de horas están disponibles para proyectos y usuarios específicos. Para obtener más información, consulte [Definir tipos de horas y disponibilidad](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Para crear nuevos tipos de horas:

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Hoja de horas y horas]** > **[!UICONTROL Tipos de horas]**.

1. Haga clic en **[!UICONTROL Nuevo tipo de hora].**
1. Especifique la siguiente información en el formulario **[!UICONTROL Nuevo tipo de hora]**:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nombre]</td> 
      <td>Asigne un nombre al nuevo tipo de hora que sea fácilmente reconocible en el sistema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descripción]</td> 
      <td>Agregue una descripción para su tipo de hora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ámbito]</td> 
      <td> <p>Defina si el tipo de hora es un tipo de hora general o específico del proyecto seleccionando el ámbito correcto en el menú desplegable.</p> <p>Los tipos de horas generales solo están visibles en las hojas de horas y no pueden asociarse a proyectos, tareas o problemas.</p> <p><b>IMPORTANTE</b>: si tiene un tipo de hora personalizado que es [!UICONTROL Específico del proyecto] y lo cambia a [!UICONTROL General], todas las horas de tareas, problemas y proyectos existentes se establecen en sus tipos predeterminados del sistema.</p> </td> 
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

   **[!UICONTROL Contar como ingresos]**: seleccione esta opción si desea que la entrada de horas asociada con este tipo de hora afecte a los cálculos de ingresos.

1. Haga clic en **[!UICONTROL Crear tipo de hora].**

## Desactivar tipos de horas

Si los tipos de horas quedan obsoletos y ya no desea que los usuarios asocien sus entradas de horas con ellos, puede desactivar los tipos de horas.

Al desactivar los tipos de horas, se ocultan los tipos de horas de cualquier lugar de [!DNL Workfront] donde estén visibles los tipos de horas.

Para desactivar un tipo de hora:

{{step-1-to-setup}}

1. Expanda **[!UICONTROL Preferencias de horas y hoja de horas]** y luego haga clic en **[!UICONTROL Tipos de horas]**.

1. Seleccione el tipo de hora que desea desactivar.

1. Haga clic en **[!UICONTROL Desactivar]**.
