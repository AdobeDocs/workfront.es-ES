---
content-type: reference
product-area: documents
navigation-topic: documents-navigation-topic
title: Editar documentos por lotes
description: Puede editar varios documentos a la vez en el área Documentos.
author: Courtney
feature: Digital Content and Documents
recommendations: noDisplay, noCatalog
exl-id: e8badce6-86f5-416c-a238-f9b7f19cdd2d
source-git-commit: f9ebf647c7672a9d471288806cf596d103007613
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 19%

---

# Editar documentos por lotes

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

Puede editar la descripción, agregar formularios personalizados y editar formularios personalizados en varios documentos a la vez.

## Consideraciones al editar formularios personalizados

Tenga en cuenta lo siguiente al editar formularios personalizados de documento de forma masiva:

* La información que está cambiando en todos los documentos seleccionados sobrescribe la información existente en documentos individuales.
* Cuando se seleccionan documentos con valores diferentes para un mismo campo, el campo muestra el indicador &quot;Varios valores&quot;. Los campos que son casillas de verificación, botones de opción y conmutadores tienen el indicador “Varios valores” junto a ellos.
* Cuando se actualiza una opción en un campo de varias opciones (por ejemplo, un campo que se muestra como un conjunto de opciones o casillas de verificación), todas las demás opciones deben coincidir entre los documentos seleccionados.

>[!BEGINSHADEBOX]

**Ejemplo**
Puede tener un formulario personalizado con un campo de casilla de verificación con tres casillas de verificación (Opción 1, Opción 2 y Opción 3) y la Opción 1 está desactivada para todos los documentos seleccionados, y las Opciones 2 y 3 están seleccionadas para algunos y no están seleccionadas para otros documentos que ha seleccionado. Si desea comprobar la opción 1 para todos los documentos, también debe hacer que las opciones 2 y 3 coincidan con todos los proyectos seleccionados antes de poder guardar los cambios. Por lo tanto, debe seleccionarlos o deseleccionarlos para que puedan coincidir en todos los proyectos seleccionados. Si no cambia ninguna de las opciones, puede guardar el campo tal cual y los documentos mantienen su selección actual para todas las opciones.

>[!ENDSHADEBOX]

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront*</td> 
   <td><p> Nuevo: colaborador o superior</p> 
   <p> Actual: solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar el acceso al documento</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

+++

## Editar documentos por lotes

Para editar documentos de forma masiva:

1. Vaya a la pestaña Documentos de un proyecto o al área Documentos del menú principal.
1. Presione ctrl o cmd en el teclado y seleccione los documentos que desee editar.
1. Haga clic en el icono Editar ![editar icono](assets/edit-icon.png).
   ![editar la ubicación del icono en la página](assets/edit-multiple-documents.png)
1. (Opcional) Agregue o edite la **Descripción**. Si la descripción de cada documento es diferente, verá _Varios valores_ en el cuadro de descripción. Puede agregar la misma descripción para todos los documentos, pero no puede editar descripciones de documentos individuales al editar de forma masiva.
1. Realice los siguientes cambios con los formularios personalizados:

   <table>
    <tr>
    <td><strong>Añadir formularios</strong></td>
    <td>En el cuadro <strong>Agregar formulario personalizado</strong>, puede elegir entre Formularios adjuntos y Formularios que desea agregar. Los formularios adjuntos se encuentran en algunos de los documentos seleccionados, pero no en todos. Se muestra automáticamente en la ventana de edición un formulario adjunto a todo el documento seleccionado.  </td>
    </tr>
    <tr>
    <td><strong>Editar formularios</strong></td>
    <td>Edite los formularios personalizados adjuntos. La información que cambie sobrescribirá la información existente en los documentos individuales. Los campos con valores diferentes en los documentos se muestran como "Varios valores". </td>
    </tr>
    <tr>
    <td><strong>Reorganizar formularios</strong></td>
    <td>Haga clic en el formulario personalizado y arrástrelo para reorganizarlo.</td>
    </tr>
    </table>
1. Haga clic en **Guardar**.

<span class="preview">

## Editar documentos por lotes en un informe de documento

1. Desplácese a un informe de documento existente.
o
Cree un informe de documento como se describe en [Crear un informe personalizado](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
1. Seleccione los documentos que desee editar.
1. Haga clic en el icono Editar ![editar icono](assets/edit-icon.png).
   ![editar la ubicación del icono en la página](assets/edit-multiple-documents.png)
1. (Opcional) Agregue o edite la **Descripción**. Si la descripción de cada documento es diferente, verá _Varios valores_ en el cuadro de descripción. Puede agregar la misma descripción para todos los documentos, pero no puede editar descripciones de documentos individuales al editar de forma masiva.
1. Realice los siguientes cambios con los formularios personalizados:

   <table>
    <tr>
    <td><strong>Añadir formularios</strong></td>
    <td>En el cuadro <strong>Agregar formulario personalizado</strong>, puede elegir entre Formularios adjuntos y Formularios que desea agregar. Los formularios adjuntos se encuentran en algunos de los documentos seleccionados, pero no en todos. Se muestra automáticamente en la ventana de edición un formulario adjunto a todo el documento seleccionado.  </td>
    </tr>
    <tr>
    <td><strong>Editar formularios</strong></td>
    <td>Edite los formularios personalizados adjuntos. La información que cambie sobrescribirá la información existente en los documentos individuales. Los campos con valores diferentes en los documentos se muestran como "Varios valores". </td>
    </tr>
    <tr>
    <td><strong>Reorganizar formularios</strong></td>
    <td>Haga clic en el formulario personalizado y arrástrelo para reorganizarlo.</td>
    </tr>
    </table>
1. Haga clic en **Guardar**.

</span>