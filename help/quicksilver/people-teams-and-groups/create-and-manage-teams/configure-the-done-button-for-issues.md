---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configuración del botón Listo para problemas
description: El botón Listo puede establecer automáticamente el estado de una tarea o un problema. De forma predeterminada, Adobe Workfront marca un problema como Resuelto cuando un usuario asignado hace clic en Listo en su elemento de trabajo.
author: Lisa
feature: People Teams and Groups
exl-id: 2e72854a-2d49-4665-b307-b88f660b141e
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1115'
ht-degree: 0%

---

# Configure las variables [!UICONTROL Listo] botón para problemas

La variable [!UICONTROL Listo] puede establecer automáticamente el estado de una tarea o un problema. De forma predeterminada, [!DNL Adobe Workfront] marca un problema como [!UICONTROL Resuelto] cuando un usuario asignado hace clic en [!UICONTROL Listo] en su elemento de trabajo.

## Información general

Los usuarios con determinados permisos pueden configurar la variable [!UICONTROL Listo] para reflejar ciertos estados en el sistema. Hay 3 maneras diferentes de que [!UICONTROL Listo] funciona para problemas en [!DNL Workfront]:

* Si el usuario tiene una asignación [!UICONTROL Equipo principal], [!DNL Workfront] administrador o usuario con un [!UICONTROL Plan] puede configurar la [!UICONTROL Listo] para reflejar ciertos estados para los integrantes del equipo. Consulte [Configure las variables [!UICONTROL Listo] botón para un equipo](#configure-the-uicontrol-done-button-for-a-team) en este artículo.
* Si el usuario no tiene un [!UICONTROL Equipo principal] asignado, la variable [!UICONTROL Listo] para problemas está vinculado a un [!UICONTROL Resuelto] estado que tiene el código de tres letras [!UICONTROL RLV]. No hay opciones de configuración disponibles en este escenario. La variable [!UICONTROL Listo] de forma automática, el valor predeterminado es este estado.
* Si la variable [!UICONTROL Resuelto] ([!UICONTROL RLV]) y el usuario que marca el problema como [!UICONTROL Listo] no [!UICONTROL Equipo principal], el estado del problema predeterminado está vinculado a lo que esté configurado como predeterminado para [!UICONTROL Cerrado] para el grupo asignado al proyecto al que pertenece el problema. El administrador de Workfront puede configurar una configuración predeterminada de todo el sistema para el grupo. Consulte [Configure las variables [!UICONTROL Listo] cuando el [!UICONTROL Resuelto] se ha eliminado el estado](#configure-the-uicontrol-done-button-when-the-uicontrol-resolved-status-has-been-deleted) en este artículo.

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
   <td>Se requiere acceso del administrador del sistema para configurar el botón [!UICONTROL Listo] cuando se elimina el estado [!UICONTROL Resuelto]</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Configure las variables [!UICONTROL Listo] botón para un equipo

Puede cambiar qué estado se aplica al elemento de trabajo con la variable [!UICONTROL Listo] botón. También puede establecer varios estados y permitir al usuario elegir el estado que sea adecuado.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Equipos]**.

1. Haga clic en el **[!UICONTROL Cambiar equipo]** , seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Haga clic en el **[!UICONTROL Más]** a continuación, haga clic en **[!UICONTROL Editar]**.
1. Busque la **[!UICONTROL Botón Listo]** en la parte inferior del **[!UICONTROL Configuración de equipo]** página.

1. Seleccione un estado o más de un estado para cada tipo de elemento de trabajo.

   >[!NOTE]
   >
   >Tenga en cuenta lo siguiente al seleccionar estados para tareas o problemas:
   >
   >* Cuando selecciona un estado para cada tipo de elemento de trabajo, el estado de la tarea o del problema se establece en ese estado cuando un usuario hace clic en [!UICONTROL Listo] en su artículo. Si establece varios estados para cada tipo de elemento de trabajo, se agrega un menú desplegable al [!UICONTROL Listo] y el usuario debe elegir un estado para cambiar el estado en el elemento de trabajo.
   >* Solo puede asociar estados de nivel de sistema con el [!UICONTROL Listo] botón. No se pueden asociar estados específicos de grupo con estados de elementos de trabajo.
   >* Cuando un usuario asignado al elemento coloca el elemento en el estado asociado con la variable [!UICONTROL Listo] , el elemento se muestra como [!UICONTROL Listo] para ese usuario, independientemente de si el estado que seleccione es un [!UICONTROL Completado] o [!UICONTROL Cerrado] o un estado de trabajo.

   >   
   >   
   >  Por ejemplo, si asocia la variable [!UICONTROL Listo] con In Progress hace que el elemento de trabajo se muestre como [!UICONTROL Listo] para el usuario que cambia el estado de Nuevo a En curso.
   >   
   >* Los tipos de problemas se pueden personalizar y pueden tener nombres diferentes a los que se enumeran a continuación en su entorno.\
      >  A continuación se muestran las tareas predeterminadas y los tipos de problemas:
      >     
      >   * [!UICONTROL Tareas]
      >   * [!UICONTROL Problema]
      >   * [!UICONTROL Solicitud]
      >   * [!UICONTROL Solicitud de cambio]
      >   * [!UICONTROL Informe de errores]


   Si la tarea o el problema está asignado a varios usuarios, verá un[!UICONTROL Hecho con mi parte]&quot; en el menú desplegable, además de los múltiples estados elegidos para su equipo.

1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Asociar usuarios a un equipo de inicio

Para realizar los cambios en la variable [!UICONTROL Listo] funcionalidad de botones visible para los usuarios, puede hacer que el equipo cuya configuración haya cambiado el equipo principal de los usuarios.

Para asociar usuarios con un equipo de inicio:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront].

