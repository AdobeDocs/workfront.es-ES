---
user-type: administrator
content-type: reference
product-area: system-administration;timesheets
navigation-topic: configure-timesheets-and-schedules
title: Administrar tipos de hora
description: Puede asociar tipos de hora con las entradas de hora. Los tipos de hora son etiquetas que se utilizan para definir las entradas de hora.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: ad0d141b-3e56-4bb1-be24-4dd9203e7881
source-git-commit: 9f7f8a50bb805b1d6845df79ecffaa329d5abc26
workflow-type: tm+mt
source-wordcount: '759'
ht-degree: 0%

---

# Administrar tipos de hora

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. 
**Linked to Creating Billing Record-->

Puede asociar tipos de hora con las entradas de hora. Los tipos de hora son etiquetas que se utilizan para definir las entradas de hora.

Hay dos conjuntos de tipos de hora:

* **Tipos de hora específicos del proyecto**: Es el tiempo que se inicia sesión en proyectos, tareas y problemas. Los tipos de hora específicos del proyecto se pueden asociar con entradas de hora en cualquier lugar de [!DNL Adobe Workfront] donde puede registrar el tiempo para proyectos, tareas y problemas.

   Al iniciar sesión [!DNL Workfront], los tipos de hora específicos del proyecto que están disponibles dependen de las opciones de configuración establecidas en los niveles de sistema, proyecto y usuario.

   Siempre están disponibles los siguientes tipos predeterminados de hora específicos del proyecto:

   * Horas del proyecto
   * Horas de tarea
   * Hora del problema

   La variable [!DNL Workfront] el administrador determina qué tipos de hora específicos del proyecto están disponibles, tal como se describe en [Definir tipos de hora y disponibilidad para hojas de hora](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md).

   >[!NOTE]
   >
   >Si activa cualquier tipo de hora específica del proyecto en su [!DNL Workfront] del sistema, debe habilitarse al menos un tipo de hora específica del proyecto en cada proyecto del sistema. No se puede habilitar un tipo de hora específico del proyecto en el nivel del sistema y no hay tipos de hora específicos del proyecto disponibles en el nivel del proyecto.

* **Tipos de hora generales**: Las horas generales no se pueden asociar a un proyecto, tarea o problema, y se registran directamente en un parte de horas. Para obtener más información sobre el tiempo de registro, consulte [Tiempo de registro](../../../timesheets/create-and-manage-timesheets/log-time.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de [!UICONTROL Adobe Workfront]</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Tipos de hora integrados

Workfront incluye un conjunto de tipos de hora integrados. Estos tipos de hora no se pueden editar y no se pueden ocultar.

Los tipos de hora que vienen con [!DNL Workfront] son:

* **[!UICONTROL Tiempo de enfermedad]**: Tipo de hora general que no se puede asociar con entradas de hora en un proyecto, tarea o problema.
* **[!UICONTROL Tiempo de vacaciones]**: Tipo de hora general que no se puede asociar con entradas de hora en un proyecto, tarea o problema.
* **[!UICONTROL General]**: Tipo de hora general que no se puede asociar con entradas de hora en un proyecto, tarea o problema. Sin embargo, puede contabilizarse como ingresos en el proceso de planificación del proyecto.
* **[!UICONTROL Hora del proyecto]**: Tipo de hora general que solo se puede asociar con entradas de hora en un proyecto.
* **[!UICONTROL Hora de la tarea]**: Tipo de hora general que se puede asociar solo con entradas de hora en una tarea.
* **[!UICONTROL Hora del problema]**: un tipo de hora general que puede asociarse únicamente con entradas de hora sobre un problema.

## Crear tipos de hora

Como [!DNL Workfront] administrador, puede crear nuevos tipos de horas para su organización tanto en el sistema como en los niveles de proyecto. Después de crear tipos de hora en los niveles de sistema y proyecto, los usuarios pueden definir qué tipos de hora están disponibles para proyectos y usuarios específicos. Para obtener más información, consulte la [Definir tipos de hora y disponibilidad para hojas de hora](../../../timesheets/create-and-manage-timesheets/define-hour-types-and-availability.md)

Para crear nuevos tipos de hora:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe] Workfront y, a continuación, haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Hoja de horas y horas]** > **[!UICONTROL Tipos de hora]**.

1. Haga clic en **[!UICONTROL Nuevo tipo de hora].**
1. Especifique la siguiente información sobre la variable **[!UICONTROL Nuevo tipo de hora]** formulario:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Asigne un nombre al nuevo tipo de hora que sea fácilmente reconocible en el sistema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descripción]</td> 
      <td>Añada una descripción para el tipo de hora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Ámbito]</td> 
      <td> <p>Defina si el tipo de hora es un tipo de hora general o específica del proyecto seleccionando el ámbito correcto en el menú desplegable.</p> <p>Los tipos de hora generales solo están visibles en las partes de horas y no se pueden asociar a proyectos, tareas o problemas.</p> <p><b>IMPORTANTE</b>: Si tiene un tipo de hora personalizado que es [!UICONTROL Específico del proyecto], cambie a [!UICONTROL General], todas las horas existentes de tarea, problemas y proyecto se establecen en los tipos predeterminados del sistema.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Contar Como Ingresos]</td> 
      <td>Seleccione esta opción si desea que la entrada de hora asociada con este tipo de hora afecte a los cálculos de ingresos.</td> 
     </tr> 
    </tbody> 
   </table>

   **[!UICONTROL Contar como ingresos]**: Seleccione esta opción si desea que la entrada de hora asociada con este tipo de hora afecte a los cálculos de ingresos.

1. Haga clic en **[!UICONTROL Crear tipo de hora].**

## Desactivar tipos de hora

Si los tipos de hora se vuelven obsoletos y ya no desea que los usuarios asocien sus entradas de hora con ellos, puede desactivar los tipos de hora.

Al desactivar los tipos de hora, se ocultan los tipos de hora de cualquier lugar de [!DNL Workfront] donde los tipos de hora son visibles.

Para desactivar un tipo de hora:

1. Haga clic en **[!UICONTROL Configuración]** cerca de la esquina superior derecha de [!DNL Adobe Workfront] en la barra de navegación global.

1. Expandir **[!UICONTROL Preferencias de horario y horario]** y haga clic en **[!UICONTROL Tipos de hora]**.

1. Seleccione el tipo de hora que desea desactivar.

1. Haga clic en **[!UICONTROL Desactivar]**.
