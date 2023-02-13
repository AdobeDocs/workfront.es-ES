---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurar actualizaciones del sistema
description: Workfront genera actualizaciones automáticas del sistema en el [!UICONTROL Actualizaciones] para registrar los cambios que los usuarios realizan en el objeto. Como [!DNL Workfront] administrador, puede configurar qué campos y acciones de objeto [!DNL Workfront] rastrea para registrar las actualizaciones del sistema.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: f2fb8dc29011c12645d31b0effdc7cf397fd7ddb
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 7%

---

# Configurar actualizaciones del sistema

[!DNL Adobe Workfront] genera actualizaciones automáticas del sistema en el [!UICONTROL Actualizaciones] para registrar los siguientes eventos:

* Cambios que realizan los usuarios en un campo de objeto
* Acciones que los usuarios realizan en un objeto

Estas actualizaciones del sistema incluyen el cambio realizado, el nombre del usuario que realizó el cambio y la hora y fecha del cambio.

Como [!DNL Workfront] administrador, puede configurar qué campos y acciones de objeto [!DNL Workfront] rastrea para registrar las actualizaciones del sistema.

Por ejemplo, podría haber [!DNL Workfront] realice un seguimiento de todos los cambios que los usuarios realizan en los nombres de los problemas en todo el sistema. Cualquier cambio en el nombre del problema aparece luego como una actualización del sistema en la [!UICONTROL Actualizaciones] .

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

## Determinar qué campos [!DNL Workfront] pistas para un tipo de objeto

Puede determinar qué información [!DNL Workfront] rastrea cuando los usuarios cambian información asociada a un determinado tipo de objeto en todo el [!DNL Workfront] interfaz. Para ello, agregue o quite los campos que desee [!DNL Workfront] para rastrear para ese tipo de objeto.

>[!NOTE]
>
>* [!DNL Workfront] no puede rastrear ni registrar actualizaciones sobre campos personalizados calculados.
>* Puede personalizar la actualización del sistema para proyectos, tareas, problemas, portafolios, programas y usuarios. No puede personalizar la actualización del sistema para plantillas, documentos o hojas de horas, pero [!DNL Workfront] registra las actualizaciones del sistema para estos objetos.
>




* [Añada los campos que desee [!DNL Workfront] para rastrear](#add-fields-you-want-workfront-to-track)
* [Elimine los campos que no desee rastrear](#remove-fields-that-you-don-t-want-tracked)

### Añada los campos que desee [!DNL Workfront] para rastrear {#add-fields-you-want-workfront-to-track}

Puede añadir los campos que desee [!DNL Workfront] para realizar un seguimiento de un tipo concreto de objeto en la variable [!DNL Workfront] interfaz. Cuando los usuarios cambian información en ese campo, [!DNL Workfront] registra información sobre el cambio como una actualización del sistema en la [!UICONTROL Actualizaciones] para el objeto.

>[!NOTE]
>
>Puede realizar un seguimiento de hasta 300 campos integrados y personalizados en las fuentes de actualización. Si realiza el seguimiento del número máximo de campos y desea realizar el seguimiento de campos adicionales que no se muestran en la variable [!UICONTROL Todos los campos] En la subpestaña , primero debe eliminar algunos de los campos rastreados para poder realizar el seguimiento de los nuevos campos. Para obtener más información sobre cómo quitar campos de los campos de actualización, consulte [Elimine los campos que no desee rastrear](#remove-fields-that-you-don-t-want-tracked).

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. En el panel de la izquierda, haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.

1. &#x200B; clic **[!UICONTROL Agregar campos]** y, a continuación, haga clic en el objeto que desea rastrear.

1. En el &#x200B; **[!UICONTROL Actualizar fuentes]** que aparece, empiece a escribir un campo integrado (estándar) o un campo personalizado para el objeto y, a continuación, haga clic en para seleccionarlo cuando aparezca en la lista.

   If [!DNL Workfront] ya está rastreando el campo, no puede agregarlo por segunda vez desde la lista.

1. Después de agregar todos los campos que desee [!DNL Workfront] para realizar un seguimiento, haga clic en **[!UICONTROL Agregar campos]**.

   Los campos integrados que ha agregado se muestran en la sección **[!UICONTROL Campos integrados]** subpestaña .

   Los campos personalizados que ha agregado se muestran en la sección **[!UICONTROL Campos personalizados]** subpestaña .

   La variable **[!UICONTROL Todos los campos]** la subpestaña muestra los campos integrados y los campos personalizados que se están rastreando.

### Elimine los campos que no desee rastrear {#remove-fields-that-you-don-t-want-tracked}

Puede quitar los campos que no desee que el sistema rastree para un tipo concreto de objeto en todo el [!DNL Workfront] interfaz.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.

1. En el **[!UICONTROL Campos rastreados]** , seleccione **[!UICONTROL Todos los campos]** subpestaña .

   Muestra los campos integrados y personalizados que se están rastreando actualmente.

1. Seleccione el campo cuyo seguimiento desea detener y, a continuación, haga clic en **[!UICONTROL Eliminar]**.

1. En el **[!UICONTROL Quitar campo]** que aparece, haga clic en **[!UICONTROL Sí, elimínelo]** para confirmar.

Cualquier actualización sobre los campos rastreados anteriormente se conserva en la [!UICONTROL Actualizaciones] área en la que se grabaron.

## Determinar qué acciones [!DNL Workfront] pistas para un tipo de objeto

Puede tener [!DNL Workfront] realizar el seguimiento de las siguientes acciones que los usuarios pueden realizar en los objetos en todo el [!DNL Workfront] interfaz.

Por ejemplo, puede haber [!DNL Workfront] registra una actualización cada vez que un usuario cambia una asignación a una tarea o problema. A continuación, el cambio aparece como una actualización del sistema en la variable [!UICONTROL Actualizaciones] para la tarea o el problema.

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
   <td>El registro de facturación se crea o elimina</td> 
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

Para configurar las acciones que desea [!DNL Workfront] para rastrear:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront]y haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.

1. Haga clic en el **[!UICONTROL Acciones]** pestaña .

1. Seleccione una acción para habilitarla o anule la selección de una acción para deshabilitarla.
1. Haga clic en **[!UICONTROL Guardar]**.

Cuando deshabilita una acción, cualquier actualización registrada anteriormente sobre esa acción se conserva en la variable [!UICONTROL Actualizaciones] área en la que se registró.
