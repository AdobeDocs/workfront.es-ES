---
product-area: documents
navigation-topic: approvals
title: Administración de aprobaciones agrupadas
description: Puede añadir o quitar participantes y documentos en una aprobación agrupada sin interrumpir el flujo de trabajo del resto del grupo.
author: Courtney
feature: Work Management, Digital Content and Documents
source-git-commit: 9459c6251b2576207e1766d94e6cb634f65f1f68
workflow-type: tm+mt
source-wordcount: '1030'
ht-degree: 5%
---

# Administración de aprobaciones agrupadas

Una aprobación agrupada agrupa varios documentos en un solo flujo de trabajo de aprobación, por lo que todos los documentos se mueven por las mismas fases juntos en lugar de requerir una aprobación independiente por documento. Puede añadir o quitar participantes y documentos en una aprobación agrupada activa sin volver a crear el flujo de trabajo.

Las aprobaciones agrupadas admiten los modos Básico y Avanzado, varias etapas y rutas paralelas del mismo modo que las aprobaciones de un solo recurso. Para obtener más información, consulte [Crear un flujo de trabajo de aprobación de documentos](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>Si su organización utiliza el almacenamiento en la nube de Adobe, verá la nueva área Documentos al acceder a documentos en Workfront. Las aprobaciones agrupadas solo están disponibles en la nueva área de Documentos. Para obtener más información sobre el almacenamiento en la nube de Adobe, consulte [Información general sobre el almacenamiento en la nube de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto">
 <col>
 <col>
 <tbody>
  <tr>
   <td role="rowheader">Paquete de Adobe Workfront</td>
   <td> <p>Cualquier paquete de flujo de trabajo para administrar aprobaciones mediante el almacenamiento en la nube de Adobe</p> </td>
  </tr>
  <tr>
   <td role="rowheader">Licencia de Adobe Workfront</td>
   <td>
   <p>Colaborador o superior</p>
   <p>Revisión o superior</p>
   <p>Si utiliza la integración de Frame.io, debe tener una licencia Standard para crear flujos de trabajo de aprobación.</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader">Configuraciones de nivel de acceso</td>
   <td> <p>Acceso de visualización o superior a Proyectos, Tareas, Problemas, Plantillas, Portafolios, Programas, Informes, Tableros, Calendarios y Documentos</p></td>
  </tr>
  <tr>
   <td role="rowheader">Permisos de objeto</td>
   <td> <p>Administrar el acceso al objeto asociado con la solicitud o aprobación</p></td>
  </tr>
 </tbody>
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agregar participantes a una aprobación agrupada activa

Puede agregar aprobadores o revisores a una aprobación agrupada mientras una fase está activa, sin interrumpir las aprobaciones que ya están en curso.

Para agregar participantes a una aprobación agrupada activa:

1. Vaya al proyecto, tarea o problema que contiene la aprobación agrupada y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en cualquier documento del grupo y luego en el icono **Aprobaciones** que hay a la derecha de la página.

   ![Agregar aprobadores en el resumen del documento](assets/approvals-icon-new.png)

1. Haga clic en **Editar flujo de trabajo**.

1. Escriba el usuario, equipo o correo electrónico en el campo **Agregar nombres o correos electrónicos** de la etapa activa.

1. Para cada persona que agregue, elija si es un aprobador o un revisor.

1. Haga clic en **Guardar**.

   Los nuevos participantes ven todas las aprobaciones abiertas en el grupo de su cola. No ven las decisiones que se tomaron antes de agregarse, por lo que aún necesitan completar todas las aprobaciones abiertas actualmente por sí mismas.

## Quitar participantes de una aprobación agrupada activa

Puede quitar aprobadores o revisores de una aprobación agrupada mientras una fase está activa. Los participantes eliminados dejan inmediatamente de ver las aprobaciones del grupo en la cola, pero las decisiones que ya han tomado se mantienen y no se restablecen.

Para eliminar participantes de una aprobación agrupada activa:

1. Vaya al proyecto, tarea o problema que contiene la aprobación agrupada y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en cualquier documento del grupo y luego en el icono **Aprobaciones** que hay a la derecha de la página.

   ![Quitar aprobadores en el resumen del documento](assets/approvals-icon-new.png)

1. Haga clic en **Editar flujo de trabajo**.

1. Busque el participante que desea eliminar de la fase activa y, a continuación, haga clic en el icono **Quitar** que aparece junto a su nombre.

1. Haga clic en **Guardar**.

## Agregar documentos a una aprobación agrupada

Puede añadir documentos a una aprobación agrupada hasta que se bloquee su primera fase. Una vez que se bloquea el primer paso, ya no puede añadir documentos.

Para agregar un documento a una aprobación agrupada:

1. Vaya al proyecto, tarea o problema que contiene la aprobación agrupada y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en cualquier documento del grupo y luego en el icono **Aprobaciones** que hay a la derecha de la página.

1. Haga clic en **Editar flujo de trabajo** y luego haga clic en la ficha **Documentos**.

1. Seleccione el documento o documentos que desee agregar al grupo.

1. Haga clic en **Guardar**.

   Se notifica a todos los participantes en el grupo que se ha añadido un documento adicional para que lo revisen.

## Eliminación de documentos de una aprobación agrupada

Puede quitar un documento de una aprobación agrupada en cualquier punto del flujo de trabajo. El documento eliminado se convierte en su propia aprobación independiente y mantiene todas sus decisiones, comentarios e historial existentes sin reiniciar. Dado que el documento ya contiene una decisión de aprobación, no puede volver a agregarlo a una aprobación agrupada posteriormente.

Para eliminar un documento de una aprobación agrupada:

1. Vaya al proyecto, tarea o problema que contiene la aprobación agrupada y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en el documento que desee quitar y, a continuación, haga clic en el icono **Aprobaciones** que aparece a la derecha de la página.

1. Haga clic en **Editar flujo de trabajo** y luego haga clic en la ficha **Documentos**. El documento seleccionado está anclado en la parte superior de la lista y ya está marcado.

1. Borre la selección del documento que desea quitar del grupo.

1. Haga clic en **Guardar**.

   >[!NOTE]
   >
   >El estado de aprobación del documento permanece visible y sin cambios desde el momento en que se eliminó. La vista de aprobación agrupada se actualiza para reflejar los documentos restantes del grupo.


## Resolver una decisión &quot;Necesita trabajo&quot; en un solo documento en una aprobación agrupada de varias fases

En una aprobación agrupada de varias fases, todos los documentos de una fase deben alcanzar una decisión antes de que el grupo pueda pasar a la siguiente fase. Si un documento está marcado como **Necesita trabajo**, no puede avanzar con el resto del grupo, por lo que debe eliminarse manualmente del grupo para que la fase avance.

Al eliminar el documento del grupo, se convierte en su propia aprobación independiente y mantiene todas sus decisiones, comentarios e historial existentes sin reiniciar. Puede añadir el documento revisado como una nueva versión a la aprobación independiente o crear una nueva aprobación agrupada con él.

Para resolver una decisión de &quot;Necesita trabajo&quot;:

1. Elimine del grupo el documento marcado **Necesita trabajo**. Para obtener más información, vea [Quitar documentos de una aprobación agrupada](#remove-documents-from-a-grouped-approval). El documento eliminado se convierte en su propia aprobación independiente y conserva sus decisiones, comentarios e historial existentes.

1. Una vez actualizado el documento, cárguelo como una nueva versión y vuelva a solicitar la aprobación o agréguelo como parte de un nuevo grupo.

   Para obtener más información, consulte

   * [Cargar una nueva versión del documento y solicitar una aprobación](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/upload-new-doc-version.md)
   * [Crear un flujo de trabajo de aprobación de documentos](create-a-document-approval.md)
   * [Creación de una aprobación agrupada](create-a-grouped-approval.md)


## Limitaciones conocidas

Hay un problema temporal de sincronización con Frame.io cuando se añaden o eliminan documentos en una aprobación agrupada. Los cambios no se reflejarán en Frame.io hasta la próxima vez que se sincronice el documento.