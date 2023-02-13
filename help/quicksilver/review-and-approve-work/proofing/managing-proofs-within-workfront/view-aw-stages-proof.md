---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Ver las etapas del flujo de trabajo automatizado en una prueba
description: Puede realizar un seguimiento del progreso de una prueba configurada con un flujo de trabajo automatizado. Puede ver, modificar, añadir, iniciar y bloquear el trabajo ya realizado en las fases de la prueba.
author: Courtney
feature: Digital Content and Documents
exl-id: 71df1445-c64c-4de2-a9b8-23bd47898b6d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '527'
ht-degree: 0%

---

# Ver las etapas del flujo de trabajo automatizado en una prueba

Puede realizar un seguimiento del progreso de una prueba configurada con un flujo de trabajo automatizado. Puede ver, modificar, añadir, iniciar y bloquear el trabajo ya realizado en las fases de la prueba.

Para obtener información sobre cómo agregar etapas y usuarios a una prueba con un flujo de trabajo automatizado, consulte [Agregar etapas y usuarios a un flujo de trabajo automatizado en una prueba](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/add-stages-users-to-automated-workflow-proof.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o superior</p> <p>o</p> <p>Plan heredado: Select o Premium</p> <p>Para obtener más información sobre la prueba de acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de pruebas en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o plan</p> <p>Plan heredado: Cualquiera (debe tener las pruebas habilitadas para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Ver el diagrama de flujo de trabajo automatizado

1. En una lista de documentos que contenga el documento, pase el ratón sobre la fila que contiene el documento y haga clic en **Flujo de trabajo de prueba**.

   El diagrama del flujo de trabajo automatizado se muestra justo debajo del título del flujo de trabajo.

   Las etapas del diagrama se marcan de la siguiente manera:

   ![dot.png](assets/dot.png) Estadio activo

   ![gray_dot.png](assets/grey-dot.png) Etapa inactiva\
   ![sbw-key-icon.png](assets/sbw-key-icon.png)  Fase privada

   ![sbw-padlock-icon.png](assets/sbw-padlock-icon.png)  Etapa bloqueada

   Las líneas entre las etapas representan las dependencias entre las etapas. Las líneas que conducen a etapas inactivas se puntean hasta que se activa el escenario.

   Puede situar el cursor sobre un escenario del diagrama para mostrar su progreso. Si el escenario no está activo y tiene derechos de edición en el escenario, puede hacer clic en el botón Activar etapa ![](assets/activate-stage-btn.png) para iniciar el escenario. Si el escenario está activo y tiene derechos de edición en el escenario, puede bloquearlo. ![](assets/lock-stage-btn.png) Para obtener más información sobre la barra de progreso (S, O, C, D) , consulte  [Ver el progreso y estado de una prueba en Workfront Proof](../../../workfront-proof/wp-work-proofsfiles/manage-your-work/view-progress-and-status-of-proof.md).

## Ver un escenario

1. En una lista de documentos que contenga el documento, pase el ratón sobre la fila que contiene el documento y haga clic en **Flujo de trabajo de prueba**.
1. En el diagrama, haga clic en el escenario que desee ver.

   ![](assets/view-stage-diagram-350x204.png)

1. Para expandir los detalles de un escenario, haga clic en la flecha lateral debajo de su nombre.

   ![](assets/stage-details-caret-350x167.png)

## Ver todas las etapas

Para ver todas las etapas de un flujo de trabajo automatizado:

1. Haga clic en el botón Cambiar vista en la parte superior de la página ![](assets/change-view-btn.png)y haga clic en **Ver todas las etapas**.

   En la sección se enumeran todas las etapas del flujo de trabajo automatizado, aunque los detalles están ocultos.

1. Para expandir los detalles de un escenario, haga clic en la flecha lateral debajo de su nombre.

## Ver todas las etapas en detalle

Para ver todas las etapas del flujo de trabajo automatizado con sus detalles ampliados:

1. Haga clic en el botón Cambiar vista en la parte superior de la página ![](assets/change-view-btn.png)y haga clic en **Ver todas las etapas en detalle**.
1. Para ver los detalles de un escenario, haga clic en la flecha abajo bajo su nombre.
