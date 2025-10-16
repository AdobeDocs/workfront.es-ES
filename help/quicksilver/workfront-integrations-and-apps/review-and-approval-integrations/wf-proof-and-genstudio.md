---
content-type: reference
product-area: workfront-integrations
navigation-topic: workfront-integrations-navigation-topic
title: Introducción a la integración de GenStudio for Performance Marketing y Workfront Proof
description: Introducción a la integración de GenStudio for Performance Marketing y Workfront Proof
author: Courtney
feature: Workfront Integrations and Apps, Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: 9905a522-9913-49c0-8c80-a8b46221fcbb
source-git-commit: a65a4568c6428768ee6bc60a59a8499efdbec9f8
workflow-type: tm+mt
source-wordcount: '546'
ht-degree: 7%

---

# Introducción a la integración de GenStudio for Performance Marketing y Workfront Proof

Con la integración entre GenStudio for Performance Marketing y Workfront Proof, puede

* Uso de plantillas de prueba de Workfront para definir flujos de trabajo de revisión y aprobación

* Revise y apruebe el contenido de borrador de GenStudio for Performance Marketing en el visualizador de pruebas de Workfront

* Ver decisiones de revisión en GenStudio for Performance Marketing para su aprobación y publicación finales

Para obtener más información acerca de la revisión y aprobación en GenStudio for Performance Marketing, consulte [Integración de Workfront Proof con GenStudio for Performance Marketing](https://experienceleague.adobe.com/es/docs/genstudio-for-performance-marketing/user-guide/approve/proof-integration).


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
 <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> 
   <p>Cualquiera</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Estándar </p> 
   <p>Plan </p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Productos adicionales</td> 
   <td> 
   <p> Debe tener GenStudio for Performance Marketing y se le debe añadir al producto como usuario en Admin Console. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a proyectos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Requisitos de integración

* Workfront y GenStudio for Performance Marketing deben implementarse en la misma organización de Identity Management system (IMS).

* Los usuarios solo pueden pertenecer a una instancia de Workfront dentro de la organización IMS.

* La instancia de Workfront debe estar habilitada en la experiencia unificada de Adobe.

* La integración debe habilitarse en el área Configuración de Workfront.


## Habilitar la integración en Workfront

Debe ser administrador del sistema para habilitar esta integración.

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **[!UICONTROL Configuración]** ![Icono de configuración](/help/_includes/assets/gear-icon-setup.png).
1. En el panel izquierdo, haga clic en **Revisar y aprobar** > **Adobe GenStudio**.
1. Habilitar **Usar aprobaciones de revisión**.
   ![habilitar revisión para la configuración de GenStudio](assets/enable-proofing-gs.png)

## Uso de plantillas de prueba de Workfront para definir flujos de trabajo de aprobación

Si el proceso de revisión de contenido de su organización se repite con frecuencia o lo revisan las mismas personas, puede utilizar plantillas de prueba para automatizar los flujos de trabajo de revisión y aprobación.

### Creación de una plantilla de prueba en Workfront

Puede crear plantillas sencillas de una sola etapa para uno o dos revisores, o bien crear plantillas automatizadas de varias etapas para revisiones complejas con muchas fases y dependencias.

Para obtener más información sobre la creación de plantillas y flujos de trabajo automatizados en Workfront, consulte

* [Información general sobre flujos de trabajo automatizados](/help/quicksilver/review-and-approve-work/proofing/proofing-overview/automated-workflow.md)
* [Crear y administrar plantillas de flujo de trabajo automatizado](/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/create-manage-automated-workflow-templates.md)

### Elija o modifique la plantilla en GenStudio for Performance Marketing

Cuando un usuario inicia una revisión en GenStudio for Performance Marketing, simplemente elige la plantilla que necesita. Los usuarios pueden cambiar fácilmente cualquier plantilla de flujo de trabajo de prueba y agregar o eliminar revisores y fases en cualquier momento.

Para obtener más información, vea [Solicitar revisión y aprobación](https://experienceleague.adobe.com/es/docs/genstudio-for-performance-marketing/user-guide/approve/request-review).

## Revise y apruebe el contenido de borrador de GenStudio for Performance Marketing en el visualizador de pruebas de Workfront

Puede revisar y aprobar el contenido del borrador directamente en GenStudio for Performance Marketing en el visualizador de pruebas de Workfront.

Con el visualizador de pruebas, puede

* Dejar comentarios
* Borrador de marcado para mostrar lo que debe cambiar
* Tomar una decisión

Para obtener más información, vea [Revisar y editar contenido](https://experienceleague.adobe.com/es/docs/genstudio-for-performance-marketing/user-guide/approve/review-and-edit).


>[!IMPORTANT]
>
>Los usuarios deben instalar [Revisar contenido interactivo con la herramienta de revisión de Adobe Workfront](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/review-proof-in-web-viewer-extension.md) para poder empezar a revisar borradores en GenStudio for Performance Marketing.


## Ver decisiones de revisión en GenStudio for Performance Marketing para su aprobación y publicación finales

Una vez que el recurso ha pasado por el proceso de revisión y aprobación, puede ver la decisión de revisión y publicar el contenido directamente desde GenStudio for Performance Marketing.

Para obtener más información, consulte [Publicar contenido aprobado](https://experienceleague.adobe.com/es/docs/genstudio-for-performance-marketing/user-guide/approve/publish-content).
