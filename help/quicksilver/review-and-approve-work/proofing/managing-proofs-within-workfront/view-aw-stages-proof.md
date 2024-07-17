---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Visualización de las fases del flujo de trabajo automatizado en una prueba
description: Puede realizar un seguimiento práctico del progreso de una prueba configurada con un flujo de trabajo automatizado. Puede ver, modificar, agregar, iniciar y bloquear el trabajo ya realizado en las fases de la prueba.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '526'
ht-degree: 0%

---

# Visualización de las fases del flujo de trabajo automatizado en una prueba

Puede realizar un seguimiento práctico del progreso de una prueba configurada con un flujo de trabajo automatizado. Puede ver, modificar, agregar, iniciar y bloquear el trabajo ya realizado en las fases de la prueba.

Para obtener información sobre cómo agregar etapas y usuarios a una prueba con un flujo de trabajo automatizado, consulte [Agregar etapas y usuarios a un flujo de trabajo automatizado en una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o Superior</p> <p>o</p> <p>Plan heredado: Select o Premium</p> <p>Para obtener más información sobre cómo revisar el acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o Plan</p> <p>Plan heredado: Cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Responsable o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

## Ver el diagrama de flujo de trabajo automatizado

1. En una lista de documentos que contenga el documento, pase el ratón sobre la fila que contiene el documento y haga clic en **Flujo de trabajo de revisión**.

   El diagrama del flujo de trabajo automatizado se muestra justo debajo del título del flujo de trabajo.

   Las fases del diagrama se marcan de la siguiente manera:

   ![dot.png](assets/dot.png) fase activa

   ![gray_dot.png](assets/grey-dot.png) fase inactiva\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  Fase privada

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  Fase bloqueada

   Las líneas entre las fases muestran las dependencias entre las fases. Las líneas que conducen a etapas inactivas se puntean hasta que se activa la etapa.

   Puede situarse sobre una fase del diagrama para mostrar su progreso. Si la fase no está activa y tiene derechos de edición en la fase, puede hacer clic en el botón Activar fase ![](assets/activate-stage-btn.png) para iniciar la fase. Si la fase está activa y tiene derechos de edición en la fase, puede bloquearla. ![](assets/lock-stage-btn.png) Para obtener más información sobre la barra de progreso (S, O, C, D) , consulte  [Ver el progreso y el estado de una revisión en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Ver una fase

1. En una lista de documentos que contenga el documento, pase el ratón sobre la fila que contiene el documento y haga clic en **Flujo de trabajo de revisión**.
1. En el diagrama, haga clic en el escenario que desee ver.

   ![](assets/view-stage-diagram-350x204.png)

1. Para expandir los detalles de una etapa, haga clic en la flecha lateral debajo de su nombre.

   ![](assets/stage-details-caret-350x167.png)

## Ver todas las fases

Para ver todas las fases en un flujo de trabajo automatizado:

1. Haga clic en el botón Cambiar vista en la parte superior de la página ![](assets/change-view-btn.png) y, a continuación, haga clic en **Ver todas las fases**.

   Todas las fases del flujo de trabajo automatizado se enumeran en la sección; sin embargo, los detalles están ocultos.

1. Para expandir los detalles de una etapa, haga clic en la flecha lateral debajo de su nombre.

## Ver todas las etapas en detalle

Para ver todas las etapas del flujo de trabajo automatizado con sus detalles expandidos:

1. Haga clic en el botón Cambiar vista en la parte superior de la página ![](assets/change-view-btn.png) y, a continuación, haga clic en **Ver todas las fases en detalle**.
1. Para ver los detalles de una fase, haga clic en la flecha hacia abajo debajo de su nombre.
