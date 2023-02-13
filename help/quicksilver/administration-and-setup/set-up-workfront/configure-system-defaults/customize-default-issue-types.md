---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Personalización de tipos de problemas predeterminados
description: Puede personalizar las etiquetas de cada tipo de problema predeterminado para que coincidan mejor con la terminología utilizada en su organización. Los tipos de problemas son útiles para personalizar estados de problemas y crear colas de solicitud.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 0%

---

# Personalización de tipos de problemas predeterminados

Los tipos de problemas son útiles en las siguientes circunstancias:

* Al personalizar los estados de problemas, tal como se describe en [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* Al crear una cola de solicitudes, tal como se describe en [Crear una cola de solicitud](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Puede personalizar las etiquetas de cada tipo de problema predeterminado para que coincidan mejor con la terminología utilizada en su organización.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
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

## Tipos de problemas predeterminados

Si tiene [!DNL Adobe Workfront] [!UICONTROL administrador] acceso, hay cuatro tipos de problemas predeterminados que puede configurar y cambiar de nombre:

* **[!UICONTROL Informe de errores]** Se utiliza para rastrear los errores notificados en el sistema.
* **[!UICONTROL Cambiar orden]** Se utiliza para realizar el seguimiento de los problemas que deben actualizarse o revisarse.
* **[!UICONTROL Problema]** Un objeto de [!DNL Workfront] que comunica el trabajo no planificado, un problema que surge o algo que debe resolverse para poder continuar con una tarea.
* **[!UICONTROL Solicitud]** Tipo de problema que se aplica a una cola de solicitudes donde los usuarios realizan solicitudes en Workfront.

![](assets/default-issue-types.png)

## Personalización de un tipo de problema

Tenga en cuenta lo siguiente sobre la personalización de tipos de problemas:

* Puede modificar la etiqueta para un tipo de problema, pero no puede cambiar su función.
* No puede crear tipos de problemas adicionales.
* No se pueden cambiar los valores de filtro para el nombre de un tipo de problema. Por lo tanto, si crea un filtro en un informe de problemas, el valor del filtro (clave) no refleja el nombre personalizado del tipo de problema.
* Hay tres estados predeterminados asociados a cada tipo de problema: [!UICONTROL Nuevo], [!UICONTROL En curso]y [!UICONTROL Cerrado]. No es posible eliminar estos estados ni quitarlos de un tipo de problema, pero sí cambiarles el nombre.
* Puede volver a ordenar las opciones que aparecen en el menú desplegable para cada tipo de problema.

Para personalizar un tipo de problema:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Preferencias de proyecto]** > **[!UICONTROL Estados]**.

1. Haga clic en el **[!UICONTROL Problemas]** pestaña .
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre el tipo de problema que quiera personalizar y haga clic en el botón [!UICONTROL Editar] icono ![](assets/edit-icon.png) que aparece en el extremo derecho y, a continuación, escriba un nuevo nombre para el tipo de problema.

      ![](assets/customize-issue-type.png)

   * Haga clic en [!UICONTROL tipo de problema] para enumerar sus estados asociados, arrastre los controladores que aparecen cuando pasa el ratón sobre ellos y suéltelos en el orden en que desea que aparezcan en el problema de los usuarios **[!UICONTROL Estado]** menú desplegable.
