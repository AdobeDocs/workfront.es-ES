---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configurar el botón Listo para problemas
description: El botón Listo puede establecer automáticamente el estado de una tarea o un problema. De forma predeterminada, Adobe Workfront marca un problema como Resuelto cuando un asignado hace clic en Listo en su elemento de trabajo.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: dd47158a4c2e1b7372af6c9450b2d277d1ca8c6f
workflow-type: tm+mt
source-wordcount: '1167'
ht-degree: 96%

---

# Configurar el botón [!UICONTROL Listo] para problemas

El botón [!UICONTROL Listo] puede establecer automáticamente el estado de una tarea o un problema. De manera predeterminada, [!DNL Adobe Workfront] marca un problema como [!UICONTROL Resuelto] cuando un asignado hace clic en [!UICONTROL Listo] en su elemento de trabajo.

>[!NOTE]
>
>El botón Listo aparece como Marcar como listo en todas las áreas de Workfront.

## Información general

Los usuarios con determinados permisos pueden configurar el botón [!UICONTROL Listo] para reflejar determinados estados en el sistema. Hay tres maneras diferentes de funcionamiento del botón [!UICONTROL Listo] para los problemas en [!DNL Workfront]:

* Si el usuario tiene un [!UICONTROL Equipo de inicio] asignado, un administrador de [!DNL Workfront] o un usuario con una licencia de [!UICONTROL Plan] puede configurar el botón [!UICONTROL Listo] para reflejar determinados estados para los integrantes del equipo. Consulte [Configurar el botón [!UICONTROL Listo] para un equipo](#configure-the-uicontrol-done-button-for-a-team) en este artículo.
* Si el usuario no tiene un [!UICONTROL equipo de inicio], pero tiene [!UICONTROL otros equipos] en su perfil, Workfront busca la configuración del botón [!UICONTROL Listo] en cualquiera de los equipos asociados al usuario. La selección es aleatoria y el estado asociado a cualquiera de los equipos se utiliza para el problema.
* Si el usuario no tiene un [!UICONTROL Equipo de inicio] asignado, el botón [!UICONTROL Listo] para los problemas está vinculado a un estado [!UICONTROL Resuelto] generado por el sistema que tiene el código de tres letras [!UICONTROL RLV]. No hay opciones de configuración disponibles en este escenario. El botón [!UICONTROL Listo] adopta automáticamente este estado como valor predeterminado.
* Si se elimina el estado [!UICONTROL Resuelto] ([!UICONTROL RLV]) y el usuario que marca el problema como [!UICONTROL Listo] no tiene ningún [!UICONTROL Equipo de inicio], el estado predeterminado del problema estará vinculado al que esté establecido como predeterminado para [!UICONTROL Cerrado] para el grupo asignado al proyecto al que pertenece el problema. El administrador de Workfront puede establecer una configuración predeterminada en todo el sistema para el grupo. Consulte [Configurar el botón [!UICONTROL Listo] cuando el estado [!UICONTROL Resuelto] se haya eliminado](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) en este artículo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>paquete de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Se requiere acceso de administrador del sistema para configurar el botón Listo cuando se elimina el estado Resuelto</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar el botón [!UICONTROL Listo] para un equipo

Puede cambiar el estado aplicado al elemento de trabajo con el botón [!UICONTROL Listo]. También puede establecer varios estados y permitir al usuario elegir qué estado es apropiado.

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar de equipo]** y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Haga clic en el menú **[!UICONTROL Más]** y luego haga clic en **[!UICONTROL Editar]**.
1. Busque la sección **[!UICONTROL Botón Listo]** en la parte inferior de la página **[!UICONTROL Configuración del equipo]**.

1. Seleccione un estado o más de un estado para cada tipo de elemento de trabajo.

   >[!NOTE]
   >
   >Tenga en cuenta lo siguiente al seleccionar estados para tareas o problemas:
   >
   >* Cuando selecciona un estado para cada tipo de elemento de trabajo, el estado de la tarea o del problema se establece en ese estado cuando un usuario hace clic en [!UICONTROL Listo] en su elemento. Si establece varios estados para cada tipo de elemento de trabajo, se añade un menú desplegable al botón [!UICONTROL Listo] y el usuario debe elegir un estado para cambiar el estado del elemento de trabajo.
   >* Solo puede asociar estados de nivel de sistema con el botón [!UICONTROL Listo]. No puede asociar estados específicos de grupo a estados de elementos de trabajo.
   >* Cuando un usuario asignado al elemento coloca el elemento en el estado asociado al botón [!UICONTROL Listo], el elemento se muestra como [!UICONTROL Listo] para ese usuario, independientemente de si el estado que seleccione tiene un estado [!UICONTROL Completado] o [!UICONTROL Cerrado] o un estado de trabajo.
   >   
   >   
   >  Por ejemplo, si se asocia el botón [!UICONTROL Listo] a En curso, el elemento de trabajo se mostrará como [!UICONTROL Listo] para el usuario cuyo estado cambia de Nuevo a En curso.
   >   
   >* Los tipos de problemas se pueden personalizar y pueden tener nombres diferentes a los que se enumeran a continuación en su entorno.\
   >  A continuación se muestran las tareas y los tipos de problemas predeterminados:
   >     
   >   * [!UICONTROL Tareas]
   >   * [!UICONTROL Problema]
   >   * [!UICONTROL Solicitud]
   >   * [!UICONTROL Solicitud de cambio]
   >   * [!UICONTROL Informe de errores]

   Si la tarea o el problema están asignados a varios usuarios, verá la opción “[!UICONTROL Terminé mi parte]” en el menú desplegable, además de los múltiples estados seleccionados para su equipo.

