---
product-area: resource-management
navigation-topic: the-workload-balancer
title: Uso compartido de Workload Balancer con un vínculo
description: Puede compartir el equilibrador de carga de trabajo con otros usuarios que podrían no tener el área de recursos disponible para ellos. Para obtener información sobre el uso del equilibrador de carga de trabajo, consulte Navegar por el equilibrador de carga de trabajo.
author: Alina
feature: Resource Management
exl-id: e2d6b1f8-bdc9-4a34-bdc3-b56f7aa2e7a5
source-git-commit: 57ca3b58f3ef39eaea82acf609135b1e5ae8e631
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---

# Uso compartido de Workload Balancer con un vínculo

Puede compartir el equilibrador de carga de trabajo con otros usuarios que podrían no tener el área de recursos disponible para ellos. Para obtener información sobre el uso del equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquier plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar, al utilizar el equilibrador de carga de trabajo en el área de recursos</p>
   <p>Trabajar, al utilizar el equilibrador de carga de trabajo de un equipo o proyecto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver o acceso superior a lo siguiente:</p> 
    <ul> 
     <li> <p>Administración de recursos</p> </li> 
     <li> <p>Proyectos</p> </li> 
     <li> <p>Tareas</p> </li> 
     <li> <p>Problemas</p> </li> 
    </ul> <p><b>NOTA</b>

Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver o permisos superiores para proyectos, tareas y problemas </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Información incluida en el equilibrador de carga de trabajo al visualizarla desde un vínculo compartido

Cuando comparte un vínculo al equilibrador de carga de trabajo con otros usuarios, se incluye la siguiente información con el vínculo compartido:

* El área Trabajo asignado del equilibrador de carga de trabajo.
* Proyecto, tarea, información de usuario. Esto incluye la información de asignación de usuarios.
* La información se muestra según el filtro seleccionado.

   >[!IMPORTANT]
   >
   >Si elimina los filtros después de compartir el vínculo, los usuarios que vean el equilibrador de carga de trabajo desde el vínculo recibirán una advertencia avisando de que se eliminaron los filtros. Ven todos los usuarios del área Trabajo asignado. Esta es la vista predeterminada para el equilibrador de carga de trabajo.

* Número de semanas seleccionadas previamente.

El usuario que ve el equilibrador de carga de trabajo desde un vínculo compartido puede acceder a las siguientes opciones para actualizarse:

* Las siguientes selecciones de línea de tiempo:

   * Hoy
   * Iconos Atrás y Adelante
   * Selección del calendario

* Iconos de día, semana y mes
* El icono Configuración
* El icono Mostrar asignaciones

   Para obtener información sobre el uso de estas opciones, consulte [Navegar por el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

* Icono Mostrar asignaciones de funciones

   Esto solo está disponible para el equilibrador de carga de trabajo de un proyecto.

El usuario que recibe el vínculo compartido no puede hacer lo siguiente en el equilibrador de carga de trabajo desde este vínculo:

* Asignar elementos de trabajo a los usuarios
* Administrar asignaciones de usuario
* Generar filtros nuevos o actualizados aplicados originalmente

## Acceso necesario para ver información en el equilibrador de carga de trabajo desde un vínculo compartido

Necesita el siguiente acceso para ver información en el equilibrador de carga de trabajo desde un vínculo compartido:

* Una licencia de Adobe Workfront válida y debe iniciar sesión en Workfront.
* Al menos Ver el acceso a la Administración de recursos en su nivel de acceso. Para obtener información sobre la concesión de acceso a Administración de recursos, consulte [Conceder acceso a la Administración de recursos](../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md).
* Ver permisos para los proyectos, tareas, problemas y usuarios que se muestran en el equilibrador de carga de trabajo.

## Compartir el equilibrador de carga de trabajo con otros usuarios desde un vínculo

1. Vaya al equilibrador de carga de trabajo

   Para obtener información sobre el acceso al equilibrador de carga de trabajo, consulte [Navegar por el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/navigate-the-workload-balancer.md).

1. (Opcional) Realice una o más de las siguientes acciones:

   * Actualice la selección del periodo de tiempo.
   * Haga clic en **Día, semana** o **Mes** para ver información diaria, semanal o mensual.

      ![](assets/month-icon-on-toolbar-selected-wb-350x226.png)

   * Aplique filtros a las áreas Trabajo sin asignar y Trabajo asignado .

      Para obtener información sobre el filtrado de información en el equilibrador de carga de trabajo, consulte [Filtrar información en el equilibrador de carga de trabajo](../../resource-mgmt/workload-balancer/filter-information-workload-balancer.md).

1. Haga clic en el **icono de vínculo** ![](assets/wb-shearable-link-icon-small.png).

   Esto añade el vínculo al portapapeles.

1. Realice una de las siguientes acciones para compartir el vínculo con otros usuarios:

   * Péguelo en un correo electrónico, un mensaje de chat o cualquier otra aplicación y compártalo con otros usuarios.
   * Añádala a una sección personalizada como página externa, añada la sección personalizada al perfil de un usuario o a una plantilla de diseño y, a continuación, comparta la plantilla de diseño con usuarios, equipos, funciones de trabajo o grupos.

      Para obtener información sobre la creación de una página externa, consulte [Incrustar una página web externa en un panel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md). Para obtener información sobre cómo agregar secciones personalizadas a una plantilla de diseño, consulte [Personalización del panel izquierdo mediante una plantilla de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md).

      >[!IMPORTANT]
      >
      >Cuando se agrega el equilibrador de carga de trabajo a la sección personalizada de un objeto, el objeto no filtra la información del equilibrador de carga de trabajo. El equilibrador de carga de trabajo muestra la información filtrada por los filtros aplicados originalmente.
