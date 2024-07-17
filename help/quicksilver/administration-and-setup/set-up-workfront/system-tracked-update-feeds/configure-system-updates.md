---
user-type: administrator
product-area: system-administration;setup
navigation-topic: system-tracked-update-feeds
title: Configurar actualizaciones del sistema
description: Workfront genera actualizaciones automáticas del sistema en el área [!UICONTROL Updates] de un objeto para registrar los cambios que los usuarios realizan en el objeto. Como administrador, puede configurar qué acciones y campos de objeto [!DNL Workfront] rastrea para registrar las actualizaciones del sistema. [!DNL Workfront]
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 54fc3f77-57d1-47f1-8e16-73626a6733ec
source-git-commit: c2c09486756db021b6edaf380c5a54d531ffa723
workflow-type: tm+mt
source-wordcount: '889'
ht-degree: 7%

---

# Configurar actualizaciones del sistema

[!DNL Adobe Workfront] genera actualizaciones automáticas del sistema en el área [!UICONTROL Updates] de un objeto para registrar los eventos siguientes:

* Cambios que los usuarios realizan en un campo de objeto
* Acciones que los usuarios realizan en un objeto

Estas actualizaciones del sistema incluyen el siguiente tipo de información:

* El cambio que se realizó
* El nombre del usuario que realizó el cambio
* Fecha y hora del cambio

Para obtener más información sobre las actualizaciones del sistema, consulte [Actualizaciones con seguimiento del sistema](../system-tracked-update-feeds/system-tracked-update-feeds.md).

Como administrador de [!DNL Workfront], puede configurar los campos de objeto y las acciones que [!DNL Workfront] realiza para registrar las actualizaciones del sistema.

Por ejemplo, puede hacer que [!DNL Workfront] realice un seguimiento de todos los cambios que los usuarios realizan en los nombres de los problemas en todo el sistema. Cualquier cambio de nombre de problema aparecerá como una actualización del sistema en el área [!UICONTROL Actualizaciones] del problema.

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
   <td> <p>Debe ser administrador de [!DNL Workfront].</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Determinar qué campos [!DNL Workfront] realiza un seguimiento para un tipo de objeto

Puede determinar qué información rastrea [!DNL Workfront] cuando los usuarios cambian la información asociada con un tipo de objeto determinado en toda la interfaz [!DNL Workfront]. Para ello, agregue o elimine los campos sobre los que desea que [!DNL Workfront] realice un seguimiento para ese tipo de objeto.

>[!NOTE]
>
>* [!DNL Workfront] no puede rastrear y registrar actualizaciones acerca de campos personalizados calculados.
>* Puede personalizar la actualización del sistema para proyectos, tareas, problemas, portafolios, programas y usuarios. No puede personalizar la actualización del sistema para plantillas, documentos u hojas de horas, pero [!DNL Workfront] registra las actualizaciones del sistema para estos objetos.
>



* [Agregue los campos que quiera que [!DNL Workfront] rastreen](#add-fields-you-want-workfront-to-track)
* [Elimine los campos de los que no desee realizar un seguimiento](#remove-fields-that-you-don-t-want-tracked)

### Agregue los campos de los que desea que [!DNL Workfront] realice un seguimiento {#add-fields-you-want-workfront-to-track}

Puede agregar campos de los que desee que [!DNL Workfront] realice un seguimiento para un tipo concreto de objeto en toda la interfaz [!DNL Workfront]. Cuando los usuarios cambian la información en ese campo, [!DNL Workfront] registra la información sobre el cambio como una actualización del sistema en el área de [!UICONTROL Actualizaciones] para el objeto.

>[!NOTE]
>
>Puede realizar un seguimiento de hasta 300 campos integrados y personalizados en las fuentes de actualización. Si realiza el seguimiento del número máximo de campos y desea realizar el seguimiento de campos adicionales que no se muestran en la subpestaña [!UICONTROL Todos los campos], primero debe quitar algunos de los campos rastreados para poder realizar el seguimiento de nuevos campos. Para obtener más información acerca de cómo quitar campos de los campos de actualización, vea [Quitar campos de los que no se desea realizar un seguimiento](#remove-fields-that-you-don-t-want-tracked).

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. En el panel de la izquierda, haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.

1. &#x200B;Haga clic en **[!UICONTROL Agregar campos]** y, a continuación, haga clic en el objeto sobre el que desea realizar el seguimiento.

1. En el cuadro&#x200B; **[!UICONTROL Actualizar fuentes]** que aparece, empiece a escribir un campo integrado (estándar) o un campo personalizado para el objeto y, a continuación, haga clic en para seleccionarlo cuando aparezca en la lista.

   Si [!DNL Workfront] ya está realizando el seguimiento del campo, no podrá agregarlo por segunda vez desde la lista.

1. Después de agregar todos los campos que desea que [!DNL Workfront] rastree, haga clic en **[!UICONTROL Agregar campos]**.

   Los campos integrados que agregó se muestran bajo la subpestaña **[!UICONTROL Campos integrados]**.

   Los campos personalizados que agregó se muestran en la subpestaña **[!UICONTROL Campos personalizados]**.

   La subpestaña **[!UICONTROL Todos los campos]** muestra los campos integrados y personalizados de los que se está realizando un seguimiento.

### Elimine los campos de los que no desee realizar un seguimiento {#remove-fields-that-you-don-t-want-tracked}

Puede quitar campos sobre los que no desea que el sistema realice un seguimiento para un tipo concreto de objeto en la interfaz [!DNL Workfront].

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.

1. En la ficha **[!UICONTROL Campos rastreados]**, seleccione la subpestaña **[!UICONTROL Todos los campos]**.

   Esto muestra tanto los campos integrados como los personalizados de los que se está realizando un seguimiento.

1. Seleccione el campo cuyo seguimiento desea detener y luego haga clic en **[!UICONTROL Quitar]**.

1. En el cuadro **[!UICONTROL Quitar campo]** que aparece, haga clic en **[!UICONTROL Sí, eliminarlo]** para confirmar.

Cualquier actualización sobre los campos rastreados anteriormente se conserva en el área de [!UICONTROL Actualizaciones] en la que se registraron.

## Determinar qué acciones [!DNL Workfront] realiza un seguimiento para un tipo de objeto

Puede hacer que [!DNL Workfront] realice un seguimiento de las siguientes acciones que los usuarios pueden realizar en objetos a través de la interfaz [!DNL Workfront].

Por ejemplo, puede hacer que [!DNL Workfront] registre una actualización cada vez que un usuario cambie una asignación a una tarea o problema. A continuación, el cambio aparece como una actualización del sistema en el área de [!UICONTROL Actualizaciones] para la tarea o el problema.

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

Para configurar qué acciones desea que [!DNL Workfront] realice un seguimiento:

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.

1. Haga clic en la ficha **[!UICONTROL Acciones]**.

1. Seleccione una acción para habilitarla o anule la selección de una acción para deshabilitarla.
1. Haga clic en **[!UICONTROL Guardar]**.

Cuando deshabilita una acción, cualquier actualización registrada anteriormente sobre esa acción se conserva en el área de [!UICONTROL Actualizaciones] en la que se registró.
