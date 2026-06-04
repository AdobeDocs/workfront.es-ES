---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Editar documentos de forma masiva
description: Puede editar varios documentos a la vez en el área Documentos.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: e8badce6-86f5-416c-a238-f9b7f19cdd2d
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/bAHZFeyzwdwfL5DtWep5THlkv2t5MqhcIIq-pmuj4ps
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: e458b7274f0f80c8be395bdc8ad91eaf6cfd0876
workflow-type: tm+mt
source-wordcount: 915
ht-degree: 78%

---

# Editar documentos de forma masiva

Puede editar la descripción, añadir formularios personalizados y editar formularios personalizados en varios documentos a la vez.

## Consideraciones al editar formularios personalizados

Tenga en cuenta lo siguiente al editar formularios personalizados de documentos de forma masiva:

* La información que está cambiando en todos los documentos seleccionados sobrescribe la información existente en documentos individuales.
* Cuando se seleccionan proyectos que tienen valores diferentes para el mismo campo, el campo muestra un indicador “Varios valores”. Los campos que son casillas de verificación, botones de opción y conmutadores tienen el indicador “Varios valores” junto a ellos.
* Cuando se actualiza una opción en un campo de varias opciones (por ejemplo, un campo que se muestra como un conjunto de opciones o casillas de verificación), todas las demás opciones deben coincidir entre los documentos seleccionados.

>[!BEGINSHADEBOX]

**Ejemplo**
Puede tener un formulario personalizado con un campo de casilla de verificación con tres casillas de verificación (Opción 1, Opción 2 y Opción 3) y la Opción 1 está desactivada para todos los documentos seleccionados, y las Opciones 2 y 3 están seleccionadas para algunos y no están seleccionadas para otros documentos que ha seleccionado. Si desea comprobar la Opción 1 para todos los documentos, también debe hacer que la Opción 2 y la Opción 3 coincidan con todos los proyectos seleccionados antes de poder guardar los cambios. Por lo tanto, debe seleccionarlas o deseleccionarlas para que puedan coincidir en todos los proyectos seleccionados. Si no cambia ninguna de las opciones, puede guardar el campo tal cual y los documentos mantendrán su selección actual para todas las opciones.

>[!ENDSHADEBOX]

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquier paquete de Workfront para administrar documentos mediante el almacenamiento heredado de Workfront</p>
<p>Cualquier paquete de flujo de trabajo para administrar documentos mediante Adobe Cloud Storage.</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td><p>Colaborador o superior</p> 
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a documentos</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar el acceso al documento</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Editar documentos por lotes en el área de documentos heredados

