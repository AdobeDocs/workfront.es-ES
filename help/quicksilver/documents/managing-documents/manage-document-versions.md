---
product-area: documents
navigation-topic: manage-documents
title: Administrar versiones de documentos
description: Puede administrar varias versiones de un documento en Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 477153e4-847b-46ec-8107-72a7399c3767
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '514'
ht-degree: 0%

---

# Administrar versiones de documentos

Puede administrar varias versiones de un documento en Workfront.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Ver acceso a documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver acceso al documento</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

* Este artículo supone que el documento tiene varias versiones.

   Si necesita información sobre cómo cargar nuevas versiones de un documento a Workfront, consulte [Cargar una nueva versión de un documento](../../documents/managing-documents/upload-new-document-version.md).

## Ver una lista de todas las versiones de un documento

1. En el Resumen, desplácese hasta la vista del **Todas las versiones** para obtener más información. Aquí puede ver todas las versiones del documento.

## Ver y administrar detalles de una versión de documento anterior

1. Cerca de la parte superior de la página Detalles del documento, haga clic en el menú desplegable junto al nombre y, a continuación, haga clic en el nombre de la versión que desee ver y administrar.

   ![](assets/version-drop-dn-doc-dtls-nwe-350x93.png)

   Junto con la visualización de los Detalles de la versión, puede realizar cambios en la versión, como su nombre, metadatos y configuración de pruebas (si es una prueba de documento).

## Descargar una sola versión de documento

1. En el resumen, en **Versiones**, haga clic en el menú Más ![](assets/more-icon.png) a la derecha de la versión, haga clic en **Descargar** en la lista desplegable que aparece.

   ![](assets/more-versions-350x143.png)

## Descargar todas las versiones de un documento

1. Haga clic en **Detalles del documento** y, a continuación, seleccione **Todas las versiones** en el panel izquierdo.

1. Haga clic en **Descargar todo** en la parte superior de la lista.

## Eliminar una versión de documento

Si carga una versión de un documento por error o ya no se necesita una versión, puede eliminar la versión y mantener el documento original.

>[!IMPORTANT]
>
>No puede recuperar una versión de documento que elimine individualmente.

Tenga en cuenta lo siguiente cuando considere la posibilidad de eliminar una versión de documento:

* Solo se puede eliminar una versión a la vez. Si se elimina una versión, esta acción aparece en la sección **Actualizaciones** en el documento .
* Si carga una nueva versión después de eliminar una versión, la nueva versión recibe el siguiente número secuencial. Por ejemplo, si hay 3 versiones de un documento y elimina la versión 3, el siguiente documento cargado será la versión 4.
* Las actualizaciones del sistema y los comentarios realizados en una versión se conservan en Workfront después de eliminar la versión.

   <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a document version in Workfront does not delete the Proof version.&nbsp;</li>
  -->

Para eliminar una versión de documento:

1. Vaya al proyecto, la tarea o el problema que contiene el documento y, a continuación, seleccione **Documentos** Busque el documento que necesita.
1. En el **Versión** en el Resumen, haga clic en la versión y, a continuación, haga clic en **Eliminar** en la lista desplegable que aparece. La variable **Eliminar** solo está visible si hay al menos dos versiones.

   Si el documento está vinculado a un origen externo, ese vínculo se elimina y ya no se puede acceder al documento a través de Workfront.

   ![](assets/more-versions-350x143.png)
