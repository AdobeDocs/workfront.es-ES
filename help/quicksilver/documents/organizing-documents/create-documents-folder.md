---
product-area: documents
navigation-topic: organize-documents
title: Crear carpetas de documentos
description: Los documentos se pueden organizar en carpetas. Puede crear carpetas personales en el área de documentos personales.
author: Courtney
feature: Digital Content and Documents
exl-id: 41974d6b-fb00-49b7-9db2-36519994e0fd
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/L473t3JSVgXHJ-RQXLXkBxQdzh9TbBwXM42DeiiCR7s
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 811
ht-degree: 30%

---

# Crear carpetas de documentos

Los documentos se pueden organizar en carpetas. Actualmente, Workfront tiene dos versiones del área Documentos: el área de documentos heredados y el área de documentos nueva. La versión que utilice su organización depende de si su organización utiliza almacenamiento de Workfront heredado o almacenamiento en la nube de Adobe. Para obtener más información acerca de estos tipos de almacenamiento, vea [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete de Workfront para administrar documentos mediante el almacenamiento heredado de Workfront</p>
<p>Cualquier paquete de flujo de trabajo para administrar documentos mediante Adobe Cloud Storage.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p>
   <p>Revisión o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear carpetas de documentos en el área de documentos heredados

Si su organización está en un almacenamiento de Workfront heredado, verá el área de documentos heredados al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento heredado de Workfront, consulte [Diferencias entre el almacenamiento en la nube de Adobe y el almacenamiento heredado de Workfront](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

>[!NOTE]
>
>La organización de los documentos simplemente crea vínculos entre los documentos y los objetos con los que se asocian. No los reubica en el sistema.

### Mostrar carpetas

Puede mostrar carpetas en vista de miniaturas, estándar o de lista. Para cambiar la vista, utilice las opciones de vista de la esquina superior derecha.

{{step1-to-documents}}

O

Con un objeto de Workfront abierto, haga clic en **Documentos** en el panel izquierdo.

1. Haga clic en las opciones de vista encima del panel derecho para cambiar la forma en que se muestran los documentos.

   ![Opciones de vista de documento](assets/screenshot-2016-07-07-12.46.54.png)

### Crear carpetas y subcarpetas

Cree carpetas para organizar mejor los documentos. Puede crear hasta 2000 carpetas en un objeto y hasta 50 subcarpetas dentro de cada carpeta. Las subcarpetas se cuentan hasta un máximo de 2000 carpetas.

{{step1-to-documents}}

O

Con un objeto de Workfront abierto, haga clic en **Documentos** en el panel izquierdo.

1. Para crear una carpeta de nivel superior, asegúrese de que no hay nada seleccionado y luego haz clic en **Añadir nuevo** > **Carpeta**.

   O

   Para crear una subcarpeta, selecciónela donde desee crear la subcarpeta y, a continuación, haga clic en **Añadir nuevo** > **Carpeta**.

### Compartir carpetas

Para obtener información acerca de cómo compartir carpetas, consulte [Compartir una carpeta de documentos](../../workfront-basics/grant-and-request-access-to-objects/share-a-document-folder.md).

## Crear carpetas de documentos en el área de documentos nueva

Si su organización utiliza el almacenamiento en la nube de Adobe, verá la nueva área Documentos al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento en la nube de Adobe, consulte [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

### Carpetas generadas por el sistema

Cuando se carga un documento en una tarea o un problema, Workfront crea automáticamente una carpeta generada por el sistema denominada después de la tarea o el problema. Esta carpeta está vinculada a la tarea o al problema y hereda sus permisos. Las carpetas generadas por el sistema son visibles en el área de documentos de nivel de proyecto.

Para obtener más información sobre los permisos de carpeta, consulte [Funcionamiento de los permisos de documentos](/help/quicksilver/review-and-approve-work/esm-access-permissions.md#how-document-permissions-work).

### Creación de subcarpetas

Puede crear subcarpetas dentro de una carpeta generada por el sistema para organizar aún más los documentos. Todas las subcarpetas heredan los permisos de la carpeta principal.

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.
1. Haga clic en la carpeta en la que desee crear una subcarpeta y, a continuación, haga clic en el icono **Agregar carpeta** ![agregar icono de carpeta](assets/add-folder-icon.png).
   ![agregar subcarpeta](assets/add-subfolder.png)
1. Escriba un nombre para la subcarpeta y haga clic en **Crear**.

### Cambiar nombre de carpeta

Las carpetas generadas por el sistema heredan automáticamente el nombre de la tarea o el problema. Se les puede cambiar el nombre haciendo clic en el nombre de la carpeta y editándola.

Para cambiar el nombre de una carpeta:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.
1. Busque la carpeta cuyo nombre desea cambiar y, a continuación, haga clic en el icono **Más** ![más](assets/more-icon.png).
1. Haga clic en **Cambiar nombre** y, a continuación, escriba un nombre nuevo para la carpeta.

   ![cambiar el nombre de la carpeta](assets/rename-folder.png)

1. Haga clic en **Cambiar nombre**.

### Mover una carpeta

Las carpetas generadas por el sistema se pueden mover a otro proyecto, tarea o problema. Si una carpeta generada por el sistema se mueve a otra ubicación, su objeto vinculado se actualiza al nuevo objeto y los permisos se heredan del nuevo objeto principal. También puede mover subcarpetas a otro proyecto, tarea o problema.

>[!NOTE]
>
>En el cuadro de diálogo Mover solo están disponibles los proyectos, las tareas y los problemas que utilizan el mismo tipo de almacenamiento. Por ejemplo, si mueve una carpeta en un proyecto de almacenamiento en la nube de Adobe, solo los proyectos, las tareas y los problemas que utilizan el almacenamiento en la nube de Adobe están disponibles para su traslado a.


Para mover una carpeta:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.
1. Busque la carpeta que quiera mover y luego haga clic en el icono **Más** ![más](assets/more-icon.png).
1. Haga clic en **Mover** y, a continuación, seleccione el proyecto, la tarea o el problema al que desee mover la carpeta.


   ![mover carpeta](assets/rename-folder.png)

<!-- STEPS PLACEHOLDER: Add steps for moving a folder in the new Documents area -->

### Eliminar una carpeta

Para eliminar una carpeta:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.
1. Busque la carpeta que desee eliminar y, a continuación, haga clic en el icono **Más** ![más](assets/more-icon.png).
1. Haga clic **eliminar**.

   ![eliminar carpeta](assets/rename-folder.png)
