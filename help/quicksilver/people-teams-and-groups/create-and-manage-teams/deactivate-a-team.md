---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Desactivar o eliminar un equipo
description: Puede desactivar los equipos que ya no utilice y conservar los datos históricos asociados. Los administradores de Adobe Workfront pueden reactivar un equipo en cualquier momento desde el área Equipos de la Configuración.
author: Lisa
feature: People Teams and Groups
exl-id: 634e4c0f-aa1d-4197-92e3-54f414344ac0
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '460'
ht-degree: 0%

---

# Desactivar o eliminar un equipo

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
     <li> <p>Cuadro de diálogo Agregar al panel  en un proyecto</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Los equipos desactivados no aparecen cuando buscas un equipo, pero se mostrarán en [!UICONTROL Equipo doméstico] y Otros equipos si el usuario se asignó al equipo antes de la desactivación.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td>
  </tr>
  <tr>
   <td>Configuraciones de nivel de acceso</td>
   <td><p>Para desactivar un equipo, no se requiere ninguna configuración.</p>
   <p>Para eliminar un equipo, debe ser administrador del sistema.</p></td>
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Desactivar un equipo

Cualquier trabajo asignado al equipo antes de la desactivación permanece asignado. Se recomienda reasignar el trabajo antes de desactivar el equipo.

>[!TIP]
>
>Puede crear un informe para filtrar por cualquier tarea o problema en el que el equipo desactivado aún esté asignado.

Al utilizar colas de solicitudes, si desactiva un equipo asignado como equipo por defecto en una regla de enrutamiento, el equipo permanece y las solicitudes se siguen redirigiendo al equipo desactivado. Se recomienda actualizar las reglas de enrutamiento con los equipos activos antes de desactivar el equipo.

{{step1-to-team}}

1. Haga clic en el icono **[!DNL Switch team]** y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Haga clic en el menú **[!UICONTROL Más]** y luego seleccione **[!UICONTROL Editar]**.

   ![](assets/edit-team-settings.png)

1. Desactive la casilla de verificación **[!UICONTROL Está activo]** en la configuración del equipo.
1. Haga clic en **[!UICONTROL Guardar cambios]**.

## Limitaciones conocidas de la desactivación de un equipo

Los equipos desactivados se muestran en las siguientes áreas:

* El campo Propietario en [!DNL Workfront Goals]. Esto requiere una licencia adicional para [!DNL Adobe Workfront Goals]. Para obtener más información, consulte [Introducción a [!DNL Adobe Workfront Goals]](../../workfront-goals/goal-management/getting-started-with-wf-goals.md).

## Eliminación de un equipo

Solamente un administrador del sistema puede eliminar un equipo. Si es el propietario de un equipo (pero no un administrador) y trata de eliminar un equipo, verá un mensaje de error.

Para eliminar un equipo:

{{step1-to-team}}

1. Haga clic en el icono **[!DNL Switch team]** y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.
1. Haga clic en el menú **[!UICONTROL Más]** y luego seleccione **[!UICONTROL Eliminar]**.

   ![](assets/edit-team-settings.png)

1. Haz clic en [!UICONTROL **Confirmar**] en el mensaje de confirmación para eliminar permanentemente el equipo. Los equipos eliminados no se pueden recuperar.
