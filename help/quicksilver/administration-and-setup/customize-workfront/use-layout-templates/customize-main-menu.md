---
title: Personalización del menú principal mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador de Adobe Workfront o de un grupo, puede utilizar una plantilla de diseño para configurar las opciones que ven los usuarios cuando abren el menú principal en Workfront.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 4%

---

# Personalización del menú principal mediante una plantilla de diseño

Como administrador de Adobe Workfront o de un grupo, puede utilizar una plantilla de diseño para configurar las opciones que ven los usuarios cuando abren el menú principal en Workfront:

![Opciones del menú principal](assets/main-menu-with-blueprints-no-branding.png)

>[!NOTE]
>
>Las opciones del menú principal que ven los usuarios dependen del tipo de licencia y de la configuración de su nivel de acceso. Es posible que algunos usuarios que usen esta plantilla de diseño no vean todas las opciones que elija aquí. Para obtener más información, consulte [Cómo funcionan juntos los niveles de acceso y los permisos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) y [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).

Para obtener información sobre la creación de plantillas de diseño, consulte [Creación y administración de plantillas de diseño](../use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información sobre plantillas de diseño para grupos, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Después de configurar una plantilla de diseño, debe asignarla a usuarios para que los cambios que ha realizado sean visibles para otros. Para obtener información sobre cómo asignar una plantilla de diseño a los usuarios, consulte [Asignar usuarios a una plantilla de diseño](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront</strong></td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront</strong></td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso</strong></td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> <p><b>NOTA</b>: si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Personalización del menú principal

1. Empiece a trabajar en una plantilla de diseño como se describe en [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Clic **Definir menú principal** cerca de la esquina superior derecha.

   En el cuadro Menú principal que aparece, puede ver los elementos que están activos actualmente en el menú principal de la plantilla, así como los elementos que están disponibles para agregar. A continuación se indican todos los elementos posibles que se pueden agregar:

   * Página de inicio

     >[!TIP]
     >
     >De forma predeterminada, Inicio se muestra como Mis actualizaciones para los usuarios con licencia de revisión, a menos que tengan una plantilla de diseño asociada a su perfil que incluya el área Mis actualizaciones en el menú principal.

   * Portafolios
   * Programas
   * Proyectos
   * Informes
   * Paneles
   * Calendarios
   * Asignando recursos
   * Escenarios

     >[!NOTE]
     >
     >El planificador de escenarios solo está disponible en la nueva experiencia de Adobe Workfront y requiere una licencia adicional. Para obtener información sobre el Scenario Planner de Workfront, consulte [Información general del Scenario Planner](../../../scenario-planner/scenario-planner-overview.md).

   * Equipos
   * Usuarios

     >[!NOTE]
     >
     >Solo los usuarios con una licencia de planificación pueden ver usuarios ![](assets/users-icon-in-main-menu.png) en el menú principal.

   * Solicitudes
   * Plantillas de horas
   * Documentos
   * Plantillas
   * Análisis
   * Revisión
   * Metas

     >[!NOTE]
     >
     >Esto requiere una licencia adicional. Para obtener información sobre los objetivos de Workfront, consulte [Información general sobre Adobe Workfront Goals](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * Mis actualizaciones
   * Tableros 
   * Modelos

1. Realice una de las siguientes acciones:

   * Hide ![](assets/remove-icon---x-in-circle.png) **Elementos activos** que no desea mostrar.
   * Mostrar ![](assets/add-icon-plus-in-circle.png) **Elementos disponibles** que no desea mostrar en el menú principal.
   * Arrastrar ![](assets/move-icon---dots.png) **Elementos activos** para cambiar el orden de visualización en el menú principal.

1. Clic **Listo**.

   También puede hacer clic en **Cancelar** en cualquier momento si desea descartar los cambios.

1. Siga personalizando la plantilla de diseño.

   O

   Si ha terminado de personalizar, haga clic en **Guardar**.

   >[!TIP]
   >
   >Puede hacer clic en Guardar en cualquier momento para guardar el progreso y seguir modificando la plantilla más adelante.

Para obtener más información sobre las plantillas de diseño, consulte [Creación y administración de plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
