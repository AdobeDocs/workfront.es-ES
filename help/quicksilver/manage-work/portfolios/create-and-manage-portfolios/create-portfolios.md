---
product-area: portfolios
navigation-topic: create-and-manage-portfolios
title: Crear un Portfolio
description: Un portafolio es una colección de proyectos que se completan para los mismos recursos, presupuesto y programación. Los proyectos de un portafolio son lo suficientemente similares como para utilizar el mismo conjunto de recursos y medirse con el mismo cuadro de resultados.
author: Alina
feature: Work Management, Strategic Planning
exl-id: fdaed68d-d9cc-4514-8f80-b169cdd739bd
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/p47W1Seb-Ew-p-ogdb-ebjLAuxvY-0rdRHLMQtWCH30
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40cid: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 890
ht-degree: 58%

---

# Crear un portafolio

<!--Audited: 08/2025-->

Un portafolio es una colección de proyectos que se completan para los mismos recursos, presupuesto y programación. Los proyectos de un portafolio son lo suficientemente similares como para utilizar el mismo conjunto de recursos y medirse con el mismo cuadro de resultados.

Puede utilizar portafolios para agrupar proyectos que pertenezcan a las mismas líneas de productos, divisiones, departamentos, compañías u otras unidades de negocio.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquete</td> 
   <td> <p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de [!UICONTROL Edit] al portafolio</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Después de crear un portafolio, tiene permisos de administración</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Any</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td> <p>New: [!UICONTROL Standard]</p>
   <p>Current:[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>After you create a portfolio, you have Manage permissions to it, by default</p>  </td> 
  </tr> 
 </tbody> 
</table>

*For information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

## Formas de crear portafolios

Puede crear portafolios en Workfront mediante uno de los métodos siguientes:

* Cree un portafolio desde cero empezando por el área Portafolios del menú principal. Este artículo describe cómo crear un portafolio desde cero.

* Importe un portafolio mediante kick-starts.

  Como administrador de Workfront, puede importar portafolios mediante una &quot;kick-start&quot;.

  Para obtener información acerca de cómo importar datos mediante kick-starts en Workfront, consulte [Importar datos en Adobe Workfront a través de una plantilla de Kick-Start](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

* Agregue portafolios de Workfront Planning de las siguientes maneras:

   * Al conectarlos desde un tipo de registro en Workfront Planning.

  Para obtener información acerca de cómo crear portafolios agregándolos a registros, vea la sección &quot;Crear registros al conectarlos&quot; en el artículo [Crear registros](/help/quicksilver/planning/records/create-records.md).
   * Uso de automatizaciones de Workfront Planning.

  Para obtener más información, vea [Crear objetos mediante automatizaciones de registros de Adobe Workfront Planning](/help/quicksilver/planning/records/create-wf-objects-using-planning-automations.md).

  Debe tener una nueva licencia de Workfront y un paquete de Workfront Planning adicional para Workfront Planning.

  Para obtener información sobre el acceso a Workfront Planning, consulte [Información general sobre el acceso](/help/quicksilver/planning/access/access-overview.md).


## Crear un portafolio

{{step1-click-main-menu}}

1. Haga clic en **[!UICONTROL Portafolio]**.

1. (Condicional) Según el almacenamiento de documentos que utilice su organización, haga clic en una de las siguientes opciones:

   * **Nuevo portafolio**, cuando el administrador de Workfront elige **Adobe cloud storage** o **Workfront heredado**, y seleccionó o no la configuración **Permitir al usuario seleccionar el proveedor de almacenamiento**.
   * **Nuevo portafolio (almacenamiento heredado)**, cuando el administrador de Workfront elige **almacenamiento en la nube de Adobe** o **Workfront heredado**, y también selecciona la configuración **Permitir que el usuario seleccione el proveedor de almacenamiento**.

     Esta opción solo se muestra cuando la opción **Permitir que el usuario seleccione el proveedor de almacenamiento** está seleccionada en el área de configuración.

     Para obtener más información, consulte [Habilitar el almacenamiento en la nube de Adobe para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-esm.md).

     >[!NOTE]
     >
     >Es posible que la instancia de Workfront no tenga ambos tipos de almacenamiento de documentos.

     Se crea un portafolio y su nombre predeterminado sigue los siguientes patrones, según el almacenamiento que utilice Workfront para los documentos:

      * `Untitled Portfolio` para un portafolio de almacenamiento de Workfront heredado.

        Un portafolio de almacenamiento heredado de Workfront muestra un **almacenamiento heredado de Workfront** icono ![icono del portafolio de almacenamiento heredado](assets/legacy-storage-project-icon.png) junto a su nombre.

      * `Untitled Portfolio - < Month day, year hour.minute.second >` para un portafolio de almacenamiento en la nube de Adobe

        >[!IMPORTANT]
        >
        >Los portafolios que utilizan el almacenamiento en la nube de Adobe deben tener nombres únicos.

     Para los portafolios de almacenamiento en la nube de Adobe, se crea automáticamente una nueva carpeta de documentos con el mismo nombre que el portafolio en el área Documentos.

1. Reemplace el nombre del portafolio por un nuevo nombre en el encabezado del portafolio.

   El nombre puede contener hasta 255 caracteres.

1. (Opcional) Haga clic en el nombre bajo **[!UICONTROL Administrador de portafolios]** en el encabezado situado en la parte superior de la página para asignar un administrador diferente para el portafolio.

   ![nombre del administrador de Portfolio](assets/portfolio-manager-name-350x51.jpg)

   Como creador del portafolio, se le asigna como administrador de portafolios de forma predeterminada.

1. Haga clic en **[!UICONTROL Papelera de reciclaje]** en el panel de la izquierda.
1. En el área **[!UICONTROL Información general]**, cambie la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Description]</td> 
      <td> <p>Escriba una descripción para que el Portafolios indique lo que tiene de único. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Portfolio Manager]</td> 
      <td> <p>Comience a escribir el nombre de un usuario que desee indicar como administrador del portafolio y, a continuación, selecciónelo cuando aparezca en la lista. Es igual que el [!UICONTROL Portfolio Owner]. Es la persona que puede supervisar el trabajo definido en los proyectos del portafolio y aprobar el caso empresarial.</p> <p>Importante: Cuando designa a alguien como [!UICONTROL Portfolio Manager], obtiene automáticamente permisos de [!UICONTROL Manage] para el portafolio, los programas y los proyectos del portafolio. </p> <p>Sugerencia: también puede actualizar el [!UICONTROL Portfolio Manager] en el encabezado de la parte superior de la página.</p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Grupo </td> 
      <td> <p>Añada el nombre de un solo grupo si éste es propietario del portafolio o tiene la responsabilidad de completarlo. </p> <p>Para asegurarse de que esté seleccionando el grupo correcto, pase el puntero por encima de él y haga clic en el icono de [!UICONTROL information] <img src="assets/info-icon.png"> que aparece junto a él. Esta acción muestra la ayuda contextual con información sobre el grupo, como la jerarquía de los grupos que tiene por encima y sus administradores.</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/group-details-widget-portfolios-350x250.png" style="width: 350;height: 250;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Haga clic dentro del cuadro **[!UICONTROL Añadir formulario personalizado]** en la esquina superior derecha de la página [!UICONTROL Detalles del portafolio] para seleccionar un formulario personalizado para el portafolio y actualizar los campos personalizados.

   >[!TIP]
   >
   >Debe tener formularios personalizados de portafolio ya creados para poder adjuntarlos a los portafolios.

1. Haga clic en **[!UICONTROL Guardar cambios]**.
1. (Opcional) Haga clic en **[!UICONTROL Programas]** en el panel izquierdo y, a continuación, en **[!UICONTROL Añadir programas]** para añadir programas al portafolio.

   Para obtener más información sobre la creación de programas, consulte [Crear un programa](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

1. (Opcional) Haga clic en **[!UICONTROL Proyectos]** en el panel izquierdo y, a continuación, en **[!UICONTROL Añadir proyectos]** para añadir proyectos al portafolio.

   Para obtener más información sobre cómo añadir proyectos a un portafolio, consulte [Añadir proyectos a un portafolio](../../../manage-work/portfolios/create-and-manage-portfolios/add-projects-to-portfolios.md).

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
