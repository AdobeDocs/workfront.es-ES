---
title: Personalización del menú principal mediante una plantilla de diseño
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Como administrador de Adobe Workfront o de un grupo, puede utilizar una plantilla de diseño para configurar las opciones que ven los usuarios cuando abren el menú principal en Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d4f02102-0378-472f-9ebb-753502ec048b
source-git-commit: 0f96a4d941eb4595ac60302b579cff31461272a7
workflow-type: tm+mt
source-wordcount: '659'
ht-degree: 35%

---

# Personalizar el menú principal mediante una plantilla de diseño

<!--Audited: 01/2024-->

Como administrador de Adobe Workfront o de un grupo, puede utilizar una plantilla de diseño para configurar las opciones que ven los usuarios cuando abren el menú principal en Workfront.

>[!NOTE]
>
>Las opciones del menú principal que ven los usuarios dependen del tipo de licencia y de la configuración de su nivel de acceso. Es posible que algunos usuarios que usen esta plantilla de diseño no vean todas las opciones que elija aquí. Para obtener más información, vea [Cómo funcionan juntos los niveles de acceso y los permisos](../../../administration-and-setup/add-users/access-levels-and-object-permissions/how-access-levels-permissions-work-together.md) y [Acceso configurable a la funcionalidad para cada tipo de objeto](../../../administration-and-setup/add-users/access-levels-and-object-permissions/configurable-functionality-in-each-access-level-by-object-type.md).
>
>Puede ver diferentes opciones en el menú principal si su organización se ha incorporado en la experiencia unificada de Adobe Workfront. Para obtener más información, consulte [Adobe Unified Experience para Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).

Para obtener información sobre cómo crear plantillas de diseño, consulte [Crear y administrar plantillas de diseño](../use-layout-templates/create-and-manage-layout-templates.md).

Para obtener información acerca de las plantillas de diseño para grupos, consulte [Creación y modificación de las plantillas de diseño de un grupo](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

Después de configurar una plantilla de diseño, debe asignarla a usuarios para que los cambios que ha realizado sean visibles para otros. Para obtener información acerca de cómo asignar una plantilla de diseño a los usuarios, consulte [Asignar usuarios a una plantilla de diseño](../use-layout-templates/assign-users-to-layout-template.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p>
       <p>Añadir aplicaciones personalizadas al menú principal solo está disponible para organizaciones con licencia para Adobe App Builder.</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.</p>
        <p>Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Personalización del menú principal

1. Empiece a trabajar en una plantilla de diseño, tal como se describe en [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
1. Haga clic en **Establecer menú principal** en la esquina superior derecha de la plantilla.

   Se abrirá el cuadro Menú principal, donde podrá ver las áreas que se muestran actualmente en el menú principal de la plantilla, así como los elementos que están disponibles para agregar. A continuación se indican todos los elementos posibles que puede agregar:
   * Inicio

     >[!TIP]
     >
     >De forma predeterminada, el icono Inicio del menú principal muestra el área Mis actualizaciones para los usuarios con licencia de revisión (en el plan de licencia actual), a menos que tengan una plantilla de diseño asociada a su perfil que incluya el área Mis actualizaciones del menú principal, además del área de Inicio.

   * Prioridades
   * Portafolios
   * Programas
   * Proyectos
   * Informes
   * Paneles de control
   * Calendarios
   * Asignando recursos
   * Escenarios

     >[!NOTE]
     >
     >El Planificador de escenarios requiere una licencia adicional. Para obtener información sobre el Planificador de escenarios de Workfront, consulte [Información general sobre el Planificador de escenarios](../../../scenario-planner/scenario-planner-overview.md).

   * Equipos
   * Usuarios

     >[!NOTE]
     >
     >Solo los usuarios con una licencia de planificación (en el modelo de licencia actual) o los usuarios con una licencia estándar (en el nuevo modelo de licencia) pueden ver el área de usuarios ![Icono de usuarios](assets/users-icon-in-main-menu.png) en el menú principal.

   * Solicitudes
   * Hojas de horas
   * Documentos
   * Plantillas
   * Metas

     >[!NOTE]
     >
     >Las metas requieren una licencia adicional. Para obtener información sobre Workfront Goals, consulte [Información general sobre Adobe Workfront Goals](../../../workfront-goals/goal-management/wf-goals-overview.md).

   * Mis actualizaciones
   * Tableros
   * Modelos
   * Planificación

     >[!NOTE]
     >
     >Planning requiere una licencia adicional. Para obtener información acerca de Workfront Planning, consulte [Introducción a Adobe Workfront Planning](/help/quicksilver/planning/general/planning-overview.md).

   * Aplicación personalizada

     >[!NOTE]
     >
     > Las aplicaciones personalizadas deben crearse por separado antes de que estén disponibles como opciones del menú principal. Para obtener más información, consulte [Crear una aplicación personalizada para Workfront con Adobe App Builder](/help/quicksilver/app-builder/app-builder.md).

1. Realice una de las siguientes acciones:

   * Ocultar ![Ocultar icono](assets/remove-icon---x-in-circle.png) **elementos activos** que no desee mostrar
   * Mostrar ![icono Mostrar](assets/add-icon-plus-in-circle.png) **elementos disponibles** que no desea mostrar en el menú principal.
   * Arrastre ![Icono de arrastre](assets/move-icon---dots.png) **Elementos activos** para cambiar el orden de visualización en el menú principal.

1. Haga clic en **Listo**.

   También puede hacer clic en **Cancelar** en cualquier momento si desea descartar los cambios.

1. Siga personalizando la plantilla de diseño. Puede hacer clic en **Aplicar** en cualquier momento para guardar el progreso.

   O

   Si ha terminado de personalizar, haga clic en **Guardar y cerrar**.

Para obtener más información sobre las plantillas de diseño, consulte [Crear y administrar plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
