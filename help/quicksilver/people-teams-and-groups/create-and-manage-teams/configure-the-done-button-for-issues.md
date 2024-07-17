---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configurar el botón Listo para problemas
description: El botón Listo puede establecer automáticamente el estado de una tarea o un problema. De forma predeterminada, Adobe Workfront marca un problema como Resuelto cuando un usuario asignado hace clic en Listo en su elemento de trabajo.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 1f749ba9a54ce75a917e4b1e95713ac7abeaa66b
workflow-type: tm+mt
source-wordcount: '1169'
ht-degree: 1%

---

# Configurar el botón [!UICONTROL Listo] para problemas

El botón [!UICONTROL Listo] puede establecer automáticamente el estado de una tarea o un problema. De manera predeterminada, [!DNL Adobe Workfront] marca un problema como [!UICONTROL Resuelto] cuando un usuario asignado hace clic en [!UICONTROL Listo] en su elemento de trabajo.

## Información general

Los usuarios con ciertos permisos pueden configurar el botón [!UICONTROL Listo] para reflejar ciertos estados en el sistema. Hay tres maneras diferentes en que el botón [!UICONTROL Listo] funciona para los problemas en [!DNL Workfront]:

* Si el usuario tiene un [!UICONTROL Equipo de inicio] asignado, un administrador de [!DNL Workfront] o un usuario con una licencia de [!UICONTROL Plan] puede configurar el botón [!UICONTROL Listo] para reflejar ciertos estados para los integrantes del equipo. Consulte [Configurar el botón [!UICONTROL Listo] para un equipo](#configure-the-uicontrol-done-button-for-a-team) en este artículo.
* Si el usuario no tiene un [!UICONTROL equipo de inicio], pero tiene [!UICONTROL otros equipos] en su perfil, Workfront busca la configuración del botón [!UICONTROL Listo] en cualquiera de los equipos asociados con el usuario. La selección es aleatoria y el estado asociado a cualquiera de los equipos se utiliza para el problema.
* Si el usuario no tiene un [!UICONTROL Equipo de inicio] asignado, el botón [!UICONTROL Listo] para los problemas está vinculado a un estado [!UICONTROL Resuelto] generado por el sistema que tiene el código de tres letras [!UICONTROL RLV]. No hay opciones de configuración disponibles en este escenario. El botón [!UICONTROL Listo] toma automáticamente este estado como valor predeterminado.
* Si se elimina el estado [!UICONTROL Resuelto] ([!UICONTROL RLV]) y el usuario que marca el problema como [!UICONTROL Listo] no tiene [!UICONTROL Equipo de inicio], el estado predeterminado del problema estará vinculado al que esté establecido como predeterminado para [!UICONTROL Cerrado] para el grupo asignado al proyecto al que pertenece el problema. El administrador de Workfront puede establecer una configuración predeterminada para todo el sistema para el grupo. Ver [Configurar el botón [!UICONTROL Listo] cuando el estado [!UICONTROL Resuelto] se haya eliminado](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) en este artículo.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td>Se requiere acceso de administrador del sistema para configurar el botón [!UICONTROL Listo] cuando se elimina el estado [!UICONTROL Resuelto]</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Configurar el botón [!UICONTROL Listo] para un equipo

Puede cambiar el estado aplicado al elemento de trabajo con el botón [!UICONTROL Listo]. También puede establecer varios estados y permitir al usuario elegir qué estado es apropiado.

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y luego haga clic en **[!UICONTROL Equipos]**.

1. Haga clic en el icono **[!UICONTROL Cambiar de equipo]** y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Haga clic en el menú **[!UICONTROL Más]** y luego haga clic en **[!UICONTROL Editar]**.
1. Busque la sección **[!UICONTROL Botón Listo]** en la parte inferior de la página **[!UICONTROL Configuración del equipo]**.

1. Seleccione un estado o más de un estado para cada tipo de elemento de trabajo.

   >[!NOTE]
   >
   >Tenga en cuenta lo siguiente al seleccionar estados para tareas o problemas:
   >
   >* Cuando selecciona un estado para cada tipo de elemento de trabajo, el estado de la tarea o del problema se establece en ese estado cuando un usuario hace clic en [!UICONTROL Listo] en su elemento. Si establece varios estados para cada tipo de elemento de trabajo, se agrega un menú desplegable al botón [!UICONTROL Listo] y el usuario debe elegir un estado para cambiar el estado del elemento de trabajo.
   >* Solo puede asociar estados de nivel de sistema con el botón [!UICONTROL Listo]. No puede asociar estados específicos de grupo con estados de elementos de trabajo.
   >* Cuando un usuario asignado al elemento coloca el elemento en el estado asociado con el botón [!UICONTROL Listo], el elemento se muestra como [!UICONTROL Listo] para ese usuario, independientemente de si el estado que seleccione es un estado [!UICONTROL Completado] o [!UICONTROL Cerrado] o un estado de trabajo.
   >   
   >   
   >  Por ejemplo, si se asocia el botón [!UICONTROL Listo] con En curso, el elemento de trabajo se mostrará como [!UICONTROL Listo] para el usuario que cambia el estado de Nuevo a En curso.
   >   
   >* Los tipos de problemas se pueden personalizar y pueden tener nombres diferentes a los que se enumeran a continuación en su entorno.\
   >  A continuación se muestran las tareas y los tipos de problemas predeterminados:
   >     
   >   * [!UICONTROL Tareas]
   >   * [!UICONTROL Problema]
   >   * [!UICONTROL Solicitud]
   >   * [!UICONTROL Solicitud de cambio]
   >   * [!UICONTROL Informe de errores]

   Si la tarea o el problema están asignados a varios usuarios, verá la opción &quot;[!UICONTROL Listo con mi parte]&quot; en el menú desplegable, además de los múltiples estados seleccionados para su equipo.

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
Cualquier configuración del equipo, incluidos los estados asociados con el botón [!UICONTROL Listo], ahora es visible para estos usuarios.

## Configurar el botón [!UICONTROL Listo] cuando se haya eliminado el estado [!UICONTROL Resuelto]

Si un usuario no tiene un equipo de inicio y se ha eliminado el valor predeterminado en todo el sistema para [!UICONTROL Resuelto] ([!UICONTROL RLV]), un administrador de [!DNL Workfront] puede configurar el estado [!UICONTROL Cerrado] para el grupo en el proyecto. [!DNL Workfront] selecciona este estado para un problema cerrado cuando el usuario hace clic en el botón [!DNL Done].

### Buscar el grupo asociado con el proyecto

Cuando un usuario crea un proyecto, su grupo de inicio se asigna automáticamente al proyecto. Los usuarios con acceso para [!UICONTROL Administrar] en el proyecto pueden cambiar este grupo en la sección [!UICONTROL Detalles del proyecto] en cualquier momento. Para saber qué estado usa [!DNL Workfront] para un problema resuelto en este caso, debe saber en qué grupo está asociado el problema con el proyecto y cuál es el estado predeterminado de [!UICONTROL Cerrado] este grupo con problemas.

Para buscar el grupo asociado al proyecto:

1. Vaya a un proyecto.
1. En el lado izquierdo de la página, haga clic en **[!UICONTROL Detalles del proyecto]**.
1. Busque la sección **[!UICONTROL Asociación del proyecto]** y, a continuación, busque **[!UICONTROL Grupo]**.\
   Es el nombre del grupo que debe utilizar para comprobar el estado en el área de Configuración. Consulte la siguiente sección para obtener instrucciones sobre cómo actualizar el estado predeterminado de un grupo específico.

### Actualizar el estado predeterminado de un grupo específico

Como administrador de [!UICONTROL Workfront], puede actualizar el estado de un grupo específico:

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).
1. En el panel izquierdo, haga clic en **[!UICONTROL Preferencias del proyecto]** y, a continuación, en **[!UICONTROL Estados]**.

1. Haga clic en **[!UICONTROL Problemas]** y, a continuación, escriba el nombre del grupo en el cuadro de búsqueda **[!UICONTROL Estados del sistema]** situado a la derecha.

1. Seleccione el grupo.
1. Haga clic en el menú desplegable **[!UICONTROL Establecer estados predeterminados]** y, a continuación, elija un estado predeterminado para [!UICONTROL Cerrado]. [!DNL Workfront] usa este estado para un problema cerrado cuando un usuario hace clic en el botón [!UICONTROL Listo].

   >[!IMPORTANT]
   >
   >Este estado solo se usa cuando el usuario no tiene asignado un equipo de inicio y se ha eliminado el estado [!UICONTROL RLV].

1. Haga clic en **[!UICONTROL Guardar]**.
