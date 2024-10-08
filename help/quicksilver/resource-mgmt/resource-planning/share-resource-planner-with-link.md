---
product-area: resource-management
navigation-topic: resource-planning
title: Compartir la vista de usuario del Planificador de recursos con un vínculo
description: Adobe Workfront puede generar una dirección URL única para la vista de usuario del planificador de recursos, que se puede incrustar en un tablero como una página externa o abrirla por separado en una nueva pestaña del explorador. Esto resulta útil cuando se comparte la información del Planificador de recursos con usuarios que podrían no tener acceso directo al área de Recursos.
author: Lisa
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: 3c3175c347431b10aed1a6034df6c756056399b3
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 0%

---

# Compartir la vista de usuario del Planificador de recursos con un vínculo

Adobe Workfront puede generar una dirección URL única para la vista de usuario del planificador de recursos, que se puede incrustar en un tablero como una página externa o abrirla por separado en una nueva pestaña del explorador. Esto resulta útil cuando se comparte la información del Planificador de recursos con usuarios que podrían no tener acceso directo al área de Recursos.

![](assets/rp-user-view-with-link-highlight-350x49.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
    <td><p>Nuevo: Cualquiera</p>
       <p>o</p>
       <p>Actual: Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a Administración de recursos, Proyectos y Usuarios</p> <p>Ver acceso a datos financieros para ver información de costes</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver los permisos superiores a los proyectos que desea mostrar en el Planificador de recursos</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


Tenga en cuenta lo siguiente al generar la URL única para la vista de usuario del Planificador de recursos:

* Solo puede obtener una URL única para la vista de usuario. La opción para generar la dirección URL no existe en las vistas de proyectos o roles.
* Puede compartir la dirección URL con otros usuarios, incluidos los usuarios con licencia de Trabajar y Revisar.\
  Deben tener acceso para ver otros usuarios a fin de ver la información en el Planificador de recursos desde la URL que comparta con ellos.
* La siguiente información se guarda al compartir la dirección URL con otros usuarios:

   * El tipo de periodos de tiempo (semana, mes, trimestre).
   * Los filtros que aplique.
   * El tipo de visualización (Horas o ETC).

Para obtener una dirección URL única en la vista de usuario del Planificador de recursos y compartirla con otros usuarios:

{{step1-to-resourcing}}

1. Seleccione **Ver por usuario**.
1. (Opcional) Seleccione el periodo de tiempo en el que desea ver la información en el Planificador de recursos. Seleccione una de las siguientes opciones:

   * Semana
   * Mes
   * Trimestre

1. (Opcional) Seleccione si desea ver la información por **FTE** o **Horas**.\
   ![RP_hours_or_fte_in_user_view.png](assets/rp-hours-or-fte-in-user-view.png)

1. (Opcional) Aplique filtros al Planificador de recursos.\
   Para obtener información acerca de cómo aplicar filtros, vea [Información sobre filtros en el Planificador de recursos](../../resource-mgmt/resource-planning/filter-resource-planner.md) .

1. Haga clic en el icono **hipervínculo**.\
   ![RP_Storm_generate_URL_with_copy_URL_link.png](assets/rp-storm-generate-url-with-copy-url-link-350x182.png)

1. Haga clic en **Copiar URL**.\
   Esto copia la dirección URL única del Planificador de recursos en la vista de usuario en el portapapeles.

1. (Opcional) Realice una de las siguientes acciones:  

   * Pegue la dirección URL en otra aplicación para enviarla a otro usuario.\
     El usuario debe iniciar sesión en Workfront para ver el Planificador de recursos en la vista de usuario.
   * Abra una nueva pestaña o ventana del navegador, pegue el enlace que ha copiado y, a continuación, haga clic en Enter en el teclado para abrir el Planificador de recursos en una nueva pestaña o ventana.
   * Haga lo siguiente:

     <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. Ir a **Informes**>**Paneles**>**Nuevo panel**>**Agregar página externa.**

      1. Pegue el vínculo que ha copiado en el portapapeles en el campo **URL**.
      1. Haga clic en **Guardar** y luego en **Guardar + Cerrar**.\
         Esto incrustará la dirección URL en el panel y la vista de usuario del Planificador de recursos se mostrará en un panel independiente.

1. (Opcional) Si ha incrustado la dirección URL en un panel, considere la posibilidad de agregarla a una plantilla de diseño o compartirla con otros usuarios que podrían no tener acceso al área de Administración de recursos.\
   Para obtener información sobre cómo agregar tableros a una plantilla de diseño, consulte [Crear y administrar plantillas de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md) .\
   Para obtener información acerca de cómo compartir paneles, vea [Compartir un panel](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md) .\
   Al ver la dirección URL compartida, los usuarios pueden ver la información con la configuración que aplicó originalmente al Planificador de recursos. Deben iniciar sesión en Workfront para ver la URL compartida.\
   ![user_view_dashboard_from_unique_url.png](assets/user-view-dashoard-from-unique-url-350x85.png)
