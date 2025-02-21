---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Ver las fases del flujo de trabajo automatizado en una revisión
description: Puede realizar un práctico seguimiento del progreso de una revisión configurada con un flujo de trabajo automatizado. Puede ver, modificar, añadir, iniciar y bloquear el trabajo ya realizado en las fases de la revisión.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '549'
ht-degree: 82%

---

# Ver las fases del flujo de trabajo automatizado en una revisión

Puede realizar un práctico seguimiento del progreso de una revisión configurada con un flujo de trabajo automatizado. Puede ver, modificar, añadir, iniciar y bloquear el trabajo ya realizado en las fases de la revisión.

Para obtener información sobre cómo añadir fases y usuarios a una revisión con un flujo de trabajo automatizado, consulte [Añadir fases y usuarios a un flujo de trabajo automatizado en una revisión](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: pro o superior</p> <p>o</p> <p>Plan heredado: select o premium</p> <p>Para obtener más información sobre el acceso de revisión con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: trabajo o plan</p> <p>Plan heredado: cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de prueba </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Ver el diagrama de flujo de trabajo automatizado

1. En una lista de documentos que contenga el documento, pase el puntero por encima de la fila que contiene el documento y, a continuación, haga clic en **Flujo de trabajo de revisión**.

   El diagrama del flujo de trabajo automatizado se muestra justo debajo del título del flujo de trabajo.

   Las fases del diagrama se marcan de la siguiente manera:

   ![dot.png](assets/dot.png) Fase activa

   ![gray_dot.png](assets/grey-dot.png) Fase inactiva\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  Fase privada

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  Fase bloqueada

   Las líneas entre las fases representan las dependencias entre las fases. Las líneas que conducen a fases inactivas aparecen punteadas hasta que se activa la etapa.

   Puede pasar el puntero por encima de una fase del diagrama para mostrar su progreso. Si la fase no está activa y tiene derechos de edición en la fase, puede hacer clic en el botón Activar fase ![Activar fase](assets/activate-stage-btn.png) para iniciar la fase. Si la fase está activa y tiene derechos de edición en la fase, puede bloquearla. ![Bloquear fase](assets/lock-stage-btn.png) Para obtener más información sobre la barra de progreso (S, O, C, D) , consulte  [Ver el progreso y el estado de una revisión en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Ver una fase

1. En una lista de documentos que contenga el documento, pase el puntero por encima de la fila que contiene el documento y, a continuación, haga clic en **Flujo de trabajo de revisión**.
1. En el diagrama, haga clic en la fase que desee ver.

   ![Ver diagrama de fase](assets/view-stage-diagram-350x204.png)

1. Para expandir los detalles de una fase, haga clic en la flecha lateral de debajo de su nombre.

   ![Detalles del escenario](assets/stage-details-caret-350x167.png)

## Ver todas las fases

Para ver todas las fases de un flujo de trabajo automatizado:

1. Haga clic en el botón Cambiar vista en la parte superior de la página ![Cambiar vista](assets/change-view-btn.png) y, a continuación, haga clic en **Ver todas las fases**.

   Todas las fases del flujo de trabajo automatizado se enumeran en la sección; sin embargo, los detalles están ocultos.

1. Para expandir los detalles de una fase, haga clic en la flecha lateral de debajo de su nombre.

## Ver todas las etapas en detalle

Para ver todas las fases del flujo de trabajo automatizado con sus detalles expandidos:

1. Haga clic en el botón Cambiar vista en la parte superior de la página ![Cambiar vista](assets/change-view-btn.png) y, a continuación, haga clic en **Ver todas las fases en detalle**.
1. Para ver los detalles de una fase, haga clic en la flecha hacia abajo debajo de su nombre.
