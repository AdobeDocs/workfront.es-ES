---
product-area: portfolios;projects
navigation-topic: create-and-manage-portfolios
title: Añadir proyectos a un Portfolio
description: Le recomendamos que cuando inicie proyectos, los añada a un portafolio. Sin embargo, puede añadirlos a un portafolio en cualquier momento durante su vida útil.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 97f36c18-3ac8-45ac-b5bc-dfe8b1363faf
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/UkUQdW12tLqRjh5zmbwtjNfRxFwc-Uhj2gGwjmDyKb8
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 689
ht-degree: 42%

---

# Añadir proyectos a un portafolio

<!--Audited: 08/2025-->

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>
-->

Le recomendamos que cuando inicie proyectos, los añada a un portafolio. Sin embargo, puede añadirlos a un portafolio en cualquier momento durante su vida útil.

Al añadir proyectos a un portafolio, tenga en cuenta lo siguiente:

* Solo puede asociar un portafolio con un proyecto.
* Un proyecto permanece en un portafolio hasta que se elimina o se asocia con otro.
* Un portafolio puede contener un número ilimitado de proyectos.

>[!CAUTION]
>
>Es posible que los permisos heredados no se apliquen correctamente cuando se utilizan en un gran número de objetos secundarios.
>   
>Para evitar problemas de permisos heredados, recomendamos lo siguiente:
>
>* Limite el número de objetos secundarios (proyectos) bajo un solo elemento principal (portafolio o programa). Recomendamos no más de 10.000 proyectos por portafolio o programa.
>
>* Reduzca la profundidad de la herencia al aplicar permisos en un objeto de nivel inferior.
>
>  Por ejemplo, aplique los permisos directamente en el nivel de proyecto en lugar de depender de los permisos heredados del portafolio para el programa y, a continuación, para el proyecto.
>
>* Divida los programas para que contengan menos proyectos, lo que reduce la complejidad de los permisos.
>


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] paquete</td> 
   <td> <p>Cualquiera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td><p>Estándar</p> 
   <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuración de nivel de acceso</td> 
   <td> <p>Acceso [!UICONTROL Edit] a portafolios</p> <p>Acceso [!UICONTROL Edit] a proyectos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de [!UICONTROL Manage] al portafolio</p> <p>Permisos de [!UICONTROL Manage] a los proyectos</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level</td> 
   <td> <p>[!UICONTROL Edit] access Portfolios</p> <p>[!UICONTROL Edit] access to Projects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>[!UICONTROL Manage] permissions to the projects</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## Añadir un proyecto a un portafolio

1. Vaya a un portafolio y, a continuación, haga clic en **[!UICONTROL Proyectos]** en el panel izquierdo.

   ![Portfolio con proyectos](assets/qs-portfolio-with-projects-350x90.png)

