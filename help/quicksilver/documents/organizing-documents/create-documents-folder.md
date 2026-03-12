---
product-area: documents
navigation-topic: organize-documents
title: Crear carpetas de documentos
description: Los documentos se pueden organizar en carpetas. Puede crear carpetas personales en el área de documentos personales.
author: Courtney
feature: Digital Content and Documents
exl-id: 41974d6b-fb00-49b7-9db2-36519994e0fd
source-git-commit: ff05270bd808d26abfed7b0d20b37f0bfc314c08
workflow-type: tm+mt
source-wordcount: '775'
ht-degree: 31%

---

# Crear carpetas de documentos

Los documentos se pueden organizar en carpetas. Actualmente, Workfront tiene dos versiones del área Documentos: el área de documentos heredados y el área de documentos nuevos. La versión que utilice su organización depende de si su organización utiliza almacenamiento de Workfront heredado o almacenamiento empresarial. Para obtener más información acerca de estos tipos de almacenamiento, vea [Información general sobre el almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
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

Si su organización está en un almacenamiento de Workfront heredado, verá el área de documentos heredados al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento heredado de Workfront, consulte [Diferencias entre el almacenamiento empresarial de Adobe y el almacenamiento heredado de Workfront](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-enterprise-storage-and-legacy-workfront-storage).

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

## Crear carpetas de documentos en el área de documentos nuevos

Si su organización utiliza el almacenamiento empresarial, verá el área de nuevos documentos al acceder a ellos en Workfront. Para obtener más información acerca del almacenamiento empresarial, consulte [Descripción general del almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

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
>En el cuadro de diálogo Mover solo están disponibles los proyectos, las tareas y los problemas que utilizan el mismo tipo de almacenamiento. Por ejemplo, si mueve una carpeta en un proyecto de almacenamiento empresarial, solo los proyectos, las tareas y los problemas que utilizan el almacenamiento empresarial están disponibles para su traslado a.


Para mover una carpeta:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.
1. Busque la carpeta que quiera mover y luego haga clic en el icono **Más** ![más](assets/more-icon.png).
1. Haga clic en **Mover** y, a continuación, seleccione el proyecto, la tarea o el problema al que desee mover la carpeta.


   ![mover carpeta](assets/rename-folder.png)

<!-- STEPS PLACEHOLDER: Add steps for moving a folder in the new documents area -->

### Eliminar una carpeta

Para eliminar una carpeta:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.
1. Busque la carpeta que desee eliminar y, a continuación, haga clic en el icono **Más** ![más](assets/more-icon.png).
1. Haga clic **eliminar**.

   ![eliminar carpeta](assets/rename-folder.png)
