---
product-area: documents
navigation-topic: approvals
title: Quitar aprobadores o revisores de un flujo de trabajo de aprobación de documentos
description: Puede quitar aprobadores o revisores individuales de un documento.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6877ee90-9a70-4616-98f4-4b0ff932d79a
source-git-commit: 3fd4d18e1be14cc27b3b39d4abf399ec26ddcd51
workflow-type: tm+mt
source-wordcount: '854'
ht-degree: 43%

---

# Quitar aprobadores o revisores de un flujo de trabajo de aprobación de documentos

<span class="preview">La información resaltada en esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

Puede quitar aprobadores o revisores individuales de un recurso o documento después de haberlos asignado.

>[!IMPORTANT]
>
>El contenido de este artículo hace referencia a la funcionalidad actualizada de aprobación de documentos que solo está disponible para cuentas específicas. Para obtener información sobre los procesos de aprobación estándar, consulte los artículos enumerados en [Aprobaciones de trabajo](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

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
   <p>Revisión o superior</p>
   <p>Si utiliza la integración de Frame.io, debe tener una licencia Standard para crear flujos de trabajo de aprobación.</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de visualización o superior a Proyectos, Tareas, Problemas, Plantillas, Portafolios, Programas, Informes, Paneles de control y Calendarios, Documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de administración al objeto asociado con el acceso de solicitud o la aprobación </p>  </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++


## Eliminar aprobadores o revisores de la página Detalles del documento en el entorno de producción

1. Vaya a la página del documento haciendo clic en su nombre y, a continuación, seleccione la versión del documento cuya aprobación desea eliminar en el menú desplegable de la versión. La última versión está seleccionada de forma predeterminada.

1. Seleccione **Aprobaciones** en el panel izquierdo.

1. Pase el ratón sobre el nombre del aprobador o revisor que quiera eliminar y luego haga clic en el icono **Eliminar** ![Eliminar icono](../assets/delete.png) que aparece después de su nombre.

   La solicitud de aprobación o revisión se elimina y el aprobador recibe una notificación que le informa de que ya no necesita su aprobación. También se elimina su acceso compartido relacionado con la aprobación.

1. (Opcional) Para devolver un aprobador a un revisor en lugar de eliminarlo por completo, desmarque la casilla de verificación **Aprobador** junto con su nombre.

1. Repita el paso anterior para eliminar los aprobadores o revisores adicionales.

## Quitar aprobadores o revisores del resumen del documento en el entorno de producción

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.

1. Haga clic en el documento que necesita y se abrirá el panel Resumen del documento para ese documento.

1. Seleccione la versión del documento para la que desea quitar un aprobador o revisor en el menú desplegable de la versión. La última versión está seleccionada de forma predeterminada.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** del panel Resumen del documento. Pase el ratón sobre el nombre del aprobador o revisor que quiera eliminar y luego haga clic en el icono **Eliminar** ![Eliminar icono](../assets/delete.png) que aparece después de su nombre.

   La solicitud de aprobación o revisión se elimina y el aprobador recibe una notificación que le informa de que ya no necesita su aprobación. También se elimina su acceso compartido relacionado con la aprobación.

1. (Opcional) Para devolver un aprobador a un revisor en lugar de eliminarlo por completo, desmarque la casilla de verificación **Aprobador** junto con su nombre.

1. Repita el paso anterior para eliminar los aprobadores o revisores adicionales.


<div class="preview">

## Elimine aprobadores o revisores de un flujo de trabajo de aprobación en su entorno de vista previa en el área de documentos heredados

Si su organización está en el almacenamiento de Workfront, verá el área de documentos heredados al acceder a documentos en Workfront. Para obtener más información sobre el almacenamiento de Workfront, consulte [Almacenamiento de Workfront frente al almacenamiento empresarial de Adobe](/help/quicksilver/review-and-approve-work/esm-overview.md#workfront-storage-vs-adobe-enterprise-storage).

Para eliminar aprobadores o revisores de un flujo de trabajo de aprobación:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en el documento que necesita y se abrirá el panel Resumen del documento para ese documento.

1. Desplácese hacia abajo hasta la sección **Aprobaciones** del panel Resumen del documento.

1. Haga clic en **Editar flujo de trabajo**.

1. Busque el participante que desea eliminar y haga clic en el icono **Eliminar** que aparece junto a su nombre.

   La solicitud de aprobación o revisión se elimina y el aprobador recibe una notificación que le informa de que ya no necesita su aprobación. También se elimina su acceso compartido relacionado con la aprobación.

   ![editar flujo de trabajo de aprobación](assets/edit-approval-in-legacy.png)

1. (Opcional) Para cambiar la función de un aprobador a un revisor o viceversa, haga clic en el menú desplegable situado junto al nombre de usuario y seleccione la nueva función.

1. Repita el paso anterior para eliminar los aprobadores o revisores adicionales.

</div>


## Eliminar aprobadores o revisores a un flujo de trabajo de aprobación en la nueva área de documento

Si su organización utiliza el almacenamiento empresarial, verá el área de nuevos documentos al acceder a ellos en Workfront. Para obtener más información acerca del almacenamiento empresarial, vea [Información general sobre el almacenamiento empresarial](/help/quicksilver/review-and-approve-work/esm-overview.md).

Para crear un flujo de trabajo de aprobación:

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos** en el panel izquierdo.

1. Haga clic en el documento y luego en el icono **Aprobaciones** que encontrará a la derecha de la página.

   ![Agregar aprobadores en el resumen del documento](assets/approvals-icon-new.png)


1. Haga clic en **Editar flujo de trabajo**.

1. Busque el participante que desea eliminar y haga clic en el icono **Eliminar** que aparece junto a su nombre.

   La solicitud de aprobación o revisión se elimina y el aprobador recibe una notificación que le informa de que ya no necesita su aprobación.

1. (Opcional) Para cambiar la función de un aprobador a un revisor o viceversa, haga clic en el menú desplegable situado junto al nombre de usuario y seleccione la nueva función.

1. Repita el paso anterior para eliminar los aprobadores o revisores adicionales.

   ![quitar participantes de una fase](assets/add-or-remove-participants.png)
1. Haga clic en **Guardar**.