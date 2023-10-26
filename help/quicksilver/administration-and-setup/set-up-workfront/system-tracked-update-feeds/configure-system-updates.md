---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurar actualizaciones del sistema
description: Workfront genera actualizaciones automáticas del sistema en el [!UICONTROL Actualizaciones] para registrar los cambios que los usuarios realizan en el objeto. As a [!DNL Workfront] administrador, puede configurar qué campos de objeto y acciones [!DNL Workfront] rastrea para registrar las actualizaciones del sistema.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '888'
ht-degree: 7%

---

# Configurar actualizaciones del sistema

[!DNL Adobe Workfront] genera actualizaciones automáticas del sistema en el [!UICONTROL Actualizaciones] para registrar los eventos siguientes:

* Cambios que los usuarios realizan en un campo de objeto
* Acciones que los usuarios realizan en un objeto

Estas actualizaciones del sistema incluyen el siguiente tipo de información:

* El cambio que se realizó
* El nombre del usuario que realizó el cambio
* Fecha y hora del cambio

Para obtener más información sobre las actualizaciones del sistema, consulte [Actualizaciones rastreadas por el sistema](../system-tracked-update-feeds/system-tracked-update-feeds.md).

As a [!DNL Workfront] administrador, puede configurar qué campos de objeto y acciones [!DNL Workfront] rastrea para registrar las actualizaciones del sistema.

Por ejemplo, podría tener [!DNL Workfront] haga un seguimiento de todos los cambios que los usuarios realizan en los nombres de los problemas en todo el sistema. Cualquier cambio en el nombre del problema aparece como una actualización del sistema en el [!UICONTROL Actualizaciones] área.

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
   <td> <p>Debe ser un [!DNL Workfront] administrador.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo [!DNL Workfront] El administrador puede modificar su nivel de acceso. Consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Determinar qué campos [!DNL Workfront] pistas para un tipo de objeto

Puede determinar qué información desea [!DNL Workfront] registra cuándo cambian los usuarios la información asociada a un determinado tipo de objeto en todo el [!DNL Workfront] interfaz. Para ello, agregue o elimine los campos que desee [!DNL Workfront] para realizar el seguimiento de ese tipo de objeto.

>[!NOTE]
>
>* [!DNL Workfront] no puede realizar el seguimiento y registrar actualizaciones sobre campos personalizados calculados.
>* Puede personalizar la actualización del sistema para proyectos, tareas, problemas, portafolios, programas y usuarios. No puede personalizar la actualización del sistema para plantillas, documentos u hojas de horas, pero [!DNL Workfront] registra actualizaciones del sistema para estos objetos.
>



* [Agregue los campos que desee [!DNL Workfront] para realizar el seguimiento](#add-fields-you-want-workfront-to-track)
* [Elimine los campos de los que no desee realizar un seguimiento](#remove-fields-that-you-don-t-want-tracked)

### Agregue los campos que desee [!DNL Workfront] para realizar el seguimiento {#add-fields-you-want-workfront-to-track}

Puede agregar los campos que desee [!DNL Workfront] para realizar el seguimiento de un tipo concreto de objeto en el [!DNL Workfront] interfaz. Cuando los usuarios cambian la información en ese campo, [!DNL Workfront] registra información sobre el cambio como una actualización del sistema en la [!UICONTROL Actualizaciones] para el objeto.

>[!NOTE]
>
>Puede realizar un seguimiento de hasta 300 campos integrados y personalizados en las fuentes de actualización. Si realiza el seguimiento del número máximo de campos y desea rastrear campos adicionales que no se muestran en la variable [!UICONTROL Todos los campos] En la subpestaña, primero debe quitar algunos de los campos rastreados para poder rastrear nuevos campos. Para obtener más información sobre la eliminación de campos de los campos de actualización, consulte [Elimine los campos de los que no desee realizar un seguimiento](#remove-fields-that-you-don-t-want-tracked).

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. En el panel de la izquierda, haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.

1. &#x200B;Haga clic **[!UICONTROL Agregar campos]** y, a continuación, haga clic en el objeto cuyo seguimiento desea realizar.

1. En&#x200B; **[!UICONTROL Actualizar fuentes]** Cuando aparezca, empiece a escribir un campo integrado (estándar) o un campo personalizado para el objeto y, a continuación, haga clic en para seleccionarlo cuando aparezca en la lista.

   If [!DNL Workfront] ya está realizando el seguimiento del campo, no puede añadirlo por segunda vez desde la lista.

1. Después de agregar todos los campos que desee [!DNL Workfront] para rastrear, haga clic en **[!UICONTROL Agregar campos]**.

   Los campos integrados que ha agregado se muestran debajo de **[!UICONTROL Campos integrados]** subpestaña.

   Los campos personalizados que ha añadido se muestran debajo de **[!UICONTROL Campos personalizados]** subpestaña.

   El **[!UICONTROL Todos los campos]** La subpestaña muestra los campos integrados y personalizados que se están rastreando.

### Elimine los campos de los que no desee realizar un seguimiento {#remove-fields-that-you-don-t-want-tracked}

Puede eliminar campos sobre los que no desee que el sistema realice un seguimiento para un tipo concreto de objeto en todo el [!DNL Workfront] interfaz.

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.

1. En el **[!UICONTROL Campos rastreados]** , seleccione la pestaña **[!UICONTROL Todos los campos]** subpestaña.

   Esto muestra tanto los campos integrados como los personalizados de los que se está realizando un seguimiento.

1. Seleccione el campo cuyo seguimiento desee detener y, a continuación, haga clic en **[!UICONTROL Eliminar]**.

1. En el **[!UICONTROL Quitar campo]** que aparece, haga clic en **[!UICONTROL Sí, eliminarla]** para confirmar.

Cualquier actualización sobre los campos rastreados anteriormente se conserva en la variable [!UICONTROL Actualizaciones] área donde se registraron.

## Determinar qué acciones [!DNL Workfront] pistas para un tipo de objeto

Puede tener [!DNL Workfront] realizar un seguimiento de las siguientes acciones que los usuarios pueden realizar en los objetos de [!DNL Workfront] interfaz.

Por ejemplo, puede tener [!DNL Workfront] registrar una actualización cada vez que un usuario cambie una asignación a una tarea o un problema. A continuación, el cambio aparece como una actualización del sistema en la [!UICONTROL Actualizaciones] para la tarea o el problema.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Acción</strong> </th> 
   <th><strong>Objetos</strong> </th> 
   <th><strong>Estado primario</strong> </th> 
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

Para configurar las acciones que desea [!DNL Workfront] para realizar el seguimiento:

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront], luego haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Clic **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.

1. Haga clic en **[!UICONTROL Acciones]** pestaña.

1. Seleccione una acción para habilitarla o anule la selección de una acción para deshabilitarla.
1. Haga clic en **[!UICONTROL Guardar]**.

Cuando deshabilita una acción, cualquier actualización registrada anteriormente sobre esa acción se conserva en el [!UICONTROL Actualizaciones] área en la que se registró.
