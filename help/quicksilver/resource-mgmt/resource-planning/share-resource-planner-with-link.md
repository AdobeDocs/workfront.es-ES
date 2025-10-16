---
product-area: resource-management
navigation-topic: resource-planning
title: Compartir la vista de usuario del Planificador de recursos con un vínculo
description: Adobe Workfront puede generar una URL única para la vista de usuario del planificador de recursos, que puedes incrustar en un panel de control como una página externa o abrirla por separado en una nueva pestaña del explorador. Esto resulta útil cuando se comparte la información del Planificador de recursos con usuarios que podrían no tener acceso directo al área de Recursos.
author: Lisa
feature: Resource Management
exl-id: feb2ec26-f1a6-4581-9e1d-be948a2170c3
source-git-commit: 987b6e9b5f6b1feb323906cf7c24f5024fc84663
workflow-type: tm+mt
source-wordcount: '637'
ht-degree: 95%

---

# Compartir la vista de usuario del Planificador de recursos con un vínculo

Adobe Workfront puede generar una URL única para la vista de usuario del planificador de recursos, que puedes incrustar en un panel de control como una página externa o abrirla por separado en una nueva pestaña del explorador. Esto resulta útil cuando se comparte la información del Planificador de recursos con usuarios que podrían no tener acceso directo al área de Recursos.

![Vista de usuario con vínculo](assets/rp-user-view-with-link-highlight-350x49.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td>
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a Administración de recursos, Proyectos y Usuarios</p> <p>Ver acceso a datos financieros para ver información de costes</p></td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td> <p>Ver los permisos superiores a los proyectos que desea mostrar en el planificador de recursos</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

Tenga en cuenta lo siguiente al generar la URL única para la vista de usuario del planificador de recursos:

* Solo puede obtener una URL única para la vista de usuario. La opción para generar la dirección URL no existe en las vistas de proyectos o roles.
* Puede compartir la dirección URL con otros usuarios, incluidos los usuarios con licencia de trabajar y revisar.\
  Deben tener acceso para ver a otros usuarios con el fin de visualizar la información en el Planificador de Recursos desde la URL que compartas con ellos.
* La siguiente información se guarda al compartir la dirección URL con otros usuarios:

   * El tipo de períodos de tiempo (semana, mes, trimestre).
   * Los filtros que aplique.
   * El tipo de visualización (Horas o ETP).

Para obtener una dirección URL única en la vista de usuario del Planificador de recursos y compartirla con otros usuarios:

{{step1-to-resourcing}}

1. Seleccione **Ver por usuario**.
1. (Opcional) Seleccione el período de tiempo en el que desea ver la información en el planificador de recursos. Seleccione entre las siguientes opciones:

   * Semana
   * Mes
   * Trimestre

1. (Opcional) Seleccione si desea ver la información por **ETP** u **Horas**.\
   ![Seleccionar FTE u Horas](assets/rp-hours-or-fte-in-user-view.png)

1. (Opcional) Aplique filtros al Planificador de recursos.\
   Para obtener información acerca de cómo aplicar filtros, consulte [Información sobre filtros en el Planificador de recursos](../../resource-mgmt/resource-planning/filter-resource-planner.md).

1. Haga clic en el icono **hipervínculo**.\
   ![Icono de hipervínculo y dirección URL](assets/rp-generate-url-from-link-icon.png)

1. Haga clic en **Copiar URL**.\
   Esto copia la dirección URL única del Planificador de recursos en la vista de usuario en el portapapeles.

1. (Opcional) Realice una de las siguientes acciones:

   * Pegue la dirección URL en otra aplicación para enviarla a otro usuario.\
     El usuario debe iniciar sesión en Workfront para ver el Planificador de recursos en la vista de usuario.
   * Abra una nueva pestaña o ventana del navegador y pegue el vínculo que copió, luego haga clic en Intro en tu teclado para abrir el Planificador de recursos en una nueva pestaña o ventana.
   * Haga lo siguiente:

     <!--   
     <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">   
     (NOTE:&nbsp;turn this into a numbered list)   
     </MadCap:conditionalText>   
     -->

      1. Vaya a **Informes**>**Paneles de control**>**Nuevo panel de control**>**Añadir página externa.**

      1. Pegue el vínculo que ha copiado en el portapapeles en el campo **URL**.
      1. Haga clic en **Guardar**, luego en **Guardar + Cerrar**.\
         Esto incrusta la dirección URL en el panel de control y la vista de usuario del Planificador de recursos se muestra en un panel de control independiente.

1. (Opcional) Si incrustaste la URL en un panel de control, considera añadirla a una plantilla de diseño o compartirla con otros usuarios que podrían no tener acceso al área de Gestión de Recursos.\
   Para obtener información sobre cómo añadir tableros a una plantilla de diseño, consulte [Crear y administrar plantillas de diseño](../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).\
   Para obtener información acerca de cómo compartir paneles de control, consulte [Compartir un panel de control](../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/share-dashboard.md).\
   Al ver la dirección URL compartida, los usuarios pueden ver la información con la configuración que aplicó originalmente al Planificador de recursos. Deben iniciar sesión en Workfront para ver la URL compartida.\
   ![Panel de muestra con el Planificador de recursos mostrado](assets/user-view-dashoard-from-unique-url-350x85.png)
