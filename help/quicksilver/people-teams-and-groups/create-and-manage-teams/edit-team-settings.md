---
product-area: agile-and-teams
navigation-topic: create-and-manage-teams
title: Editar configuración de equipo
description: Los administradores de Workfront y los usuarios con una licencia de planificación o de trabajo pueden editar la configuración del equipo.
author: Lisa
feature: People Teams and Groups
exl-id: b6761188-8630-446e-bc70-70fe272881ce
source-git-commit: 79da9f7ed5149ca33f6eaeac347188149f410695
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Editar configuración del equipo

Como administrador de [!DNL Adobe Workfront] o usuario con una licencia de [!UICONTROL Estándar], [!UICONTROL Plan] o [!UICONTROL Trabajo], puede editar [!UICONTROL Configuración del equipo].

Puede añadir usuarios a un equipo, definir la plantilla de diseño del equipo y definir cómo se registra el estado cuando un equipo completa los elementos de trabajo.

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
   <p>Actual: Trabajo o superior</p></td>
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar configuración del equipo

{{step1-to-team}}

1. Haga clic en el icono **[!UICONTROL Cambiar equipo]** ![Cambiar icono de equipo](assets/switch-team-icon.png) y, a continuación, seleccione un nuevo equipo en el menú desplegable o busque un equipo en la barra de búsqueda.

1. Haga clic en el menú **[!UICONTROL Más]** ![](assets/more-icon.png) y luego seleccione **[!UICONTROL Editar]**.

   Solo los miembros del equipo con licencia de [!UICONTROL Standard], [!UICONTROL Plan] o [!UICONTROL Trabajo] ven esta opción.

   Si debería tener la opción [!UICONTROL Editar] pero no la ve, pídale al administrador de Workfront que verifique que [!UICONTROL Configuración del equipo] esté visible en la plantilla de diseño para [!UICONTROL Equipo de Scrum], [!UICONTROL Equipo de Kanban] o [!UICONTROL Equipo de Waterfall].

   ![](assets/edit-team-settings.png)

1. En la configuración del equipo, puede realizar los siguientes tipos de cambios:

   * Modificación del nombre del equipo
   * Desactivar el equipo
   * Asociar el equipo a un grupo

     >[!NOTE]
     >
     >Cuando se asigna un equipo a un grupo o subgrupo, cualquier administrador de grupo de ese grupo o subgrupo puede administrar el equipo sin ser miembro de él. Los administradores del grupo pueden ir al área de Equipos desde el menú principal y hacer clic en la flecha [!UICONTROL Cambiar equipos] ![Cambiar icono del equipo](assets/switch-team-icon.png) para ver una lista de todos los equipos asignados a los grupos que administran.

     Puede asegurarse de que está asociando el grupo correcto con el equipo pasando el puntero sobre él y haciendo clic en el icono de información ![](assets/info-icon.png) que se muestra junto a él. Se muestra información de objeto sobre el grupo, como la jerarquía de grupos por encima y sus administradores.

   * Designar el propietario del equipo
   * Adición y eliminación de miembros del equipo
   * Añada una descripción del equipo
   * Aplicar una plantilla de diseño al equipo

     Para obtener más información sobre cómo aplicar una plantilla de diseño personalizada a un equipo, consulte la sección &quot;Aplicar una plantilla personalizada a un equipo&quot; en Cambiar las áreas de [!UICONTROL Mi trabajo] y [!UICONTROL Solicitudes de trabajo] con plantillas de diseño.

   * Decida si este equipo es un equipo Agile, seleccionando la opción **[!UICONTROL Este es un equipo Agile]**.

     Para obtener más información sobre los equipos Agile y cómo administrar el trabajo dentro de un equipo Agile, consulte [Crear un equipo Agile](../../agile/get-started-with-agile-in-workfront/create-an-agile-team.md).

   * Cambiar el botón [!UICONTROL Trabajar en ello] por un botón [!UICONTROL Iniciar]. Para obtener más información sobre cómo configurar el botón [!UICONTROL Iniciar], consulte [Reemplazar el botón Trabajar en ello por un botón [!UICONTROL Iniciar]](../../people-teams-and-groups/create-and-manage-teams/work-on-it-button-to-start-button.md).
   * Personalizar el botón **[!UICONTROL Listo]**. Para obtener más información sobre cómo personalizar el botón [!UICONTROL Listo], consulte:

      * [Configurar el botón [!UICONTROL Listo] para las tareas](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-tasks.md)
      * [Configurar el botón [!UICONTROL Listo] para problemas](../../people-teams-and-groups/create-and-manage-teams/configure-the-done-button-for-issues.md)

1. Haga clic en **[!UICONTROL Guardar cambios]**.
