---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Desactivación de un equipo
description: Puede desactivar los equipos que ya no utilice mientras conserva los datos históricos asociados. Los administradores de Adobe Workfront pueden reactivar un equipo en cualquier momento desde el área Equipos de la Configuración.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Desactivación de un equipo

Puede desactivar los equipos que ya no utilice mientras conserva los datos históricos asociados. [!DNL Adobe Workfront] los administradores pueden reactivar un equipo en cualquier momento desde el área Equipos de la Configuración. Si desactiva un equipo, este ya no se mostrará en las siguientes áreas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Campos Typeforward en formularios personalizados</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Cuadro de diálogo para compartir objetos</p> </li> 
     <li> <p>[!UICONTROL Perfil de usuario]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Menú desplegable Selección principal del área [!UICONTROL Equipos]</p> </li> 
     <li> <p>tipeadelante de [!UICONTROL Asscriptions]</p> </li> 
     <li> <p>Cuadro de diálogo del tablero [!UICONTROL Agregar a Kanban] en un proyecto</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Los equipos desactivados no aparecen cuando se busca un equipo, pero se seguirán mostrando en [!UICONTROL Equipo principal] y Otros equipos si el usuario fue asignado al equipo antes de la desactivación.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
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

## Desactivación de un equipo

Cualquier trabajo asignado al equipo antes de la desactivación permanece asignado. Se recomienda reasignar el trabajo antes de desactivar el equipo.

>[!TIP]
>
>Puede crear un informe para filtrar por cualquier tarea o problema en el que el equipo desactivado aún esté asignado.

Cuando se utilizan colas de solicitud, si se desactiva un equipo asignado como equipo predeterminado en una regla de enrutamiento, el equipo permanece y las solicitudes siguen enrutándose al equipo desactivado. Se recomienda actualizar las reglas de enrutamiento con equipos activos antes de desactivar el equipo.

1. Haga clic en el **[!UICONTROL Menú principal]** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **[!UICONTROL Equipos]**.
1. Haga clic en el **[!DNL Switch team]** , seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Haga clic en el **[!UICONTROL Más]** a continuación, seleccione **[!UICONTROL Editar]**.

   ![](assets/edit-team-settings-350x205.png)

1. Borre la variable **[!UICONTROL Está activo]** en el Navegador.
1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Limitaciones conocidas

Los equipos desactivados se muestran en las siguientes áreas:

* El campo Propietario de [!DNL Workfront Goals]. Esto requiere una licencia adicional para [!DNL Adobe Workfront Goals]. Para obtener más información, consulte [Introducción a [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
