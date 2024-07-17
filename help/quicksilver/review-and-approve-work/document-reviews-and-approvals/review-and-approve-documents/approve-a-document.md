---
product-area: projects
navigation-topic: approvals
title: Aprobación de un documento en Workfront
description: Si se le asigna como aprobador de un documento, puede tomar su decisión de aprobación de varias formas.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 5490973b-99a7-4790-9d89-bf8f16ff5765
source-git-commit: 50a38ad915b639bf742a4b1f18bcb4da88e07d63
workflow-type: tm+mt
source-wordcount: '1067'
ht-degree: 0%

---

# Aprobación de un documento en Workfront

Si se le asigna como aprobador de un documento, puede tomar su decisión de aprobación de varias formas.

Para obtener información acerca de cómo crear una nueva aprobación de documento, vea [Crear una solicitud de revisión o aprobación de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

>[!IMPORTANT]
>
>El contenido de este artículo hace referencia a la funcionalidad actualizada de aprobación de documentos que solo está disponible para cuentas específicas. Para obtener información sobre los procesos de aprobación estándar, consulte los artículos enumerados en [Aprobaciones de trabajo](/help/quicksilver/review-and-approve-work/manage-approvals/manage-approvals.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Revisar o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de visualización o superior a los objetos asociados con las aprobaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Ver permisos superiores a los objetos asociados con las aprobaciones o</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Aprobar un documento desde Inicio

1. Haga clic en el icono **Inicio** ![](../assets/home-icon-30x29.png) en la esquina superior izquierda de Adobe Workfront.

   >[!NOTE]
   >
   >El administrador de Workfront puede realizar los siguientes cambios en el icono Inicio de su entorno:
   >
   >* Sustitúyala por una imagen personalizada para ilustrar su organización. En este caso, el icono tendrá un aspecto diferente al que se muestra en este artículo.
   >
   >* Reemplace la página vinculada a ella por una página diferente. En este caso, haga clic en **Menú principal** ![](../assets/main-menu-icon.png) en la esquina superior derecha de la página y, a continuación, haga clic en **Inicio**.

1. Haga clic en **Filtros** en la parte superior izquierda de la página y asegúrese de que **Aprobaciones** esté marcado.

   Todos los elementos de trabajo que requieren su aprobación se muestran en la lista.

   >[!NOTE]
   >
   >Las aprobaciones asignadas a roles o grupos de trabajos no aparecen en Inicio. Las aprobaciones asignadas a los equipos se muestran en la agrupación de solicitudes de equipo en la Lista de trabajos.

1. Haga clic en la aprobación del documento en la lista para la que desea tomar una decisión de aprobación. La información sobre la aprobación aparecerá en la parte derecha de la página.

1. Haga clic en una de las dos opciones de aprobación siguientes en la esquina superior derecha de la página:

   * El menú desplegable **Aprobar** contiene dos opciones:

      * **Aprobar** indica que no se necesitan cambios para esta versión del documento y que se ha dado la aprobación.

      * **Aprobar con cambios** indica que aún se requieren algunos cambios pequeños en el documento, pero la aprobación se da con la condición de que se realicen dichos cambios. Si selecciona esta opción, aparecerá una ventana que contiene un cuadro de texto denominado **Pasos siguientes** en el que puede especificar qué cambios son necesarios para que se apruebe el documento. Puede introducir esa información y hacer clic en **Agregar mensaje**, o bien hacer clic en **Omitir** para enviar la decisión de aprobación sin información adicional.

   * **Necesita trabajo** indica que la versión del documento no está aprobada y requiere cambios significativos.

   Tenga en cuenta lo siguiente cuando visualice aprobaciones de documentos en Inicio:

   * El nombre del usuario que solicitó la aprobación se muestra encima del nombre del documento en Inicio con el texto &quot;*El usuario A* desea su aprobación el...&quot;, así como en **Enviado por** en la información de aprobación que se muestra a la derecha una vez seleccionada una aprobación.

   * Después de tomar una decisión sobre una aprobación, la aprobación permanece en la pestaña Mis aprobaciones con el texto &quot;Decisión tomada&quot; hasta que haga clic en el botón **Actualizar** o hasta que actualice la página del explorador.

## Aprobar un documento desde la página de documento

1. Vaya a la página del documento haciendo clic en su nombre.

1. Seleccione la versión del documento que está pendiente de aprobación en el menú desplegable de versión situado junto al nombre del documento. La última versión se selecciona de forma predeterminada.

   Si la versión seleccionada actualmente del documento tiene una aprobación pendiente, los botones de decisión de aprobación se muestran en la esquina superior derecha de la página; si otras versiones del documento tienen aprobaciones pendientes para usted, el menú desplegable de la versión muestra un punto rojo.

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Haga clic en una de las dos opciones de aprobación siguientes en la esquina superior derecha de la página:

   * El menú desplegable **Aprobar** contiene dos opciones:

      * **Aprobar** indica que no se necesitan cambios para esta versión del documento y que se ha dado la aprobación.

      * **Aprobar con cambios** indica que aún se requieren algunos cambios pequeños en el documento, pero la aprobación se da con la condición de que se realicen dichos cambios. Si selecciona esta opción, aparecerá una ventana que contiene un cuadro de texto denominado **Pasos siguientes** en el que puede especificar qué cambios son necesarios para que se apruebe el documento. Puede introducir esa información y hacer clic en **Agregar mensaje**, o bien hacer clic en **Omitir** para enviar la decisión de aprobación sin información adicional.

   * **Necesita trabajo** indica que la versión del documento no está aprobada y requiere cambios significativos.

## Aprobar un documento desde el panel Resumen del documento

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.

1. Haga clic en el documento que necesita su aprobación y se abrirá el panel Resumen del documento.

1. Seleccione la versión del documento que desee revisar en el menú desplegable de la versión. La última versión se selecciona de forma predeterminada.

   Si la versión seleccionada actualmente del documento tiene una aprobación pendiente, los botones de decisión de aprobación se muestran en la esquina superior derecha del panel Resumen del documento; si otras versiones del documento tienen aprobaciones pendientes para usted, el menú desplegable de la versión muestra un punto rojo.

   <!--
   ![](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Haga clic en una de las dos opciones de aprobación siguientes en la esquina superior derecha del panel Resumen del documento:

   * El menú desplegable **Aprobar** contiene dos opciones:

      * **Aprobar** indica que no se necesitan cambios para esta versión del documento y que se ha dado la aprobación.

      * **Aprobar con cambios** indica que aún se requieren algunos cambios pequeños en el documento, pero la aprobación se da con la condición de que se realicen dichos cambios. Si selecciona esta opción, aparecerá una ventana que contiene un cuadro de texto denominado **Pasos siguientes** en el que puede especificar qué cambios son necesarios para que se apruebe el documento. Puede introducir esa información y hacer clic en **Agregar mensaje**, o bien hacer clic en **Omitir** para enviar la decisión de aprobación sin información adicional.

   * **Necesita trabajo** indica que la versión del documento no está aprobada y requiere cambios significativos.