1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Asociar usuarios a un equipo de inicio

Para que los usuarios puedan ver los cambios realizados en la funcionalidad del botón [!UICONTROL Listo], puede hacer que el equipo cuya configuración haya cambiado sea el equipo de inicio de los usuarios.

Para asociar usuarios a un equipo de inicio:

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront].

1. Haga clic en **[!UICONTROL Usuarios]** y, a continuación, seleccione el usuario o los usuarios que desee asociar con un equipo de inicio.
1. Haga clic en el menú **[!UICONTROL Más]** y luego seleccione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. En la sección **[!UICONTROL Organización]**, seleccione el campo **[!UICONTROL Equipo de inicio]**. Empiece a escribir el nombre del equipo cuya configuración desea asociar con los usuarios. Haga clic en el nombre del equipo cuando lo vea en la lista.

1. Haga clic en **[!UICONTROL Guardar cambios]**.\
   Los usuarios que ha seleccionado ahora están asociados a un equipo de inicio.
Cualquier configuración del equipo, incluidos los estados asociados con el botón [!UICONTROL Listo], ahora son visibles para estos usuarios.

## Configurar el botón [!UICONTROL Listo] cuando se haya eliminado el estado [!UICONTROL Resuelto]

Si un usuario no tiene un equipo de inicio y se ha eliminado el valor predeterminado en todo el sistema para [!UICONTROL Resuelto] ([!UICONTROL RLV]), un administrador de [!DNL Workfront] puede configurar el estado [!UICONTROL Cerrado] para el grupo en el proyecto. [!DNL Workfront] selecciona este estado para un problema cerrado cuando el usuario hace clic en el botón [!DNL Done].

### Buscar el grupo asociado al proyecto

Cuando un usuario crea un proyecto, su grupo de inicio se asigna automáticamente al proyecto. Los usuarios con acceso para [!UICONTROL Administrar] en el proyecto pueden cambiar este grupo en la sección [!UICONTROL Detalles del proyecto] en cualquier momento. Para saber qué estado usa [!DNL Workfront] para un problema completado en este caso, debe saber qué grupo está asociado al proyecto en el que está el problema y cuál es el estado predeterminado de [!UICONTROL Cerrado] que tiene este grupo para los problemas.

Para buscar el grupo asociado al proyecto:

1. Vaya a un proyecto. 
1. En el lado izquierdo de la página, haga clic en **[!UICONTROL Detalles del proyecto]**.
1. Busque la sección **[!UICONTROL Asociación del proyecto]** y, a continuación, busque **[!UICONTROL Grupo]**.\
   Es el nombre del grupo que debe utilizar para comprobar el estado en el área de Configuración. Consulte la siguiente sección para obtener instrucciones sobre cómo actualizar el estado predeterminado de un grupo específico.

### Actualizar el estado predeterminado de un grupo específico

Como administrador de [!UICONTROL Workfront], puede actualizar el estado de un grupo específico:

1. Haga clic en el icono de **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).
1. En el panel izquierdo, haga clic en **[!UICONTROL Preferencias del proyecto]** y, a continuación, en **[!UICONTROL Estados]**.

1. Haga clic en **[!UICONTROL Problemas]** y, a continuación, escriba el nombre del grupo en el cuadro de búsqueda **[!UICONTROL Estados del sistema]** situado a la derecha.

1. Seleccione el grupo.
1. Haga clic en el menú desplegable **[!UICONTROL Establecer estados predeterminados]** y, a continuación, elija un estado predeterminado para [!UICONTROL Cerrado]. [!DNL Workfront] usa este estado para un problema cerrado cuando un usuario hace clic en el botón [!UICONTROL Listo].

   >[!IMPORTANT]
   >
   >Este estado solo se usa cuando el usuario no tiene asignado un equipo de inicio y se ha eliminado el estado [!UICONTROL RLV].

1. Haga clic en **[!UICONTROL Guardar]**.
