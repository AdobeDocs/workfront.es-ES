---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Administrar tipos de horas
description: Puede asociar tipos de horas con sus entradas de horas. Los tipos de horas son etiquetas que se utilizan para definir las entradas de horas. Los tipos de horas pueden ser para la hora general o para la hora específica del proyecto.
author: Alina, Lisa
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 0c45c768be1dda579e507f5f6ff4b127021a5f73
workflow-type: tm+mt
source-wordcount: '1129'
ht-degree: 4%

---

# Administrar tipos de hora

<!--Audited: 05/2025-->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

<!--<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div>-->

Los tipos de horas son etiquetas que se utilizan para definir las entradas de horas. Puede asociar tipos de horas con sus entradas de horas.

Existen dos categorías de tipos de horas:

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

+++ Amplíe para ver los requisitos de acceso.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Estándar o Plan</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso</td> 
   <td>Administrador del sistema</td>
  </tr> 
 </tbody> 
</table>

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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

Como administrador de [!DNL Workfront], puede crear tipos de horas para su organización en los niveles de sistema y proyecto.

Después de definir los tipos de horas en el nivel de sistema, los usuarios pueden definir qué tipos de horas están disponibles para proyectos específicos o para usuarios específicos.

Para obtener más información, consulte [Definir tipos de horas y disponibilidad](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Para crear tipos de horas:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Hoja de horas y horas**, luego haga clic en **Tipos de horas**.

1. En la sección **Tipos de horas**, haga clic en **Nuevo tipo de hora**.
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
      <td> <p>Seleccione si el tipo de hora es un tipo de hora general o específico del proyecto en el menú desplegable <strong>Ámbito</strong>.</p> <p>Los tipos de horas generales solo están visibles en las plantillas de horas y no pueden asociarse a proyectos, tareas o problemas.</p> <p><b>IMPORTANTE</b></p><p> Si tiene un tipo de hora personalizado [!UICONTROL Específico del proyecto] y lo cambia a [!UICONTROL General], todas las horas de tareas, problemas y proyectos existentes se establecen en sus tipos predeterminados del sistema.</p> </td> 
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

1. Haga clic en **Guardar**.

   El tipo de hora se añade al sistema de Workfront y se activa de forma predeterminada.

## Editar tipos de horas

Como administrador de [!DNL Workfront], puede editar los tipos de horas para su organización en los niveles de sistema y proyecto.

>[!NOTE]
>
>* No puede editar los tipos de horas integrados.
>* No puede editar los tipos de horas de forma masiva.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Hoja de horas y horas**, luego haga clic en **Tipos de horas**.

1. Haga clic en el nombre de un tipo de hora o seleccione el tipo de hora y, a continuación, haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png) que se encuentra en la parte superior de la lista.
1. En el cuadro de diálogo **Editar tipos de horas**, especifique la siguiente información:

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
      <td> <p>Seleccione si el tipo de hora es un tipo de hora general o específico del proyecto en el menú desplegable <strong>Ámbito</strong>.</p> <p>Los tipos de horas generales solo están visibles en las plantillas de horas y no pueden asociarse a proyectos, tareas o problemas.</p> <p><b>IMPORTANTE</b></p> <p>Si tiene un tipo de hora personalizado [!UICONTROL Específico del proyecto] y lo cambia a [!UICONTROL General], todas las horas de tareas, problemas y proyectos existentes se establecen en sus tipos predeterminados del sistema.</p> </td> 
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


1. Haga clic en **Guardar**.

   Los cambios se guardarán y se editará el tipo de hora.

## Desactivar tipos de horas

Puede desactivar los tipos de horas si ya no desea que los usuarios asocien sus horas a ellos. Al desactivar los tipos de horas, se ocultan en cualquier lugar de [!DNL Workfront] donde los tipos de horas sean visibles.

>[!NOTE]
>
>* No puede desactivar los tipos de horas integrados.
>* Puede desactivar los tipos de horas de forma masiva.
>* Al desactivar un tipo de hora específico del proyecto, todo el tiempo registrado para ese tipo toma automáticamente el valor predeterminado de un tipo de hora integrado específico del proyecto. Por ejemplo, el tiempo registrado de un proyecto se establece de forma predeterminada en el tipo de hora Hora del proyecto; el tiempo registrado de una tarea se establece de forma predeterminada en el tipo de hora Hora de la tarea.
>* Cuando se desactiva un tipo de hora general, el tiempo registrado permanece en la hoja de horas, pero los usuarios ya no podrán registrar el tiempo de ese tipo de hora en el futuro.



Para desactivar un tipo de hora:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Hoja de horas y horas]**, luego haga clic en **[!UICONTROL Tipos de horas]**.

1. Seleccione el tipo de hora que desea desactivar. Puede seleccionar varios tipos de horas.

1. Haga clic en **Más** y luego en **Desactivar**.

   ![Activar y desactivar vínculos de tipo de hora](assets/activate-and-deactivate-hour-type-links.png)

   El tipo de hora se desactiva y los usuarios ya no pueden encontrarlo al registrar horas.

1. (Opcional) Para reactivar un tipo de hora, selecciónelo en la lista **Tipos de horas** y, a continuación, haga clic en **Más** > **Activar**.