1. Haga clic en **[!UICONTROL Usuarios]** y, a continuación, seleccione el usuario o usuarios que desea asociar a un equipo de inicio.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. En el **[!UICONTROL Organización]** seleccione **[!UICONTROL Equipo principal]** campo . Empiece a escribir el nombre del equipo cuya configuración desee asociar a los usuarios. Haga clic en el nombre del equipo cuando lo vea en la lista.

1. Haga clic en **[!UICONTROL Guardar cambios]**.\
   Los usuarios seleccionados ahora están asociados a un equipo de inicio.
Cualquier configuración de equipo, incluidos los estados asociados con la variable [!UICONTROL Listo] , ahora son visibles para estos usuarios.

## Configure las variables [!UICONTROL Listo] cuando el [!UICONTROL Resuelto] se ha eliminado el estado

Si un usuario no tiene un equipo de inicio y el valor predeterminado de todo el sistema para [!UICONTROL Resuelto] ([!UICONTROL RLV]), se ha eliminado un [!DNL Workfront] el administrador puede configurar la variable [!UICONTROL Cerrado] estado del grupo en el proyecto. [!DNL Workfront] selecciona este estado para un problema cerrado cuando el usuario hace clic en el botón [!DNL Done] botón.

### Buscar el grupo asociado al proyecto

Cuando un usuario crea un proyecto, su grupo principal se asigna automáticamente al proyecto. Usuarios con [!UICONTROL Administrar] el acceso al proyecto puede cambiar este grupo en la [!UICONTROL Detalles del proyecto] en cualquier momento. Para comprender qué estado [!DNL Workfront] utiliza para un problema completado en este caso, debe comprender qué grupo está asociado con el proyecto en el que se encuentra el problema y para qué estado predeterminado [!UICONTROL Cerrado] este grupo tiene para problemas.

Para buscar el grupo asociado al proyecto:

1. Vaya a un proyecto.
1. En el lado izquierdo de la página, haga clic en **[!UICONTROL Detalles del proyecto]**.
1. Busque la variable **[!UICONTROL Asociación de proyectos]** y, a continuación, busque **[!UICONTROL Grupo]**.\
   Este es el nombre de grupo que debe usar para comprobar el estado en el área de configuración. Consulte la siguiente sección para obtener instrucciones sobre cómo actualizar el estado predeterminado de un grupo específico.

### Actualizar el estado predeterminado de un grupo específico

Como [!UICONTROL Workfront] administrador, puede actualizar el estado de un grupo específico:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Configuración]** ![](assets/gear-icon-settings.png).
1. En el panel izquierdo, haga clic en **[!UICONTROL Preferencias de proyecto]**, luego **[!UICONTROL Estados]**.

1. Haga clic en **[!UICONTROL Problemas]** y, a continuación, escriba el nombre del grupo en la **[!UICONTROL Estados del sistema]** cuadro de búsqueda situado a la derecha.

1. Seleccione el grupo.
1. Haga clic en el **[!UICONTROL Definir estados predeterminados]** menú desplegable y, a continuación, elija un estado predeterminado para [!UICONTROL Cerrado]. [!DNL Workfront] utiliza este estado para un problema cerrado cuando un usuario hace clic en el [!UICONTROL Listo] botón.

   >[!IMPORTANT]
   >
   >Este estado solo se usa cuando el usuario no tiene asignado el equipo de inicio y el [!UICONTROL RLV] se ha eliminado.

1. Haga clic en **[!UICONTROL Guardar]**.
