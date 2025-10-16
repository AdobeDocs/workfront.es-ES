---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurar actualizaciones del sistema
description: Workfront genera actualizaciones automáticas del sistema en el área [!UICONTROL Actualizaciones] de un objeto para registrar los cambios que los usuarios realizan en el objeto. Como administrador de  [!DNL Workfront] , puede configurar qué acciones y campos de objeto rastrea  [!DNL Workfront]  para registrar las actualizaciones del sistema.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: c8987d036e1c1324618cb53ebcbb8fd7e4bcc6a4
workflow-type: tm+mt
source-wordcount: '930'
ht-degree: 50%

---

# Configurar las actualizaciones del sistema

<!-- Audited: 08/2025 -->

<!--

<div class="preview">

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release.     

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). 

</div> -->

[!DNL Adobe Workfront] genera actualizaciones automáticas del sistema en el área [!UICONTROL Actualizaciones] de un objeto para registrar los eventos siguientes:

* Cambios que los usuarios realizan en un campo de objeto
* Acciones que los usuarios realizan en un objeto

Estas actualizaciones del sistema incluyen el siguiente tipo de información:

* El cambio que se realizó
* El nombre del usuario que realizó el cambio
* La fecha y hora del cambio

Para obtener más información sobre las actualizaciones del sistema, consulte [Actualizaciones con seguimiento del sistema](../system-tracked-update-feeds/system-tracked-update-feeds.md).

Como administrador de [!DNL Workfront], puede configurar los campos de objeto y las acciones que [!DNL Workfront] realiza para registrar las actualizaciones del sistema.

Por ejemplo, puede hacer que [!DNL Workfront] realice un seguimiento de todos los cambios que los usuarios realicen en los nombres de los problemas en todo el sistema. Cualquier cambio en el nombre del problema aparecerá como una actualización del sistema en el área [!UICONTROL Actualizaciones] del problema.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td><p>[!UICONTROL System Administrator]</p></td>
  </tr> 
 </tbody> 
</table>

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: [!UICONTROL Standard]</p>
   Or
   <p>Current: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table> -->

## Determine en qué campos realiza un seguimiento [!DNL Workfront] para un tipo de objeto.

Puede determinar qué información rastrea [!DNL Workfront] cuando los usuarios cambian la información asociada con un tipo de objeto determinado en toda la interfaz de [!DNL Workfront]. Para ello, añada o elimine los campos en los que desea que [!DNL Workfront] realice un seguimiento para ese tipo de objeto.

>[!NOTE]
>
>* [!DNL Workfront] no puede rastrear y registrar actualizaciones acerca de campos personalizados calculados.
>* Puede personalizar la actualización del sistema para proyectos, tareas, problemas, portafolios, programas y usuarios. No puede personalizar la actualización del sistema para plantillas, documentos u hojas de horas, pero [!DNL Workfront] registra las actualizaciones del sistema para estos objetos.
>


### Añada los campos en los que desee que [!DNL Workfront] realice un seguimiento {#add-fields-you-want-workfront-to-track}

Puede añadir los campos en los que desee que [!DNL Workfront] realice un seguimiento para un tipo concreto de objeto en toda la interfaz de [!DNL Workfront]. Cuando los usuarios cambian la información de ese campo, [!DNL Workfront] registra la información sobre el cambio como una actualización del sistema en el área de [!UICONTROL Actualizaciones] del objeto.

