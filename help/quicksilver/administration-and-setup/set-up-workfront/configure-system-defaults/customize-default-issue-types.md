---
user-type: administrator
product-area: system-administration;projects
navigation-topic: configure-system-defaults
title: Personalizar tipos de problemas predeterminados
description: Puede personalizar las etiquetas para cada tipo de problema predeterminado para que coincidan mejor con la terminología utilizada en su organización. Los tipos de problemas son útiles para personalizar los estados de los problemas y crear colas de solicitudes.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: caed65ab-a787-437b-9f5f-b3d4135bb980
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '449'
ht-degree: 0%

---

# Personalizar tipos de problemas predeterminados

Los tipos de problemas son útiles en las siguientes circunstancias:

* Al personalizar los estados de problemas, como se describe en [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).
* Al crear una cola de solicitudes, como se describe en [Crear una cola de solicitudes](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md).

Puede personalizar las etiquetas para cada tipo de problema predeterminado para que coincidan mejor con la terminología utilizada en su organización.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td> <p>Debe ser administrador de [!DNL Workfront].</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Tipos de problemas predeterminados

Si tiene acceso de [!DNL Adobe Workfront] [!UICONTROL administrador], hay cuatro tipos de problemas predeterminados que puede configurar y cambiar de nombre:

* **[!UICONTROL Informe de errores]** se usa para rastrear los errores notificados en el sistema.
* **[!UICONTROL Pedido de cambio]** se usa para hacer un seguimiento de los problemas que deben actualizarse o revisarse.
* **[!UICONTROL Problema]** Un objeto de [!DNL Workfront] que comunica trabajo no planeado, un problema que surge o algo que debe resolverse para continuar una tarea.
* **[!UICONTROL Solicitud]** Tipo de problema que se aplica a una cola de solicitudes en la que los usuarios realizan solicitudes en Workfront.

![](assets/default-issue-types.png)

## Personalización de un tipo de problema

Tenga en cuenta lo siguiente sobre la personalización de tipos de problemas:

* Puede modificar la etiqueta de un tipo de problema, pero no puede cambiar su función.
* No puede crear tipos de problemas adicionales.
* No puede cambiar los valores de filtro para el nombre de un tipo de problema. Por lo tanto, si crea un filtro en un informe de problemas, el valor del filtro (clave) no refleja el nombre personalizado del tipo de problema.
* Hay tres estados predeterminados asociados a cada tipo de problema: [!UICONTROL Nuevo], [!UICONTROL En curso] y [!UICONTROL Cerrado]. No puede eliminar estos estados ni quitarlos de un tipo de problema, pero puede cambiarles el nombre.
* Puede reordenar las opciones que aparecen en el menú desplegable para cada tipo de problema.

Para personalizar un tipo de problema:

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Preferencias del proyecto]** > **[!UICONTROL Estados]**.

1. Haga clic en la ficha **[!UICONTROL Problemas]**.
1. Realice una de las siguientes acciones:

   * Pase el ratón sobre el tipo de problema que quiera personalizar, haga clic en el icono [!UICONTROL Editar] ![](assets/edit-icon.png) que aparece en el extremo derecho y, a continuación, escriba un nombre nuevo para el tipo de problema.

     ![](assets/customize-issue-type.png)

   * Haga clic en un [!UICONTROL tipo de problema] para enumerar sus estados asociados y, a continuación, arrastre los controladores que aparecen cuando pasa el ratón por encima de ellos y suéltelos en el orden en que desea que aparezcan en el menú desplegable **[!UICONTROL Estado]** del problema de los usuarios.
