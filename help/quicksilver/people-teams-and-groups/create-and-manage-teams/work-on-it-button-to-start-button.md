---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Reemplazar el botón Trabajar en él por un botón Inicio
description: La configuración predeterminada de Adobe Workfront incluye un botón Trabajar en él para las tareas y los problemas que se muestran para los elementos a los que se le ha asignado.
author: Courtney
feature: People Teams and Groups
exl-id: 9387c5ae-2835-4d8f-80ec-22fcd16c5b6e
source-git-commit: 4261febe4af8628508083fa18e4767e3fd3e1136
workflow-type: tm+mt
source-wordcount: '778'
ht-degree: 15%

---

# Reemplaza el botón [!UICONTROL Trabajar] por un botón [!UICONTROL Iniciar]

La configuración predeterminada de [!DNL Adobe Workfront] incluye un botón [!UICONTROL Trabajar en ello] para tareas y problemas que se muestra para elementos a los que se le ha asignado. Al hacer clic en [!UICONTROL Trabajar] en los elementos asignados a ti, indicas a otros usuarios que has recibido el trabajo y reconoces que trabajarás en él. Sin embargo, el botón [!DNL Work On It] no actualiza el estado de la tarea o del problema para indicar que el trabajo se ha iniciado.

Puede reemplazar el botón [!DNL Work On It] por un botón [!UICONTROL Inicio] para un equipo al que pertenezca. En este caso, haga clic en el botón [!UICONTROL Inicio] en lugar de [!UICONTROL Trabajar en él], que actualiza automáticamente el estado y la [!UICONTROL Fecha de inicio real] del elemento de trabajo, lo que indica que ha comenzado a trabajar. Para obtener información sobre la configuración de qué equipo podría afectar a los cambios en el botón [!UICONTROL Trabajar en él], consulta la sección [Configurar el botón [!UICONTROL Inicio]](#configure-the-uicontrol-start-button) en este artículo.

>[!IMPORTANT]
>
>Al hacer clic en el botón [!UICONTROL Inicio], cambia el estado del elemento y la [!UICONTROL Fecha de inicio real]. Si otra persona ha empezado a trabajar en una tarea o problema (que cambió el estado a [!UICONTROL En curso] y rellenó la [!UICONTROL Fecha de inicio real]), el botón del elemento se muestra como [!UICONTROL Trabajar en él] incluso cuando se ha reemplazado el botón por un botón [!UICONTROL Iniciar] en un equipo al que pertenece.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Paquete de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar el botón [!UICONTROL Inicio]

Si tienes una licencia de [!UICONTROL Plan], puedes configurar el botón [!UICONTROL Inicio] para un equipo en la ventana [!UICONTROL Editar] equipo. A continuación se indica cómo funciona el botón una vez que se ha activado para un equipo:

* **El equipo está asignado a un elemento de trabajo**: si un equipo está asignado al elemento de trabajo, los miembros de ese equipo ven el botón [!UICONTROL Inicio] y los estados configurados para ese equipo.
* **El usuario pertenece a un equipo doméstico**: si no se ha asignado ningún equipo al elemento de trabajo pero el usuario está asignado a un equipo doméstico en su perfil, el usuario ve el botón [!UICONTROL Inicio] y los estados configurados para ese equipo. Este es el escenario que recomendamos si desea que los usuarios usen el botón [!UICONTROL Inicio] con frecuencia.
* **El usuario está asignado a un elemento de trabajo**: si no hay ningún equipo asignado al elemento de trabajo ni ningún equipo particular asignado al usuario, pero el usuario está asignado al elemento de trabajo, el usuario ve el botón [!UICONTROL Inicio] y los estados combinados configurados para todos los equipos a los que están asignados.
* **El usuario no está asignado a ningún equipo:** Si no hay ningún equipo asignado al elemento de trabajo ni ningún equipo para el usuario, incluido el equipo particular, y el elemento está asignado al usuario, el usuario parece tener el botón [!UICONTROL Trabajar en él].

>[!NOTE]
>
>Esta función no está disponible actualmente en
>
>* La aplicación móvil [!DNL Workfront]
>* [!DNL Workfront for Office 365]
>* [!DNL Workfront] notificaciones por correo electrónico
>

Para configurar el botón Inicio:

{{step1-to-team}}

1. En el menú desplegable **[!UICONTROL Equipos]**, selecciona un equipo.\
   o\
   Haga clic en **[!UICONTROL Crear nuevo equipo]**.

1. Haga clic en el icono **[!UICONTROL Más]** ![](assets/more-icon.png) y luego haga clic en **[!UICONTROL Editar]**.

1. Encuentra la sección del botón **[!UICONTROL Trabajar en ello]** cerca de la parte inferior de la página [!UICONTROL Editar equipos].
1. Active la casilla de verificación **[!UICONTROL Cambiar el botón Trabajar en él por un botón Inicio para actualizar automáticamente el estado de un elemento]**.
1. Seleccione uno o varios estados para cada tipo de elemento de trabajo. Si selecciona más de un estado, aparecerá un menú desplegable al hacer clic en [!UICONTROL Iniciar], donde podrá elegir el estado que desee.
1. Haga clic en **[!UICONTROL Guardar cambios]**. Los usuarios ahora ven un botón [!UICONTROL Iniciar tarea] o [!UICONTROL Iniciar problema] en lugar del botón [!UICONTROL Trabajar en ello] cuando se les asigna un elemento de trabajo.

   >[!NOTE]
   >
   >Se recomienda configurar el equipo como el equipo de inicio de un usuario para que aparezca el botón de inicio en todos los elementos de trabajo asignados. Consulte [Asociar usuarios con un equipo de inicio](#associate-users-with-a-home-team) a continuación.

## Asociar usuarios a un equipo de inicio

Para asociar usuarios a un equipo de inicio:

{{step-1-to-users}}

1. Seleccione el usuario o los usuarios que desee asociar a un equipo doméstico.
1. Haga clic en el menú **[!UICONTROL Más]** y luego seleccione **[!UICONTROL Editar]**.\
   ![](assets/user-settings-nwe-350x291.png)

1. En la sección **[!UICONTROL Organización]**, seleccione el campo **[!UICONTROL Equipo de inicio]**. Empiece a escribir el nombre del equipo cuya configuración desea asociar con los usuarios. Haga clic en el nombre del equipo cuando lo vea en la lista.

1. Haga clic en **[!UICONTROL Guardar cambios]**.\
   Los usuarios que ha seleccionado ahora están asociados a un equipo de inicio.

   Cualquier configuración del equipo, incluidos los estados asociados con el botón [!UICONTROL Listo], ahora es visible para estos usuarios.

