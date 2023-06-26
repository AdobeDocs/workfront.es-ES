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
source-wordcount: '1168'
ht-degree: 0%

---

# Configure las variables [!UICONTROL Listo] botón para problemas

El [!UICONTROL Listo] puede establecer automáticamente el estado de una tarea o un problema. De forma predeterminada, [!DNL Adobe Workfront] marca un problema como [!UICONTROL Resuelto] cuando un usuario asignado haga clic [!UICONTROL Listo] en su elemento de trabajo.

## Información general

Los usuarios con determinados permisos pueden configurar [!UICONTROL Listo] para reflejar ciertos estados del sistema. Existen tres formas diferentes de [!UICONTROL Listo] El botón funciona para problemas en [!DNL Workfront]:

* Si el usuario tiene un asignado [!UICONTROL Equipo de inicio], a [!DNL Workfront] o un usuario con un [!UICONTROL Plan] La licencia puede configurar el [!UICONTROL Listo] para reflejar ciertos estados de los integrantes del equipo. Consulte [Configure las variables [!UICONTROL Listo] botón para un equipo](#configure-the-uicontrol-done-button-for-a-team) en este artículo.
* Si el usuario no tiene un [!UICONTROL Equipo de inicio], pero tienen [!UICONTROL Otros equipos] en su perfil, Workfront busca la configuración del [!UICONTROL Listo] en cualquiera de los equipos asociados con el usuario. La selección es aleatoria y el estado asociado a cualquiera de los equipos se utiliza para el problema.
* Si el usuario no tiene un [!UICONTROL Equipo de inicio] asignado, el [!UICONTROL Listo] para problemas está vinculado a un problema generado por el sistema [!UICONTROL Resuelto] estado que tiene el código de tres letras [!UICONTROL RLV]. No hay opciones de configuración disponibles en este escenario. El [!UICONTROL Listo] El botón toma automáticamente este estado como valor predeterminado.
* Si la variable [!UICONTROL Resuelto] ([!UICONTROL RLV]) se elimina y el usuario marca el problema como [!UICONTROL Listo] no tiene [!UICONTROL Equipo de inicio], el estado de problema predeterminado está vinculado al que esté establecido como predeterminado para [!UICONTROL Cerrado] para el grupo asignado al proyecto al que pertenece el problema. El administrador de Workfront puede establecer una configuración predeterminada para todo el sistema para el grupo. Consulte [Configure las variables [!UICONTROL Listo] cuando el botón [!UICONTROL Resuelto] se ha eliminado el estado](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) en este artículo.

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

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Configure las variables [!UICONTROL Listo] botón para un equipo

Puede cambiar el estado que se aplica al elemento de trabajo con la variable [!UICONTROL Listo] botón. También puede establecer varios estados y permitir al usuario elegir qué estado es apropiado.

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Equipos]**.

1. Haga clic en **[!UICONTROL Cambiar equipo]** y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Haga clic en **[!UICONTROL Más]** y haga clic en **[!UICONTROL Editar]**.
1. Busque el **[!UICONTROL Botón Listo]** en la parte inferior de la **[!UICONTROL Configuración de equipo]** página.

1. Seleccione un estado o más de un estado para cada tipo de elemento de trabajo.

   >[!NOTE]
   >
   >Tenga en cuenta lo siguiente al seleccionar estados para tareas o problemas:
   >
   >* Al seleccionar un estado para cada tipo de elemento de trabajo, el estado de la tarea o del problema se establece en ese estado cuando un usuario hace clic en [!UICONTROL Listo] en su artículo. Si establece varios estados para cada tipo de elemento de trabajo, se agrega un menú desplegable al [!UICONTROL Listo] y el usuario debe elegir un estado para cambiar el estado del elemento de trabajo.
   >* Solo puede asociar estados de nivel de sistema con la variable [!UICONTROL Listo] botón. No puede asociar estados específicos de grupo con estados de elementos de trabajo.
   >* Cuando un usuario asignado al elemento coloca el elemento en el estado asociado con el [!UICONTROL Listo] botón, el elemento se muestra como [!UICONTROL Listo] para ese usuario, independientemente de si el estado seleccionado es o no [!UICONTROL Completado] o [!UICONTROL Cerrado] estado o estado de trabajo.
   >   
   >   
   >  Por ejemplo, al asociar [!UICONTROL Listo] botón con En curso hace que el elemento de trabajo se muestre como [!UICONTROL Listo] para el usuario que cambia el estado de Nuevo a En curso.
   >   
   >* Los tipos de problemas se pueden personalizar y pueden tener nombres diferentes a los que se enumeran a continuación en su entorno.\
   >  A continuación se muestran las tareas y los tipos de problemas predeterminados:
   >     
   >   * [!UICONTROL Tareas]
   >   * [!UICONTROL Problema]
   >   * [!UICONTROL Solicitud]
   >   * [!UICONTROL Solicitud de cambio]
   >   * [!UICONTROL Informe de errores]

   Si la tarea o el problema están asignados a varios usuarios, verá un &quot;[!UICONTROL Terminé mi parte]&quot; en el menú desplegable, además de los varios estados seleccionados para su equipo.