>[!NOTE]
>
>Puede realizar un seguimiento de hasta 300 campos integrados y personalizados en las fuentes de actualización. Si realiza el seguimiento del número máximo de campos y desea realizar el seguimiento de campos adicionales que no se muestran en la subpestaña [!UICONTROL Todos los campos], primero debe quitar algunos de los campos rastreados para poder realizar el seguimiento de nuevos campos. Para obtener más información acerca de cómo quitar campos de los campos de actualización, vea [Quitar campos de los que no se desea realizar un seguimiento](#remove-fields-you-don-t-want-tracked).

{{step-1-to-setup}}

1. En el panel de la izquierda, haz clic en **[!UICONTROL Interfaz]** y luego en **[!UICONTROL Actualizar fuentes]**.
1. (Opcional) En la pestaña **Campos rastreados**, haga clic en una de las siguientes subpestañas, según los tipos de campos que desee rastrear en la fuente de actualización:

   * **Campos integrados**: Muestra una lista de campos integrados.
   * **Campos personalizados**: Muestra una lista de campos personalizados. Debe crear los campos personalizados antes de que estén disponibles en la lista.
   * **Todos los campos**: muestra una lista de campos integrados y personalizados.

1. Haga clic en **[!UICONTROL Agregar campos]** y, a continuación, seleccione el objeto sobre el que desea realizar el seguimiento en la lista desplegable.

   La selección manual de campos no está disponible para todos los objetos que tienen un área de Actualizaciones.

   Seleccione entre los campos para los siguientes objetos:

   * Proyecto
   * Tarea
   * Problema
   * Portafolio
   * Programa
   * Usuario

   Se abre el cuadro **Agregar campos** para cada objeto seleccionado.
1. En el cuadro **Agregar campos**, empiece a escribir un campo integrado (estándar) o un campo personalizado para el objeto y, a continuación, selecciónelo cuando aparezca en la lista.

   >[!NOTE]
   >
   >Si [!DNL Workfront] ya está realizando el seguimiento del campo, no podrá agregarlo por segunda vez desde la lista.

1. Después de agregar todos los campos que desea que [!DNL Workfront] rastree, haga clic en **[!UICONTROL Agregar]**.
Los campos integrados que agregó se muestran bajo la subpestaña **[!UICONTROL Campos integrados]** y los campos personalizados se muestran bajo la subpestaña **[!UICONTROL Campos personalizados]**.
La subpestaña **[!UICONTROL Todos los campos]** muestra los campos integrados y personalizados que [!DNL Workfront] rastrea.

### Elimine los campos de los que no desea realizar un seguimiento {#remove-fields-you-don-t-want-tracked}

Puede quitar campos sobre los que no desea que el sistema realice un seguimiento para un tipo concreto de objeto en la interfaz [!DNL Workfront].

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Interfaz]** y luego en **[!UICONTROL Actualizar fuentes]**.

1. En la ficha **[!UICONTROL Campos rastreados]**, seleccione la subpestaña **[!UICONTROL Todos los campos]**. Se muestran los campos integrados y personalizados que se están rastreando actualmente.

1. Seleccione el campo cuyo seguimiento desea detener y, a continuación, haga clic en el icono **[!UICONTROL Quitar]** ![Quitar icono](assets/remove-icon.png).

1. En el cuadro **[!UICONTROL Remove Field]** que aparece, haga clic en **[!UICONTROL Yes, Remove It]** para confirmar.

   Cualquier actualización sobre los campos de los que anteriormente se ha realizado un seguimiento se conserva en el área [!UICONTROL Updates] en la que se haya registrado.

## Determinar de qué acciones [!DNL Workfront] realiza un seguimiento para un tipo de objeto

Puede hacer que [!DNL Workfront] rastree las acciones que los usuarios realizan en los objetos de la interfaz [!DNL Workfront].

Por ejemplo, puede hacer que [!DNL Workfront] registre una actualización cada vez que un usuario cambie una asignación a una tarea o problema.

El cambio aparecerá entonces como una actualización del sistema en el área [!UICONTROL Actualizaciones] de la tarea o el problema.

En la tabla siguiente se describen las acciones que se pueden realizar seguimientos en objetos de [!DNL Workfront]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Acción</strong> </th> 
   <th><strong>Objetos</strong> </th> 
   <th><strong>Estado predeterminado</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Se ha cambiado la asignación</td> 
   <td>Tareas y problemas</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Se ha eliminado la línea de base</td> 
   <td>Proyectos</td> 
   <td> <p>Deshabilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Se ha creado o eliminado el registro de facturación</td> 
   <td>Proyectos</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Se ha creado o eliminado el documento</td> 
   <td>Proyectos, tareas, problemas, portafolios y programas</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Se ha creado o eliminado el gasto</td> 
   <td>Proyectos y tareas</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Se ha registrado o eliminado la hora</td> 
   <td>Proyectos, tareas y problemas</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Se ha eliminado el problema</td> 
   <td>Proyectos</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Se ha eliminado la tarea</td> 
   <td>Proyectos</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Se cambia el acceso de alguien</td> 
   <td>Proyectos, tareas, problemas, documentos, portafolios y programas</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
  <tr> 
   <td>Suscribir objeto de comentario</td> 
   <td>Proyectos, tareas y problemas</td> 
   <td> <p>Habilitado</p> </td> 
  </tr> 
 </tbody> 
</table>

Para configurar de qué acciones desea que [!DNL Workfront] realice un seguimiento:

{{step-1-to-setup}}

1. Haga clic en **[!UICONTROL Interfaz]** y luego en **[!UICONTROL Actualizar fuentes]**.

1. Haga clic en la ficha **[!UICONTROL Actions]**.

1. Seleccione la casilla de verificación de una acción para activarla o desactívela para desactivarla.
1. Haga clic en **[!UICONTROL Guardar]**.

   Cuando deshabilita una acción, cualquier actualización registrada anteriormente sobre esa acción se conserva en el área de [!UICONTROL Actualizaciones] en la que se registró. [!DNL Workfront] deja de registrar cualquier actualización nueva para la acción deshabilitada.
