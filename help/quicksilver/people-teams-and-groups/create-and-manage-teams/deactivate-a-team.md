---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Desactivar un equipo
description: Puede desactivar los equipos que ya no utilice y conservar los datos históricos asociados. Los administradores de Adobe Workfront pueden reactivar un equipo en cualquier momento desde el área Equipos de la Configuración.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 24bb9b5c0836196a1c6e15f828eb47bbd489ef25
workflow-type: tm+mt
source-wordcount: '338'
ht-degree: 0%

---

# Desactivar un equipo

Puede desactivar los equipos que ya no utilice y conservar los datos históricos asociados. Los administradores de [!DNL Adobe Workfront] pueden reactivar un equipo en cualquier momento desde el área Equipos en Configuración. Si desactiva un equipo, este deja de mostrarse en las siguientes áreas:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> 
    <ul> 
     <li> <p>Campos de escritura anticipada en formularios personalizados</p> </li> 
    </ul> 
    <ul> 
     <li> <p>Cuadro de diálogo Compartir para objetos</p> </li> 
     <li> <p>[!UICONTROL Perfil de usuario]*</p> </li> 
    </ul> </td> 
   <td> 
    <ul> 
     <li> <p>Menú desplegable de selección principal en el área de [!UICONTROL Teams]</p> </li> 
     <li> <p>[!UICONTROL Asignaciones] typeforward</p> </li> 
     <li> <p>Cuadro de diálogo Agregar al panel [!UICONTROL] en un proyecto</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Los equipos desactivados no aparecen cuando buscas un equipo, pero se mostrarán en [!UICONTROL Equipo doméstico] y Otros equipos si el usuario se asignó al equipo antes de la desactivación.

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

&#42;Para saber qué plan o tipo de licencia tiene, póngase en contacto con el administrador de [!DNL Workfront].

## Desactivar un equipo

Cualquier trabajo asignado al equipo antes de la desactivación permanece asignado. Se recomienda reasignar el trabajo antes de desactivar el equipo.

>[!TIP]
>
>Puede crear un informe para filtrar por cualquier tarea o problema en el que el equipo desactivado aún esté asignado.

Al utilizar colas de solicitudes, si desactiva un equipo asignado como equipo por defecto en una regla de enrutamiento, el equipo permanece y las solicitudes se siguen redirigiendo al equipo desactivado. Se recomienda actualizar las reglas de enrutamiento con los equipos activos antes de desactivar el equipo.

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y luego haga clic en **[!UICONTROL Equipos]**.
1. Haga clic en el icono **[!DNL Switch team]** y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Haga clic en el menú **[!UICONTROL Más]** y luego seleccione **[!UICONTROL Editar]**.

   ![](assets/edit-team-settings-350x205.png)

1. Desactive la casilla **[!UICONTROL Está activo]**.
1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Limitaciones conocidas

Los equipos desactivados se muestran en las siguientes áreas:

* El campo Propietario en [!DNL Workfront Goals]. Esto requiere una licencia adicional para [!DNL Adobe Workfront Goals]. Para obtener más información, consulte [Introducción a [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).
