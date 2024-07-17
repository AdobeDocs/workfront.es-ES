---
title: Creación y administración de plantillas de diseño
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Como administrador de Workfront o de un grupo, puede crear y modificar plantillas de diseño para personalizar los elementos de diseño en Workfront para los usuarios.
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: e896d156854c6729e5ea0a82dcbc641fbfa9415e
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 0%

---

# Creación y administración de plantillas de diseño

<!--Audited: 12/2023-->

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Como administrador de Adobe Workfront o de un grupo, puede crear y modificar plantillas de diseño para personalizar los siguientes elementos de diseño en Workfront para los usuarios:

* Menú principal
* Panel de navegación izquierdo
* Área de inicio
* Vistas, filtros y agrupaciones que se utilizan con listas e informes.
* Terminología en pantalla
* Encabezados de proyecto, tarea y problema

Después de crear o modificar una plantilla de diseño, puede asignarla a usuarios individuales, equipos, grupos o funciones de trabajo.

El diseño de Workfront predeterminado de cada usuario depende de su nivel de acceso y tipo de licencia. Por ejemplo, es posible que algunos usuarios no vean algunas áreas en el menú principal. Para obtener más información, vea [Acerca del diseño predeterminado de Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
   O
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos en el sistema, necesita el nivel de acceso de administrador del sistema.</p>
<p>Para realizarlos para un grupo, debe ser administrador de ese grupo.</p> <p><b>NOTA</b>:</p> <p>Si no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso.

Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
 </tbody> 
</table>

+++

## Consideraciones para crear y administrar plantillas de diseño

* Los usuarios pueden personalizar algunas áreas de su propio diseño. Al cambiar una plantilla de diseño, los cambios se combinan con las personalizaciones que hayan realizado, sin sobrescribirlos ni restablecerlos. Esto también se aplica si asigna usuarios a una nueva plantilla de diseño.
* Los administradores de grupos y los usuarios con una licencia de planificación que puedan editar a otros usuarios pueden añadir plantillas de diseño de nivel de sistema y de grupo a los usuarios que pueden gestionar al editar su perfil.
* Los administradores de grupo no pueden asignar plantillas de diseño a roles o equipos de trabajo.

Para obtener más información acerca de las plantillas de diseño, vea [Plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

<!--removed this from above, but keeping it for a bit, in case it will be needed - known issue around old templates still visible at time:
* Your older layout templates created in Adobe Workfront Classic have been automatically available in your instance of the new Adobe Workfront experience since they were migrated in early Fall 2019. Layout templates created in Adobe Workfront Classic after that time were migrated in April 2020. We recommend that you update these layout templates in the new Adobe Workfront experience to take advantage of new functionality and to make them even more useful in that environment.
-->

## Creación o modificación de una plantilla de diseño

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Interfaz** > **Plantillas de diseño**.

1. Haga clic en **Nueva plantilla de diseño**.

   O

   Haga clic en el nombre de la plantilla de diseño que desee modificar.

1. Si está creando una nueva plantilla de diseño, escriba un **nombre de plantilla de diseño** y (opcional) una **descripción** para ella.

1. Personalice las áreas de la interfaz de usuario, tal como se describe en los siguientes artículos:

   * [Personalizar el menú principal mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Personalizar el panel izquierdo con una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Personalizar páginas ancladas mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Personalizar la vista Detalles mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Personalizar inicio y resumen mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Personalizar la página de aterrizaje mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Personalizar filtros, vistas y agrupaciones mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Personalización de la terminología de la interfaz de usuario mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Continúe probando la plantilla de diseño y poniéndola a disposición de los usuarios, tal como se describe en los artículos siguientes:

   * [Probando una nueva plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Conceder acceso administrativo a una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Asignar usuarios a una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

>[!TIP]
>
>También puede crear una plantilla de diseño copiándola y cambiando la copia. Para obtener más información, consulte [Copiar una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).

