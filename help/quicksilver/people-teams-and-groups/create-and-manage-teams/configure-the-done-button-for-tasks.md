---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configurar el botón Listo para las tareas
description: El botón Listo puede establecer automáticamente el estado de una tarea o un problema. De forma predeterminada, Adobe Workfront marca una tarea como Completada cuando un usuario asignado hace clic en Listo en su elemento de trabajo.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: 62db557f6347004836fac1ea37e55d557dcc6b87
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 1%

---

# Configure las variables [!UICONTROL Listo] botón para tareas

El [!UICONTROL Listo] puede establecer automáticamente el estado de una tarea o un problema. De forma predeterminada, [!UICONTROL Adobe Workfront] marca una tarea como [!UICONTROL Completado] cuando un usuario asignado haga clic en Listo en su elemento de trabajo.

## Información general

Los usuarios con determinados permisos pueden configurar [!UICONTROL Listo] para reflejar ciertos estados del sistema. Existen dos maneras diferentes de [!UICONTROL Listo] El botón funciona para tareas en [!UICONTROL Workfront]:

* Si el usuario tiene un equipo de inicio asignado, un [!DNL Workfront] o un usuario con un [!UICONTROL Plan] La licencia puede configurar el [!UICONTROL Listo] para reflejar ciertos estados de los integrantes del equipo. Consulte [Configure las variables [!UICONTROL Listo] botón para un equipo](#configure-the-uicontrol-done-button-for-a-team) en este artículo.
* Si el usuario no tiene un [!UICONTROL Equipo de inicio], pero tienen [!UICONTROL Otros equipos] en su perfil, Workfront busca la configuración del [!UICONTROL Listo] en cualquiera de los equipos asociados con el usuario. La selección es aleatoria y se utiliza el estado asociado con cualquiera de los equipos para la tarea.
* Si el usuario no tiene un equipo de inicio asignado, la variable [!UICONTROL Listo] para las tareas está vinculado a un estado completo. No hay opciones de configuración disponibles en este escenario. El [!UICONTROL Listo] El botón toma automáticamente este estado como valor predeterminado.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] plan*</strong></p></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong><p>[!DNL Adobe Workfront] licencia*</strong></p></td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador.

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
   >  Por ejemplo, al asociar [!UICONTROL Listo] botón con [!UICONTROL En curso] hace que el elemento de trabajo se muestre como [!UICONTROL Listo] para el usuario que cambia el estado de [!UICONTROL Nuevo] hasta [!UICONTROL En curso].
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

1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Asociar usuarios a un equipo de inicio

Para realizar los cambios en [!UICONTROL Listo] funcionalidad de botón visible para los usuarios, puede hacer que el equipo cuya configuración haya cambiado sea el equipo de inicio de los usuarios.

Para asociar usuarios a un equipo de inicio:

1. Haga clic en **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront].

1. Clic **[!UICONTROL Usuarios]**, a continuación, seleccione el usuario o usuarios que desee asociar a un equipo de inicio.
1. Haga clic en **[!UICONTROL Más]** menú, luego seleccione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. En el **[!UICONTROL Organización]** , seleccione la **[!UICONTROL Equipo de inicio]** field. Empiece a escribir el nombre del equipo cuya configuración desea asociar con los usuarios. Haga clic en el nombre del equipo cuando lo vea en la lista.

1. Haga clic en **[!UICONTROL Guardar cambios]**.\
   Los usuarios que ha seleccionado ahora están asociados a un equipo de inicio.
Cualquier configuración del equipo, incluidos los estados asociados con el [!UICONTROL Listo] ahora son visibles para estos usuarios.
