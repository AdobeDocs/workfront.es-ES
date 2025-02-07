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
source-git-commit: 85aa6cc865bfc28498cca17e1942c146eeb8e4fc
workflow-type: tm+mt
source-wordcount: '899'
ht-degree: 93%

---

# Configurar las actualizaciones del sistema

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
   <td><p>Nuevo: [!UICONTROL Standard]</p>
   O
   <p>Actual: [!UICONTROL Plan]</p>
   </td> 
  </tr>  
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Determine en qué campos realiza un seguimiento [!DNL Workfront] para un tipo de objeto.

Puede determinar qué información rastrea [!DNL Workfront] cuando los usuarios cambian la información asociada con un tipo de objeto determinado en toda la interfaz de [!DNL Workfront]. Para ello, añada o elimine los campos en los que desea que [!DNL Workfront] realice un seguimiento para ese tipo de objeto.

>[!NOTE]
>
>* [!DNL Workfront] no puede rastrear y registrar actualizaciones acerca de campos personalizados calculados.
>* Puede personalizar la actualización del sistema para proyectos, tareas, problemas, portafolios, programas y usuarios. No puede personalizar la actualización del sistema para plantillas, documentos u hojas de horas, pero [!DNL Workfront] registra las actualizaciones del sistema para estos objetos.
>



* [Añada los campos en los que desee que  [!DNL Workfront] realice un seguimiento](#add-fields-you-want-workfront-to-track)
* [Elimine los campos de los que no desee realizar un seguimiento](#remove-fields-that-you-don-t-want-tracked)

### Añada los campos en los que desee que [!DNL Workfront] realice un seguimiento {#add-fields-you-want-workfront-to-track}

Puede añadir los campos en los que desee que [!DNL Workfront] realice un seguimiento para un tipo concreto de objeto en toda la interfaz de [!DNL Workfront]. Cuando los usuarios cambian la información de ese campo, [!DNL Workfront] registra la información sobre el cambio como una actualización del sistema en el área de [!UICONTROL Actualizaciones] del objeto.

>[!NOTE]
>
>Puede realizar un seguimiento de hasta 300 campos integrados y personalizados en las fuentes de actualización. Si realiza el seguimiento del número máximo de campos y desea realizar el seguimiento de campos adicionales que no se muestran en la subficha [!UICONTROL Todos los campos], primero debe quitar algunos de los campos rastreados para poder realizar el seguimiento de nuevos campos. Para obtener más información acerca de cómo quitar campos de los campos de actualización, consulte [Quitar campos de los que no se desea realizar un seguimiento](#remove-fields-that-you-don-t-want-tracked).

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración de engranajes](assets/gear-icon-settings.png).

1. En el panel de la izquierda, haga clic en **[!UICONTROL Interfaz]** > **[!UICONTROL Actualizar fuentes]**.

1. Haga clic en **[!UICONTROL Añadir campos]** y, a continuación, haga clic en el objeto sobre el que desea realizar el seguimiento.

1. En el cuadro **[!UICONTROL Actualizar fuentes]** que aparece, empiece a escribir un campo integrado (estándar) o un campo personalizado para el objeto y, a continuación, haga clic en para seleccionarlo cuando aparezca en la lista.

   Si [!DNL Workfront] ya está realizando el seguimiento del campo, no podrá añadirlo por segunda vez desde la lista.

1. Después de añadir todos los campos que desea que [!DNL Workfront] rastree, haga clic en **[!UICONTROL Añadir campos]**.

   Los campos integrados que añadió se muestran bajo la subficha **[!UICONTROL Campos integrados]**.

   Los campos personalizados que añadió se muestran en la subficha **[!UICONTROL Campos personalizados]**.

   La subficha **[!UICONTROL Todos los campos]** muestra los campos integrados y personalizados de los que se está realizando un seguimiento.

### Elimine los campos de los que no desee realizar un seguimiento {#remove-fields-that-you-don-t-want-tracked}

Puede quitar campos en los que no desea que el sistema realice un seguimiento para un tipo concreto de objeto en la interfaz de [!DNL Workfront].

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración de engranajes](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]**.

1. En la ficha **[!UICONTROL Tracked Fields]**, seleccione la subpestaña **[!UICONTROL All Fields]**.

   Así se mostrarán tanto los campos integrados como los personalizados de los que se esté realizando un seguimiento.

1. Seleccione el campo cuyo seguimiento desea detener y luego haga clic en **[!UICONTROL Remove]**.

1. En el cuadro **[!UICONTROL Remove Field]** que aparece, haga clic en **[!UICONTROL Yes, Remove It]** para confirmar.

Cualquier actualización sobre los campos de los que anteriormente se ha realizado un seguimiento se conserva en el área [!UICONTROL Updates] en la que se haya registrado.

## Determinar de qué acciones [!DNL Workfront] realiza un seguimiento para un tipo de objeto

Puede hacer que [!DNL Workfront] realice un seguimiento de las siguientes acciones que los usuarios pueden realizar en objetos en toda la interfaz de [!DNL Workfront].

Por ejemplo, puede hacer que [!DNL Workfront] registre una actualización cada vez que un usuario cambie una asignación a una tarea o problema. El cambio aparecerá entonces como una actualización del sistema en el área [!UICONTROL Actualizaciones] de la tarea o el problema.

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

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront] y, a continuación, haga clic en **[!UICONTROL Configurar]** ![Icono de configuración de engranajes](assets/gear-icon-settings.png).

1. Haga clic en **[!UICONTROL Interface]** > **[!UICONTROL Update Feeds]**.

1. Haga clic en la ficha **[!UICONTROL Actions]**.

1. Seleccione una acción para habilitarla o anule la selección de una acción para deshabilitarla.
1. Haga clic en **[!UICONTROL Guardar]**.

Cuando deshabilita una acción, cualquier actualización registrada anteriormente sobre esa acción se conserva en el área de [!UICONTROL Actualizaciones] en la que se registró.