1. Haga clic en **[!UICONTROL Nuevo proyecto]** y seleccione un método para añadir un proyecto.

   >[!TIP]
   >
   >No se puede agregar un proyecto al ver la lista de proyectos en la vista [!UICONTROL Hito].

   Seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody>

   <tr> 
      <td role="rowheader">[!UICONTROL New Project]</td> 
      <td> <p>Añada un proyecto nuevo. </p> <p>Para obtener más información sobre cómo crear un proyecto, vea <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Crear un proyecto</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nuevo proyecto (almacenamiento heredado)]</td> 
      <td> <p>Añada un nuevo proyecto de almacenamiento de Workfront. </p>
      <p>La opción solo se muestra cuando su organización utiliza el almacenamiento de documentos en la nube de Workfront y Adobe. Es posible que la instancia de Workfront no tenga ambos tipos de almacenamiento.</p>
       <p>Para obtener más información sobre cómo crear un proyecto, vea <a href="../../../manage-work/projects/create-projects/create-project.md" class="MCXref xref">Crear un proyecto</a>. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Nuevo proyecto a partir de plantilla]</td> 
      <td> <p>Añada un nuevo proyecto con una plantilla existente. </p> <p>Para obtener más información sobre la creación de un proyecto a partir de una plantilla, consulte <a href="../../../manage-work/projects/create-projects/create-project-from-template.md" class="MCXref xref">Crear un proyecto mediante una plantilla</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Importar [!DNL MS Project]] </td> 
      <td> <p>Añada un proyecto que previamente exportó desde [!DNL MS Project] y que ha guardado en su equipo. </p> <p>Para obtener más información sobre la creación de un nuevo proyecto importándolo desde [!DNL Microsoft Project], consulte <a href="../../../manage-work/projects/create-projects/import-project-from-ms-project.md" class="MCXref xref">Importar un proyecto desde [!DNL Microsoft Project]</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Request Project]</td> 
      <td> <p>Solicite la aprobación de un proyecto.</p> <p>Para obtener información sobre cómo solicitar proyectos, consulte <a href="../../../manage-work/projects/create-projects/request-project.md">Solicitar un proyecto</a>. </p> </td> 
     </tr> 
          <tr> 
      <td role="rowheader">[!UICONTROL Existing Project]</td> 
      <td> <p>Añada un proyecto que ya se haya creado.</p> </td> 
     </tr>
    </tbody> 
   </table>

   <!-- update screen shot for both kinds of storages??-->

   ![Nuevo menú desplegable de proyecto](assets/new-project-dropdown-expanded-from-portfolio-nwe-350x376.png)

1. (Condicional) Si ha seleccionado agregar un proyecto existente, se abrirá el cuadro **Agregar proyectos**. <!--check this after UI changes-->

   ![Agregar proyecto existente](assets/add-existing-projects-to-portfolios-box.png) <!--check this after UI changes-->

1. Empiece a escribir el nombre de un proyecto en el campo **[!UICONTROL Agregar proyectos a este portafolio]** y, a continuación, haga clic en ellos cuando aparezcan en la lista.  <!--check this after UI changes-->

   Puede agregar más de un proyecto.

   >[!NOTE]
   >
   >Cuando su organización utiliza el almacenamiento en la nube heredado de Workfront y Adobe para documentos, existen los siguientes escenarios:
   >
   >
   >* Cuando agrega un proyecto de almacenamiento en la nube de Adobe a una cartera de productos de almacenamiento de Workfront heredados y esta no tiene documentos adjuntos, la cartera se convierte en una cartera de productos de almacenamiento en la nube de Adobe.
   >* Cuando agrega un proyecto de almacenamiento en la nube de Adobe a una cartera de productos de almacenamiento de Workfront heredados y esta tiene documentos adjuntos a él, el almacenamiento de documentos de la cartera permanece en el almacenamiento de Workfront. Sin embargo, el icono de almacenamiento heredado de Workfront ![Icono de almacenamiento heredado de Workfront](assets/legacy-storage-project-icon.png) se eliminará del portafolio.
   >* No puede agregar un proyecto de almacenamiento de Workfront heredado a un catálogo de productos de Adobe Cloud Storage.
   >
   >Para obtener más información, vea [Información general sobre la administración de documentos de proyectos y objetos relacionados](/help/quicksilver/manage-work/projects/manage-projects/manage-documents-on-projects.md).
   >
   >No todas las instancias de Workfront tienen ambos tipos de almacenamiento de documentos.

1. (Opcional) Si decide no agregarlo al portafolio, haga clic en el icono **X** que aparece a la derecha del nombre del proyecto para quitarlo de la lista.

   <!--replace last step with this, for unshim: 1. (Optional) Click the **Delete** icon ![Delete icon](assets/delete-icon.png) next to the name of a project if you decide not to add it to the portfolio.-->

1. Haga clic en **[!UICONTROL Agregar proyectos]**. <!--check this after UI changes-->

   El proyecto o proyectos que ha seleccionado ahora están asociados al portafolio.
