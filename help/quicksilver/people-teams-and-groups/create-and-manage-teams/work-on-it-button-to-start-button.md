---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Reemplazar el botón Trabajar en él con un botón Inicio
description: La configuración predeterminada de Adobe Workfront incluye un botón Trabajar en él para las tareas y los problemas que se muestran para los elementos a los que ha sido asignado.
author: Lisa
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

# Sustituya el [!UICONTROL Trabajar En Él] botón con un [!UICONTROL Inicio] botón

[!DNL Adobe Workfront]La configuración predeterminada de incluye un [!UICONTROL Trabajar En Él] para las tareas y los problemas que se muestran para los elementos que se le han asignado. Al hacer clic en [!UICONTROL Trabajar En Él] en los artículos asignados a usted, le indica a otros usuarios que recibió el trabajo y reconoce que trabajará en él. Sin embargo, la variable [!DNL Work On It] no actualiza la tarea o el estado del problema para indicar que el trabajo se ha iniciado.

Puede reemplazar la variable [!DNL Work On It] botón con un [!UICONTROL Inicio] para un equipo al que pertenezca. En este caso, haga clic en el botón [!UICONTROL Inicio] en lugar de [!UICONTROL Trabajar En Él], que actualiza automáticamente el estado y la variable [!UICONTROL Fecha de inicio real] del elemento de trabajo, indicando que ha empezado a trabajar. Para obtener información sobre la configuración de qué equipo puede afectar a los cambios en la variable [!UICONTROL Trabajar En Él] , consulte la sección [Configure las variables [!UICONTROL Inicio] botón](#configure-the-uicontrol-start-button) en este artículo.

>[!IMPORTANT]
>
>Al hacer clic en [!UICONTROL Inicio] cambia el estado del elemento y [!UICONTROL Fecha de inicio real]. Si otra persona ha empezado a trabajar en una tarea o problema (lo que ha cambiado el estado a [!UICONTROL En curso] y rellenan el [!UICONTROL Fecha de inicio real]), el botón del elemento se muestra como [!UICONTROL Trabajar En Él] incluso cuando a un equipo al que pertenezca se le ha reemplazado el botón por un [!UICONTROL Inicio] botón.

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
   <td> <p>Plan</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con su [!DNL Workfront] administrador.

## Configure las variables [!UICONTROL Inicio] botón

Si tiene una [!UICONTROL Plan] licencia, puede configurar la [!UICONTROL Inicio] para un equipo de [!UICONTROL Editar] ventana del equipo. A continuación se muestra cómo funciona el botón después de activarlo para un equipo:

* **El equipo está asignado a un elemento de trabajo**: Si un equipo está asignado al elemento de trabajo, los miembros de ese equipo verán la variable [!UICONTROL Inicio] y los estados configurados para ese equipo.
* **El usuario pertenece a un equipo de inicio**: Si no hay ningún equipo asignado al elemento de trabajo pero el usuario está asignado a un equipo de inicio en su perfil, el usuario verá la variable [!UICONTROL Inicio] y los estados configurados para ese equipo. Este es el escenario que recomendamos si desea que los usuarios utilicen la variable [!UICONTROL Inicio] con frecuencia.
* **El usuario está asignado a un elemento de trabajo**: Si no hay ningún equipo asignado al elemento de trabajo y ningún equipo de inicio asignado al usuario pero el usuario está asignado al elemento de trabajo, el usuario verá la variable [!UICONTROL Inicio] y los estados combinados configurados para que todos los equipos a los que están asignados.
* **El usuario no está asignado a ningún equipo:** Si no hay ningún equipo asignado al elemento de trabajo ni ningún equipo para el usuario, incluido el Equipo principal, y el elemento está asignado al usuario, el usuario parece que el [!UICONTROL Trabajar En Él] botón.

>[!NOTE]
>
>Esta función no está disponible actualmente en
>
>* La variable [!DNL Workfront] aplicación móvil
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] notificaciones por correo electrónico
>


Para configurar el botón Inicio:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Equipos]**.

1. En el **[!UICONTROL Equipos]** menú desplegable, seleccione un equipo.\
   o\
   Haga clic en **[!UICONTROL Crear equipo]**.

1. Haga clic en el **[!UICONTROL Más]** icono ![](assets/more-icon.png)y haga clic en **[!UICONTROL Editar]**.

1. Busque la **[!UICONTROL Trabajar En Él]** sección del botón cerca de la parte inferior del [!UICONTROL Editar equipos] página.
1. Seleccione el **[!UICONTROL Cambie el botón Trabajar en él a un botón Inicio para actualizar automáticamente el estado de un elemento]** en el Navegador.
1. Seleccione uno o más estados para cada tipo de elemento de trabajo. Si selecciona más de un estado, aparecerá un menú desplegable al hacer clic en [!UICONTROL Inicio] donde puede elegir el estado deseado.
1. Haga clic en **[!UICONTROL Guardar cambios]**. Los usuarios ahora ven una [!UICONTROL Iniciar tarea] o [!UICONTROL Iniciar problema] en lugar de [!UICONTROL Trabajar En Él] cuando se les asigna un elemento de trabajo.

   >[!NOTE]
   >
   >Se recomienda configurar el equipo como el equipo de inicio de un usuario para que aparezca el botón de inicio en todos los elementos de trabajo asignados. Consulte [Asociar usuarios a un equipo de inicio](#associate-users-with-a-home-team) más abajo.

## Asociar usuarios a un equipo de inicio

Para asociar usuarios con un equipo de inicio:

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de [!DNL Adobe Workfront].

1. Haga clic en **[!UICONTROL Usuarios]** y, a continuación, seleccione el usuario o usuarios que desea asociar a un equipo de inicio.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. En el **[!UICONTROL Organización]** seleccione **[!UICONTROL Equipo principal]** campo . Empiece a escribir el nombre del equipo cuya configuración desee asociar a los usuarios. Haga clic en el nombre del equipo cuando lo vea en la lista.

1. Haga clic en **[!UICONTROL Guardar cambios]**.\
   Los usuarios seleccionados ahora están asociados a un equipo de inicio.

   Cualquier configuración de equipo, incluidos los estados asociados con la variable [!UICONTROL Listo] ahora son visibles para estos usuarios.