1. Clic **[!UICONTROL Guardar cambios]**.

## Asociar usuarios a un equipo de inicio

Para realizar los cambios en [!UICONTROL Listo] funcionalidad de botón visible para los usuarios, puede hacer que el equipo cuya configuración haya cambiado sea el equipo de inicio de los usuarios.

Para asociar usuarios a un equipo de inicio:

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront].

1. Clic **[!UICONTROL Usuarios]**, a continuación, seleccione el usuario o usuarios que desee asociar a un equipo de inicio.
1. Haga clic en **[!UICONTROL Más]** menú, luego seleccione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. En el **[!UICONTROL Organización]** , seleccione la **[!UICONTROL Equipo de inicio]** field. Empiece a escribir el nombre del equipo cuya configuración desea asociar con los usuarios. Haga clic en el nombre del equipo cuando lo vea en la lista.

1. Clic **[!UICONTROL Guardar cambios]**.\
   Los usuarios que ha seleccionado ahora están asociados a un equipo de inicio.
Cualquier configuración del equipo, incluidos los estados asociados con el [!UICONTROL Listo] ahora son visibles para estos usuarios.

## Configure las variables [!UICONTROL Listo] cuando el botón [!UICONTROL Resuelto] se ha eliminado el estado

Si un usuario no tiene un equipo de inicio y la opción predeterminada para todo el sistema es [!UICONTROL Resuelto] ([!UICONTROL RLV]) se ha eliminado, a [!DNL Workfront] El administrador de puede configurar [!UICONTROL Cerrado] estado del grupo en el proyecto. [!DNL Workfront] selecciona este estado para un problema cerrado cuando el usuario hace clic en [!DNL Done] botón.

### Buscar el grupo asociado con el proyecto

Cuando un usuario crea un proyecto, su grupo de inicio se asigna automáticamente al proyecto. Usuarios con [!UICONTROL Administrar] acceso al proyecto puede cambiar este grupo en el [!UICONTROL Detalles del proyecto] en cualquier momento. Para comprender qué estado se encuentra [!DNL Workfront] utiliza para un problema resuelto en este caso, debe comprender qué grupo está asociado con el proyecto en el que se encuentra el problema y cuál es el estado predeterminado de [!UICONTROL Cerrado] este grupo tiene para problemas.

Para buscar el grupo asociado al proyecto:

1. Vaya a un proyecto.
1. En la parte izquierda de la página, haga clic en **[!UICONTROL Detalles del proyecto]**.
1. Busque el **[!UICONTROL Asociación de proyecto]** y luego buscar **[!UICONTROL Grupo]**.\
   Es el nombre del grupo que debe utilizar para comprobar el estado en el área de Configuración. Consulte la siguiente sección para obtener instrucciones sobre cómo actualizar el estado predeterminado de un grupo específico.

### Actualizar el estado predeterminado de un grupo específico

As a [!UICONTROL Workfront] administrador, puede actualizar el estado de un grupo específico:

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Configurar]** ![](assets/gear-icon-settings.png).
1. En el panel izquierdo, haga clic en **[!UICONTROL Preferencias de proyecto]**, entonces **[!UICONTROL Estados]**.

1. Clic **[!UICONTROL Problemas]**, luego escriba el nombre del grupo en el **[!UICONTROL Estados del sistema]** cuadro de búsqueda situado a la derecha.

1. Seleccione el grupo.
1. Haga clic en **[!UICONTROL Establecer estados predeterminados]** menú desplegable y, a continuación, elija un estado predeterminado para [!UICONTROL Cerrado]. [!DNL Workfront] utiliza este estado para un problema cerrado cuando un usuario hace clic en [!UICONTROL Listo] botón.

   >[!IMPORTANT]
   >
   >Este estado solo se utiliza cuando el usuario no tiene asignado un equipo de inicio y el [!UICONTROL RLV] se ha eliminado el estado.

1. Haga clic en **[!UICONTROL Guardar]**.
