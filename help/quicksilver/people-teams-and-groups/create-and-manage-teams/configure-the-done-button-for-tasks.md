---
product-area: agile-and-teams;setup
navigation-topic: create-and-manage-teams
title: Configuración del botón Listo para tareas
description: El botón Listo puede establecer automáticamente el estado de una tarea o un problema. De forma predeterminada, Adobe Workfront marca una tarea como Completada cuando un usuario asignado hace clic en Listo en su elemento de trabajo.
author: Lisa
feature: People Teams and Groups
exl-id: 55cc5562-13d5-4089-8937-f33d0cde3cac
source-git-commit: dfd5c7423b65e6065ab9c2094578443b81189abd
workflow-type: tm+mt
source-wordcount: '758'
ht-degree: 1%

---

# Configurar el botón [!UICONTROL Listo] para las tareas

El botón [!UICONTROL Listo] puede establecer automáticamente el estado de una tarea o un problema. De manera predeterminada, [!UICONTROL Adobe Workfront] marca una tarea como [!UICONTROL Completada] cuando un usuario asignado hace clic en Listo en su elemento de trabajo.

## Información general

Los usuarios con ciertos permisos pueden configurar el botón [!UICONTROL Listo] para reflejar ciertos estados en el sistema. Hay dos maneras diferentes en que el botón [!UICONTROL Listo] funciona para las tareas de [!UICONTROL Workfront]:

* Si el usuario tiene un equipo de inicio asignado, un administrador de [!DNL Workfront] o un usuario con una licencia de [!UICONTROL Plan] puede configurar el botón [!UICONTROL Listo] para reflejar ciertos estados para los integrantes del equipo. Consulte [Configurar el botón [!UICONTROL Listo] para un equipo](#configure-the-uicontrol-done-button-for-a-team) en este artículo.
* Si el usuario no tiene un [!UICONTROL equipo de inicio], pero tiene [!UICONTROL otros equipos] en su perfil, Workfront busca la configuración del botón [!UICONTROL Listo] en cualquiera de los equipos asociados con el usuario. La selección es aleatoria y se utiliza el estado asociado con cualquiera de los equipos para la tarea.
* Si el usuario no tiene un equipo de inicio asignado, el botón [!UICONTROL Listo] de las tareas estará vinculado a un estado completo. No hay opciones de configuración disponibles en este escenario. El botón [!UICONTROL Listo] toma automáticamente este estado como valor predeterminado.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

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
   >* Cuando selecciona un estado para cada tipo de elemento de trabajo, el estado de la tarea o del problema se establece en ese estado cuando un usuario hace clic en [!UICONTROL Listo] en su elemento. Si establece varios estados para cada tipo de elemento de trabajo, se agrega un menú desplegable al botón [!UICONTROL Listo] y el usuario debe elegir un estado para cambiar el estado del elemento de trabajo.
   >* Solo puede asociar estados de nivel de sistema con el botón [!UICONTROL Listo]. No puede asociar estados específicos de grupo con estados de elementos de trabajo.
   >* Cuando un usuario asignado al elemento coloca el elemento en el estado asociado con el botón [!UICONTROL Listo], el elemento se muestra como [!UICONTROL Listo] para ese usuario, independientemente de si el estado que seleccione es un estado [!UICONTROL Completado] o [!UICONTROL Cerrado] o un estado de trabajo.
   >   
   >   
   >  Por ejemplo, al asociar el botón [!UICONTROL Listo] con [!UICONTROL En curso], el elemento de trabajo se mostrará como [!UICONTROL Listo] para el usuario que cambia el estado de [!UICONTROL Nuevo] a [!UICONTROL En curso].
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
