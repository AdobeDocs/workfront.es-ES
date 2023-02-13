---
product-area: templates
navigation-topic: templates-navigation-topic
title: Compartir plantillas de proyecto
description: Puede compartir una plantilla con los usuarios o definir cómo se compartirán los proyectos creados a partir de una plantilla con los usuarios mediante las siguientes opciones de uso compartido a nivel de plantilla.
author: Alina
feature: Work Management
exl-id: 99c6b241-a2c9-4b6c-b605-177bbbc3f21a
source-git-commit: dd7f61fcd92a43303be356dd3209ec6da6a063dd
workflow-type: tm+mt
source-wordcount: '780'
ht-degree: 2%

---

# Compartir plantillas de proyecto

Puede compartir una plantilla con los usuarios o definir cómo se compartirán los proyectos creados a partir de una plantilla con los usuarios mediante las siguientes opciones de uso compartido a nivel de plantilla.

Al compartir un objeto en Adobe Workfront, se permite que otros usuarios vean, contribuyan o editen ese objeto.

Para obtener información sobre los permisos de Workfront, consulte [Información general sobre cómo compartir permisos en objetos](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Para obtener información sobre los permisos que puede conceder a los usuarios al compartir una plantilla, consulte [Compartir una plantilla](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Plantillas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en una plantilla</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Compartir una plantilla {#share-a-template}

Puede compartir sus plantillas con otros usuarios mediante el uso compartido de plantillas. Esta acción define quién tiene permisos para la plantilla.

>[!NOTE]
>
>Cuando designa a un usuario activo como Propietario de plantilla, ese usuario recibe automáticamente permisos de administración en la plantilla. Para obtener información sobre cómo designar a alguien como propietario de plantilla, consulte [Editar plantillas de proyecto](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

Para compartir una plantilla:

1. En el **Menú principal** icono ![](assets/main-menu-icon.png), haga clic en **Plantillas**.

1. Realice una de las siguientes acciones:\
   Haga clic en el nombre de una plantilla para abrirla y, a continuación, haga clic en la **Más** menú ![](assets/qs-more-icon-on-an-object.png), luego **Uso compartido de plantillas**.

   O

   Seleccione una plantilla de la lista, haga clic en el icono Compartir ![](assets/share-icon.png)y haga clic en **Plantilla.**

   >[!TIP]
   >
   >Puede compartir un objeto únicamente con usuarios, equipos, funciones o empresas activos.

1. En el **Acceso a plantilla** , seleccione las personas, equipos, funciones, grupos o empresas con las que desee compartir la plantilla.

   También puede hacer clic en el botón **Opciones** para que la plantilla esté disponible en todo el sistema:

1. En el menú desplegable de cada entidad con la que comparte, seleccione una de las siguientes opciones:

   * **Ver**: Los usuarios con estos permisos pueden ver la plantilla y crear un proyecto con ella, o adjuntarla a un proyecto existente.

      >[!TIP]
      >
      >El administrador de Workfront debe darle acceso de edición a los proyectos para poder crear proyectos.

   * **Administrar**: Los usuarios con estos permisos pueden editar o eliminar la plantilla.

      Para obtener información sobre la Configuración avanzada ![](assets/gear-icon-in-access-levels.png) disponible aquí, consulte la sección [Configuración avanzada para compartir plantillas](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md#template-permissions) en el artículo [Compartir una plantilla](../../../workfront-basics/grant-and-request-access-to-objects/share-a-template.md).

1. Haga clic en **Guardar**.

## Uso compartido de un proyecto desde una plantilla {#share-a-project-from-a-template}

Con la plantilla Uso compartido de proyectos, puede definir quién tiene permisos en los proyectos creados a partir de la plantilla en el nivel de plantilla.

Para compartir con los usuarios futuros proyectos creados a partir de una plantilla:

1. Realice una de las siguientes acciones:\
   Haga clic en el nombre de una plantilla para abrirla y, a continuación, haga clic en la **Más** menú ![](assets/qs-more-icon-on-an-object.png), luego **Uso compartido de plantillas**.

   ![Compartir proyecto de plantilla](assets/project-sharing-on-template-nwe-2022-350x172.png)

   O

   Seleccione una plantilla de la lista, haga clic en **Compartir** y haga clic en **Proyecto.**

1. En el **Acceso a proyectos** , seleccione las personas, equipos, funciones, grupos o empresas con las que se comparte la plantilla.

   >[!TIP]
   >
   >Puede compartir un objeto únicamente con usuarios, equipos, funciones o empresas activos.

1. En el menú desplegable de cada entidad, seleccione una de las siguientes opciones:

   * **Sin acceso**: Puede especificar qué usuarios no tendrán acceso a la plantilla.\
      Esta opción solo está disponible cuando se comparten proyectos de forma masiva desde plantillas. 
   * **Ver**: Los usuarios con estos permisos pueden ver los proyectos creados a partir de la plantilla.
   * **Contribute**: Los usuarios con estos permisos pueden contribuir a los proyectos creados a partir de la plantilla 
   * **Administrar**: Los usuarios con estos permisos pueden administrar o eliminar proyectos creados a partir de esta plantilla.

1. (Opcional) Haga clic en el **Opciones** para que los proyectos estén disponibles en todo el sistema.
1. Haga clic en **Guardar**.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h3>Overview of project sharing from other sources</h3>
<p>You may already have been assigned access to projects from other areas of Workfront. <br>You may have been assigned access to projects from the following areas: </p>
<ul>
<li>When a project is created<br>For more information about sharing projects when the project is created, see the "Access" section in <a href="../../../manage-work/projects/manage-projects/edit-projects.md" class="MCXref xref">Edit projects</a>.</li>
<li>When your Workfront administrator sets user access levels<br>For more information about setting access levels, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</li>
<li>When using the project access template</li>
</ul>
<p>When using the Template Project Sharing feature, if a user's access to a project is View, but you set the access permissions for Template Project Sharing to Manage, the user will have Manage permission for every project created using this specific template. The user will only have View permission for the other projects they are on.</p>
</div>
-->

## Compartir plantillas y proyectos de plantillas de forma masiva

Puede compartir varias plantillas, así como proyectos de varias plantillas al mismo tiempo.

>[!NOTE]
>
>Cuando selecciona varias plantillas, no puede ver quién ya tiene permisos para las plantillas individuales.

1. Vaya a una lista de plantillas.
1. Seleccione varias plantillas y haga clic en ![Compartir](assets/share-icon.png).

   ![Compartir plantillas o proyectos de forma masiva](assets/share-templates-projects-in-bulk-link-in-toolbar-nwe-2022.png)

   >[!TIP]
   >
   >Puede compartir un objeto únicamente con usuarios, equipos, funciones o empresas activos.

1. Haga clic en **Plantilla** para compartir las plantillas seleccionadas.

   O

   Haga clic en **Proyecto** para compartir los proyectos que se crearán a partir de las plantillas seleccionadas.

1. Siga compartiendo las plantillas o los proyectos, tal como se describe en las secciones siguientes de este artículo:

   * [Compartir una plantilla](#share-a-template)
   * [Uso compartido de un proyecto desde una plantilla](#share-a-project-from-a-template)
