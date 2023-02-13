---
navigation-topic: business-case-and-scorecards
title: Aprobar un caso empresarial
description: Después de completar y enviar el caso de negocio para una solicitud de proyecto, se debe aprobar el caso de negocio. Esto depende del flujo de trabajo de su organización. Un proyecto puede iniciarse sin que sea necesario aprobar el caso empresarial, pero es posible que el administrador de Adobe Workfront y los propietarios del proyecto no consideren ideal hacerlo.
author: Alina
feature: Work Management
exl-id: 60abb054-5cb0-4dd6-9091-c9dcd635a630
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '733'
ht-degree: 0%

---

# Aprobar un caso empresarial

Después de completar y enviar el caso de negocio para una solicitud de proyecto, se debe aprobar el caso de negocio. Esto depende del flujo de trabajo de su organización. Un proyecto puede iniciarse sin que sea necesario aprobar el caso empresarial, pero es posible que el administrador de Adobe Workfront y los propietarios del proyecto no consideren ideal hacerlo. 

Para obtener más información sobre cómo completar y enviar un caso de negocio, consulte el artículo [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un proyecto</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Información general sobre la aprobación de casos empresariales

Tenga en cuenta lo siguiente al aprobar un caso empresarial de un proyecto:

* Debe tener permisos de administración de un proyecto para aprobar el caso empresarial. 
* No podrá ver los proyectos que están a la espera de que se apruebe el caso empresarial en su página de inicio de aprobaciones.
* Debe ir manualmente a los proyectos individuales que necesitan la aprobación del caso empresarial para ver que están pendientes de aprobación. No hay ningún mecanismo de notificación de Workfront que avise a alguien de que debe aprobar el caso empresarial de un proyecto.
* Puede encontrar los proyectos que están a la espera de la aprobación del caso empresarial mediante la creación de un informe de proyecto o accediendo al portafolio con el que están asociados. 

   Para obtener más información sobre los Portfolio, consulte el artículo [Información general del Portfolio en Adobe Workfront](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## Aprobar el caso empresarial creando un informe de proyecto

Puede crear un informe para los proyectos para ver qué proyectos necesitan que se apruebe su caso empresarial. 

Para crear un informe para proyectos que están pendientes de aprobación de sus Casos de Negocio:

1. Cree un informe para los proyectos.

   Para obtener más información sobre la creación de informes, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. Seleccione el **Ver** del informe y, a continuación, haga clic en **Agregar columna**.

1. Comience a escribir &quot;Estado&quot; en la sección **Mostrar en esta columna** y seleccione este campo cuando aparezca en la lista.

    Esta columna muestra el estado de los proyectos.

1. Seleccione el **Filtros** del informe y, a continuación, haga clic en **Agregar una regla de filtro**.

1. Comience a escribir &quot;Estado&quot; en la sección **Mostrar sólo proyectos en los que ...** y selecciónelo cuando aparezca en la lista.
1. Select **Igual** para el modificador de filtro.
1. Empiece a escribir &quot;Solicitado&quot; en el campo disponible. 

   Esto garantiza que el informe incluya solo proyectos que estén en el estado Solicitado.

     ![requested_projects_filter.png](assets/requested-projects-filter-350x14.png)

1. (Opcional) Haga clic en **Añadir otra regla de filtro**.

   Puede agregar filtros adicionales para mostrar solo los proyectos en los que sea el Propietario del proyecto, el Patrocinador del proyecto o el Propietario del Portfolio.

   Por ejemplo, puede utilizar las siguientes instrucciones de filtro: 

   ```
   Project Sponsor ID Equals $$USER.ID
   ```

   para mostrar los proyectos donde está designado como patrocinador del proyecto

   ```
   Project Owner ID Equals $$USER.ID
   ```

   para mostrar los proyectos donde está designado como propietario del proyecto

   ```
   Project Portfolio Owner ID Equals $$USER. ID
   ```

   para mostrar dónde está designado como administrador de Portfolio. 

1. Haga clic en **Guardar y cerrar**.

   Observe que todos los proyectos del informe están en estado de **Solicitado**.

1. Haga clic en el nombre de un proyecto en el informe para abrirlo.
1. Haga clic en **Caso empresarial** en el panel izquierdo.
1. Haga clic en **Aprobar** o **Rechazar** en el área Resumen de casos comerciales para aprobar o rechazar el caso empresarial. 

   ![](assets/business-case-summary-with-rp-information--1-.png)

   El estado del proyecto se cambia a **Aprobado** si se aprueba el caso empresarial.

   El estado del proyecto se cambia a **Rechazado** si se rechaza el caso Business.

   >[!NOTE]
   >
   >No hay notificaciones que avisen al usuario que presentó la aprobación del caso empresarial si su solicitud de proyecto se aprobó o rechazó.

## Aprobar el caso empresarial accediendo a los proyectos solicitados en un portafolio

Para obtener más información sobre la revisión de proyectos solicitados, consulte el artículo [Revisar proyectos solicitados](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).
