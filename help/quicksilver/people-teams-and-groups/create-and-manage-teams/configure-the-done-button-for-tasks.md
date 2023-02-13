---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configuración del botón Listo para tareas
description: El botón Listo puede establecer automáticamente el estado de una tarea o un problema. De forma predeterminada, Adobe Workfront marca una tarea como Completada cuando un usuario asignado hace clic en Listo en su elemento de trabajo.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '700'
ht-degree: 1%

---

# Configure las variables [!UICONTROL Listo] botón para tareas

La variable [!UICONTROL Listo] puede establecer automáticamente el estado de una tarea o un problema. De forma predeterminada, [!UICONTROL Adobe Workfront] marca una tarea como [!UICONTROL Completado] cuando un usuario asignado hace clic en Listo en su elemento de trabajo.

## Información general

Los usuarios con determinados permisos pueden configurar la variable [!UICONTROL Listo] para reflejar ciertos estados en el sistema. Hay dos maneras diferentes de que [!UICONTROL Listo] funciona para tareas en [!UICONTROL Workfront]:

* Si el usuario tiene asignado un equipo de inicio, [!DNL Workfront] administrador o usuario con un [!UICONTROL Plan] puede configurar la [!UICONTROL Listo] para reflejar ciertos estados para los integrantes del equipo. Consulte [Configure las variables [!UICONTROL Listo] botón para un equipo](#configure-the-uicontrol-done-button-for-a-team) en este artículo.
* Si el usuario no tiene asignado un equipo de inicio, la variable [!UICONTROL Listo] para las tareas está vinculado a un estado completo. No hay opciones de configuración disponibles en este escenario. La variable [!UICONTROL Listo] de forma automática, el valor predeterminado es este estado.

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
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador.

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
   >  Por ejemplo, si asocia la variable [!UICONTROL Listo] botón con [!UICONTROL En curso] hace que el elemento de trabajo se muestre como [!UICONTROL Listo] para el usuario que cambia el estado de [!UICONTROL Nuevo] a [!UICONTROL En curso].
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
Cualquier configuración de equipo, incluidos los estados asociados con la variable [!UICONTROL Listo] ahora son visibles para estos usuarios.
