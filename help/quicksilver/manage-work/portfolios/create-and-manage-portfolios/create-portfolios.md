---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Crear un portafolio
description: Un Portfolio es un conjunto de proyectos que compiten por los mismos recursos, presupuesto y programación. Los proyectos de un Portfolio son lo suficientemente similares como para utilizar el mismo conjunto de recursos y medirse con el mismo cuadro de resultados.
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
source-git-commit: 2bfb6d03f3d0f792180a67ade8a704e4c899a671
workflow-type: tm+mt
source-wordcount: '668'
ht-degree: 1%

---

# Crear un portafolio

<!--Audited: 7/2024-->

Un Portfolio es un conjunto de proyectos que compiten por los mismos recursos, presupuesto y programación. Los proyectos de un Portfolio son lo suficientemente similares como para utilizar el mismo conjunto de recursos y medirse con el mismo cuadro de resultados.

Puede utilizar Portfolio para agrupar proyectos que pertenezcan a las mismas líneas de productos, divisiones, departamentos, compañías u otras unidades de negocio.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td> 
   <td> <p>Nuevo: [!UICONTROL Standard]</p>
   <p>Actual:[!UICONTROL plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de [!UICONTROL Edit] a Portfolio</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Después de crear un portafolio, tiene permisos de administración para él de forma predeterminada</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Formas de crear portafolios

Puede crear portafolios en Workfront mediante uno de los métodos siguientes:

* Cree un portafolio desde cero empezando por el área de Portfolio del menú principal. Este artículo describe cómo crear un portafolio desde cero.

* Importe un portafolio mediante kick-starts.

  Como administrador de Workfront, puede importar portafolios mediante una &quot;kick-start&quot;.

  Para obtener información acerca de cómo importar datos mediante kick-starts en Workfront, consulte [Importar datos en Adobe Workfront mediante una plantilla de Kick-Start](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

* Agregue portafolios a medida que los conecte desde un tipo de registro en Workfront Planning.

  Debe tener una nueva licencia de Workfront y una licencia adicional de Workfront Planning para Workfront Planning.

  Para obtener información sobre el acceso a Workfront Planning, consulte [Información general sobre el acceso](/help/quicksilver/planning/access/access-overview.md).

  Para obtener información acerca de cómo crear portafolios agregándolos a registros, vea la sección &quot;Crear registros al conectarlos&quot; en el artículo [Crear registros](/help/quicksilver/planning/records/create-records.md).


## Crear un portafolio

{{step1-click-main-menu}}

1. Haga clic en **[!UICONTROL Portfolio]**.
1. Haga clic en **[!UICONTROL Nuevo Portfolio]**.
1. Reemplace **[!UICONTROL Portfolio sin título]** por el nombre que desee para el portafolio.

   El nombre puede contener hasta 255 caracteres.

1. (Opcional) Haga clic en el nombre bajo **[!UICONTROL Administrador de Portfolio]** en el encabezado en la parte superior de la página para asignar un administrador diferente para el portafolio.

   ![](assets/portfolio-manager-name-350x51.jpg)

   Como creador del portafolio, se le asigna como administrador del portafolio de forma predeterminada.

1. Haga clic en **[!UICONTROL Detalles del Portfolio]** en el panel izquierdo.
1. En el área **[!UICONTROL Información general]**, cambie la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Descripción]</td> 
      <td> <p>Escriba una descripción para que el Portfolio indique lo que tiene de único. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Administrador de Portfolio]</td> 
      <td> <p>Comience a escribir el nombre de un usuario que desee indicar como administrador del portafolio y, a continuación, selecciónelo cuando aparezca en la lista. Es igual que el [!UICONTROL Propietario del Portfolio]. Es la persona que puede supervisar el trabajo definido en los proyectos del portafolio y aprobar el caso empresarial.</p> <p>Importante: Cuando designa a alguien como [!UICONTROL Administrador de Portfolio], obtiene automáticamente permisos de [!UICONTROL Administrar] para el portafolio, los programas y los proyectos del portafolio. </p> <p>Sugerencia: También puede actualizar el [!UICONTROL Portfolio Manager] en el encabezado de la parte superior de la página.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Grupo </td> 
      <td> <p>Añada el nombre de un solo grupo si este es propietario del portafolio o tiene la responsabilidad de completarlo. </p> <p>Para asegurarse de que está seleccionando el grupo correcto, pase el puntero sobre él y haga clic en el icono de [!UICONTROL information] <img src="assets/info-icon.png"> que aparece junto a él. Se muestra información de objeto sobre el grupo, como la jerarquía de grupos por encima y sus administradores.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Haga clic dentro del cuadro **[!UICONTROL Agregar formulario personalizado]** en la esquina superior derecha de la página [!UICONTROL Detalles del Portfolio] para seleccionar un formulario personalizado para el portafolio y actualizar los campos personalizados.

   >[!TIP]
   >
   >Debe tener formularios personalizados de portafolio ya creados para poder adjuntarlos a los portafolios.

1. Haga clic en **[!UICONTROL Guardar cambios]**.
1. (Opcional) Haga clic en **[!UICONTROL Programas]** en el panel izquierdo y, a continuación, en **[!UICONTROL Agregar programas]** para agregar programas al portafolio.

   Para obtener más información sobre cómo crear programas, vea [Crear un programa](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

1. (Opcional) Haga clic en **[!UICONTROL Proyectos]** en el panel izquierdo y, a continuación, en **[!UICONTROL Agregar proyectos]** para agregar proyectos al portafolio.

   Para obtener más información sobre cómo agregar proyectos a un Portfolio, vea [Agregar proyectos a un portafolio](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Deactivate a portfolio</h2>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: drafted this and moved it to their own article: delete-deactivate-portfolios)</p>
<p>When you deactivate a portfolio, you can still access it from the Portfolios area, but it no longer displays in the list of portfolios when users try to add it to a project.</p>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2">Click <strong>Portfolios</strong> .</li>
<li value="3"> <p>Click the name of the portfolio.</p> </li>
<li value="4" data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click the More menu <img src="assets/more-icon.png"> to the right of the portfolio name, then click <strong>Deactivate Portfolio</strong>.</li>
</ol>
<h2>Delete a portfolio</h2>
<ol>
<li value="1">Click the <strong>Main Menu</strong> icon <img src="assets/main-menu-icon.png"> in the upper-right corner of Adobe Workfront.</li>
<li value="2"> <p>Click <strong>Portfolios</strong> .</p> </li>
<li value="3"> <p>Select the portfolio, then click the Delete icon <img src="assets/delete.png">.</p> </li>
<li value="4"> <p>In the box that appears, click <strong>Yes, Delete It</strong> to confirm.</p> </li>
</ol>
</div>
-->
