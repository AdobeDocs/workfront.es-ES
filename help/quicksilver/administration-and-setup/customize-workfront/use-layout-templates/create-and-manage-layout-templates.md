---
title: Creación y administración de plantillas de diseño
user-type: administrator
content-type: overview
product-area: system-administration;templates
navigation-topic: layout-templates
description: Como administrador de Workfront o de grupo, puede crear y modificar plantillas de diseño para personalizar los elementos de diseño en Workfront para los usuarios.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 53076920-3b13-4b65-85cb-38096cf2d04d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '602'
ht-degree: 0%

---

# Creación y administración de plantillas de diseño

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.
-->

Como administrador de Workfront o de grupo, puede crear y modificar plantillas de diseño para personalizar los siguientes elementos de diseño en Workfront para sus usuarios:

* Menú principal
* Panel de navegación izquierdo
* Área de inicio
* Vistas, filtros y agrupaciones que se usan con listas e informes.
* Terminología en pantalla

Después de crear o modificar una plantilla de diseño, puede asignarla a usuarios, equipos, grupos o funciones de trabajo individuales.

El diseño predeterminado de Workfront de cada usuario depende de su nivel de acceso y tipo de licencia. Por ejemplo, es posible que algunos usuarios no vean algunas áreas en el menú principal. Para obtener más información, consulte [Acerca del diseño predeterminado de Adobe Workfront](../../../administration-and-setup/customize-workfront/use-layout-templates/about-the-default-wf-layout.md).

## Requisitos de acceso

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Para realizar estos pasos a nivel de sistema, necesita el nivel de acceso del administrador del sistema.
Para realizarlos para un grupo, debe ser administrador de dicho grupo.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Consideraciones para crear y administrar plantillas de diseño

* Los usuarios pueden personalizar algunas áreas de su propio diseño. Al cambiar una plantilla de diseño, los cambios se combinan con cualquier personalización que hayan realizado, sin sobrescribirlos ni restablecerlos. Esto también ocurre si asigna usuarios a una nueva plantilla de diseño.
* Las plantillas de diseño antiguas creadas en Adobe Workfront Classic están disponibles automáticamente en la instancia de la nueva experiencia de Adobe Workfront desde que se migraron a principios de otoño de 2019. Las plantillas de diseño creadas en Adobe Workfront Classic después de esa hora se migraron en abril de 2020. Le recomendamos que actualice estas plantillas de diseño en la nueva experiencia de Adobe Workfront para aprovechar las nuevas funciones y hacerlas aún más útiles en ese entorno.
* Los administradores de grupos y usuarios con una licencia de Plan que pueden editar otros usuarios pueden agregar plantillas de diseño de nivel de sistema y de grupo a los usuarios que pueden administrar cuando editen su perfil.
* Los administradores de grupos no pueden asignar plantillas de diseño a roles de trabajo o equipos.

Para obtener más información sobre las plantillas de diseño, consulte [Plantillas de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/use-layout-templates-customize-ui.md).

## Creación o modificación de una plantilla de diseño

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Interfaz** > **Plantillas de diseño**.

1. Haga clic en **Nueva plantilla de diseño**.

   O

   Haga clic en el nombre de la plantilla de diseño que desee modificar.

1. Si está creando una nueva plantilla de diseño, escriba una **Nombre de la plantilla de diseño** y (opcional) a **Descripción** para ello.

1. Personalice áreas de la interfaz de usuario, tal como se describe en los siguientes artículos:

   * [Personalización del menú principal mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md)
   * [Personalización del panel izquierdo mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-left-panel.md)
   * [Personalización de páginas ancladas mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-pinned-pages.md)
   * [Personalización de la vista Detalles mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)
   * [Personalizar inicio y resumen mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-home-summary-layout-template.md)
   * [Personalización de la página de aterrizaje mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-landing-page.md)
   * [Personalización de filtros, vistas y grupos mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md)
   * [Personalización de la terminología de la interfaz de usuario mediante una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/customize-terminology.md)

1. Continúe probando la plantilla de diseño y ponerla a disposición de los usuarios, tal como se describe en los artículos siguientes:

   * [Prueba de una nueva plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/test-a-layout-template.md)
   * [Conceder acceso administrativo a una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md)
   * [Asignar usuarios a una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md)

También puede crear una nueva plantilla de diseño copiándola y cambiando la copia. Para obtener más información, consulte [Copiar una plantilla de diseño](../../../administration-and-setup/customize-workfront/use-layout-templates/copy-a-layout-template.md).