Si su organización utiliza un almacenamiento de Workfront heredado, verá el área de documentos heredados al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento de Workfront, consulte [Diferencias entre el almacenamiento en la nube de Adobe y el almacenamiento de Workfront heredado](/help/quicksilver/review-and-approve-work/esm-overview.md#differences-between-adobe-cloud-storage-and-legacy-workfront-storage).

Para editar documentos de forma masiva, haga lo siguiente:

1. Vaya a la pestaña Documentos de un proyecto o al área Documentos del menú principal.
1. Presione Ctrl o Cmd en el teclado y seleccione los documentos que desee editar.
1. Haga clic en el icono Editar ![icono editar](assets/edit-icon.png).
   ![ubicación del icono editar en la página](assets/edit-multiple-documents.png)
1. (Opcional) Añada o edite la **Descripción**. Si la descripción de cada documento es diferente, verá _Múltiples valores_ en el cuadro de descripción. Puede añadir la misma descripción para todos los documentos, pero no puede editar descripciones de documentos individuales al editar de forma masiva.
1. Realice los siguientes cambios con los formularios personalizados:

   <table>
    <tr>
    <td><strong>Añadir formularios</strong></td>
    <td>En el cuadro <strong>Agregar formulario personalizado</strong>, puede elegir entre formularios adjuntos y formularios para añadir. Los formularios adjuntos se encuentran en algunos de los documentos seleccionados, pero no en todos. Un formulario adjunto a todos los documentos seleccionados se muestra de forma automática en la ventana de edición.  </td>
    </tr>
    <tr>
    <td><strong>Editar formularios</strong></td>
    <td>Edite los formularios personalizados adjuntos. La información que cambie sobrescribirá la información existente en los documentos individuales. Los campos con valores diferentes en los documentos se muestran como “Múltiples valores”. </td>
    </tr>
    <tr>
    <td><strong>Reorganizar formularios</strong></td>
    <td>Haga clic en el formulario personalizado y arrástrelo para reorganizarlo.</td>
    </tr>
    </table>
1. Haga clic en **Guardar**.

## Editar documentos por lotes en el área de Documentos nueva


Si su organización utiliza el almacenamiento en la nube de Adobe, verá la nueva área Documentos al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento en la nube de Adobe, consulte [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para editar documentos de forma masiva, haga lo siguiente:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.
1. Presione Ctrl o Cmd en el teclado y seleccione los documentos que desee editar.
1. Haga clic en Editar en la parte inferior de la página.
   ![editar varios documentos](assets/bulk-edit-documents.png)
1. (Opcional) Añada o edite la **Descripción**. Si la descripción de cada documento es diferente, verá _Múltiples valores_ en el cuadro de descripción. Puede añadir la misma descripción para todos los documentos, pero no puede editar descripciones de documentos individuales al editar de forma masiva.
1. Realice los siguientes cambios con los formularios personalizados:

   <table>
    <tr>
    <td><strong>Añadir formularios</strong></td>
    <td>En la sección <strong>Formulario personalizado</strong>, puede agregar un nuevo formulario personalizado a los documentos seleccionados. Los formularios personalizados adjuntos a todos los documentos seleccionados se muestran en la sección <strong>Formularios personalizados en común</strong>.  </td>
    </tr>
    <tr>
    <td><strong>Editar formularios</strong></td>
    <td>Edite los formularios personalizados adjuntos. La información que cambie sobrescribirá la información existente en los documentos individuales. Los campos con valores diferentes en los documentos se muestran como “Múltiples valores”. </td>
    </tr>
    </table>
1. Haga clic en **Guardar**.

## Editar documentos de forma masiva en un informe de documento

1. Desplácese a un informe de documento existente.
o
Cree un informe de documento como se describe en [Crear un informe personalizado](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Seleccione los documentos que desea editar.
1. Haga clic en el icono Editar ![icono editar](assets/edit-icon.png).
1. (Opcional) Añada o edite la **Descripción**. Si la descripción de cada documento es diferente, verá _Múltiples valores_ en el cuadro de descripción. Puede añadir la misma descripción para todos los documentos, pero no puede editar descripciones de documentos individuales al editar de forma masiva.
1. Realice los siguientes cambios con los formularios personalizados:

   <table>
    <tr>
    <td><strong>Añadir formularios</strong></td>
    <td>En el cuadro <strong>Agregar formulario personalizado</strong>, puede elegir entre formularios adjuntos y formularios para añadir. Los formularios adjuntos se encuentran en algunos de los documentos seleccionados, pero no en todos. Un formulario adjunto a todos los documentos seleccionados se muestra de forma automática en la ventana de edición.  </td>
    </tr>
    <tr>
    <td><strong>Editar formularios</strong></td>
    <td>Edite los formularios personalizados adjuntos. La información que cambie sobrescribirá la información existente en los documentos individuales. Los campos con valores diferentes en los documentos se muestran como “Múltiples valores”. </td>
    </tr>
    <tr>
    <td><strong>Reorganizar formularios</strong></td>
    <td>Haga clic en el formulario personalizado y arrástrelo para reorganizarlo.</td>
    </tr>
    </table>
1. Haga clic en **Guardar**.
