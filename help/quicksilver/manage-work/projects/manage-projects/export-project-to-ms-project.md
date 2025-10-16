---
product-area: projects
navigation-topic: manage-projects
title: Exportar un proyecto a Microsoft Project
description: Puede exportar proyectos de Adobe Workfront a Microsoft Project.
author: Alina
feature: Work Management
exl-id: 3f0f3644-a763-4b72-a93a-85af8626b5b3
source-git-commit: 5bc7a1c00b72cfc07270cafee5bf753989b48d33
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 74%

---

# Exportar un proyecto a Microsoft Project

Puede exportar proyectos de Adobe Workfront a Microsoft Project. 

>[!IMPORTANT]
>
>* No todos los campos de Workfront se transfieren al archivo de Microsoft Project.\
>  Para obtener más información acerca de la compatibilidad de campos entre Workfront y Microsoft Project, consulte el artículo [Asignar campos de Microsoft Project a proyectos de Adobe Workfront](../../../manage-work/projects/manage-projects/map-ms-project-fields-to-workfront.md).
>* Se recomienda limitar el número de veces que se transfieren proyectos de una aplicación a otra. 
>

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Ligero o superior</p>
   <p>Revisión o superior</p>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a los proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p> Permisos de visualización o superiores para el proyecto</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Review or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p><b>NOTE</b>
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information about access to projects, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md" class="MCXref xref">Grant access to projects</a>. For information on how a Workfront administrator can change your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p> View or higher permissions to the project</p> <p>For information about project permissions, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Share a project in Adobe Workfront</a>.</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Exportar un proyecto de Workfront a Microsoft Project

Puede exportar un proyecto desde Workfront desde la página del proyecto o desde una lista de proyectos o un informe.

1. Vaya al proyecto que desee exportar y haga clic en el icono **Más** ![Menú más](assets/qs-more-menu.png) que aparece a la derecha del nombre del proyecto

   ![Más lista desplegable](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   O

   Vaya a una lista de proyectos o a un informe y seleccione un proyecto. Luego, haga clic en el icono Más ![Menú Más](assets/qs-more-menu.png) en la parte superior de la lista.

   ![Menú más expandido](assets/more-menu-expanded-in-a-list-one-project-selected-nwe.png)

1. Haga clic en **Exportar MS Project**.

   El proyecto se descarga como archivo XML en el equipo y está listo para importarse en Microsoft Project. 
