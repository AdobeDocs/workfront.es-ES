---
product-area: projects
navigation-topic: approvals
title: Aprobar un documento en Workfront
description: Si se le asigna a un documento en calidad de aprobador, puede tomar su decisión de aprobación de varias formas.
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 5490973b-99a7-4790-9d89-bf8f16ff5765
source-git-commit: cd0214917620e0b147d0da3402ea2d34e28bc9c3
workflow-type: tm+mt
source-wordcount: '1180'
ht-degree: 73%

---

# Aprobar un documento en Workfront

Si se le asigna a un documento en calidad de aprobador, puede tomar su decisión de aprobación de varias formas.

Para obtener información sobre la creación de una nueva aprobación de documento, consulte [Crear una solicitud de revisión o aprobación de documento](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md).

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
   <td role="rowheader">paquete de Adobe Workfront</td> 
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
   <td> <p>Vista o acceso superior a los objetos asociados con las aprobaciones</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Vista o permisos superiores a los objetos asociados a aprobaciones</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Aprobar un documento desde Inicio

1. Haga clic en el icono **Inicio** ![Icono de inicio](../assets/home-icon-30x29.png) en la esquina superior izquierda de Adobe Workfront.

   >[!NOTE]
   >
   >El administrador de Workfront puede realizar los siguientes cambios en el icono de Inicio de su entorno:
   >
   >* Sustitúyalo por una imagen personalizada para ilustrar su organización. En este caso, el icono tendrá un aspecto diferente al que se muestra en este artículo.
   >
   >* Reemplace la página vinculada por una página diferente. En este caso, haga clic en el **icono del menú principal** ![menú principal](../assets/main-menu-icon.png) en la esquina superior derecha de la página y, a continuación, haga clic en **Inicio**.

1. Haga clic en **Filtros** en la parte superior izquierda de la página y asegúrese de que **Aprobaciones** esté marcado.

   Todos los elementos de trabajo que requieran su aprobación se mostrarán en la lista.

   >[!NOTE]
   >
   >* Las aprobaciones asignadas a roles o grupos de trabajos no aparecen en Inicio.
   >* Las aprobaciones asignadas a los equipos se muestran en el widget Mis aprobaciones de cada miembro del equipo individual en Inicio.

1. Haga clic en la aprobación del documento de la lista para el que desea tomar una decisión de aprobación. La información sobre la aprobación aparecerá en la parte derecha de la página.

1. Haga clic en una de las dos opciones de aprobación siguientes que aparecen en la esquina superior derecha de la página:

   * El menú desplegable **Aprobar** contiene dos opciones:

      * **Aprobar** indica que no se necesitan cambios para esta versión del documento y que se ha dado la aprobación.

      * **Aprobar con cambios** indica que aún se requieren algunos cambios pequeños en el documento, pero se da la aprobación con la condición de que se realicen dichos cambios. Si selecciona esta opción, aparecerá una ventana que contiene un cuadro de texto denominado **Pasos siguientes** en el que podrá especificar qué cambios son necesarios para que se apruebe el documento. Puede introducir esa información y hacer clic en **Añadir mensaje**, o bien hacer clic en **Omitir** para enviar la decisión de aprobación sin información adicional.

   * **Necesita trabajo** indica que la versión del documento no está aprobada y requiere cambios significativos.

   Tenga en cuenta lo siguiente cuando vea aprobaciones de documentos en Inicio:

   * El nombre del usuario que ha solicitado la aprobación se muestra en Inicio, encima del nombre del documento, con el texto “El *usuario A* desea su aprobación el...”, así como en **Enviado por** en la información de aprobación que aparece a la derecha una vez seleccionada una aprobación.

   * Después de tomar una decisión sobre una aprobación, la aprobación permanecerá en la pestaña Mis aprobaciones con el texto “Decisión tomada” hasta que haga clic en el botón **Actualizar** o hasta que actualice la página del explorador.

## Aprobar un documento desde la página de documento

1. Vaya a la página del documento haciendo clic en el nombre de este.

1. Seleccione la versión del documento que está pendiente de aprobación en el menú desplegable de versión situado junto al nombre del documento. La última versión se selecciona de forma predeterminada.

   Si tiene una aprobación pendiente en la versión seleccionada actualmente del documento, los botones de decisión de aprobación se mostrarán en la esquina superior derecha de la página; si tiene aprobaciones pendientes en otras versiones del documento, el menú desplegable de versión mostrará un punto rojo.

   <!--
   ![Version dropdown with red dot](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
   -->

1. Haga clic en una de las dos opciones de aprobación siguientes que aparecen en la esquina superior derecha de la página:

   * El menú desplegable **Aprobar** contiene dos opciones:

      * **Aprobar** indica que no se necesitan cambios para esta versión del documento y que se ha dado la aprobación.

      * **Aprobar con cambios** indica que aún se requieren algunos cambios pequeños en el documento, pero se da la aprobación con la condición de que se realicen dichos cambios. Si selecciona esta opción, aparecerá una ventana que contiene un cuadro de texto denominado **Pasos siguientes** en el que podrá especificar qué cambios son necesarios para que se apruebe el documento. Puede introducir esa información y hacer clic en **Añadir mensaje**, o bien hacer clic en **Omitir** para enviar la decisión de aprobación sin información adicional.

   * **Necesita trabajo** indica que la versión del documento no está aprobada y requiere cambios significativos.

## Aprobar un documento desde el panel Resumen del documento

1. Vaya al proyecto, tarea o problema que contiene el documento y, a continuación, seleccione **Documentos**.

1. Haga clic en el documento que necesita su aprobación y se abrirá el panel Resumen del documento.

1. Seleccione la versión del documento que desee revisar en el menú desplegable de la versión. La última versión se selecciona de forma predeterminada.

   Si la versión seleccionada actualmente del documento tiene una aprobación pendiente, los botones de decisión de aprobación se muestran en la esquina superior derecha del panel Resumen del documento; si otras versiones del documento tienen aprobaciones pendientes para usted, el menú desplegable Versión muestra un punto rojo.
<!--
   ![Version dropdown with red dot](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/assets/version-dropdown-red-dot.png)
 -->
1. Haga clic en una de las dos opciones de aprobación siguientes en la esquina superior derecha del panel Resumen del documento:

   * El menú desplegable **Aprobar** contiene dos opciones:

      * **Aprobar** indica que no se necesitan cambios para esta versión del documento y que se ha dado la aprobación.

      * **Aprobar con cambios** indica que aún se requieren algunos cambios pequeños en el documento, pero se da la aprobación con la condición de que se realicen dichos cambios. Si selecciona esta opción, aparecerá una ventana que contiene un cuadro de texto denominado **Pasos siguientes** en el que podrá especificar qué cambios son necesarios para que se apruebe el documento. Puede introducir esa información y hacer clic en **Añadir mensaje**, o bien hacer clic en **Omitir** para enviar la decisión de aprobación sin información adicional.

   * **Necesita trabajo** indica que la versión del documento no está aprobada y requiere cambios significativos.


## Aprobar un documento desde el visor de pruebas

Para revisar y aprobar un documento:

1. Vaya a la notificación de correo electrónico de revisión y haga clic en **Ir a revisión**.

1. Una vez que estés en Workfront, haz clic en **Ir a la revisión**.

1. Revise el contenido y agregue cualquier comentario o marca. Para obtener más información acerca de cómo usar el visor de revisión, vea [Revisar pruebas en Adobe Workfront: índice de artículos](/help/quicksilver/review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. Elija una de las siguientes decisiones:

   * **Aprobar**: el documento no necesita cambios y está listo para usarse.
   * **Aprobar con cambios**: el documento necesita cambios y está listo para usarse una vez que se hayan realizado. No se requiere una aprobación adicional.
   * **Necesita trabajo**: el documento necesita cambios y no está listo para usarse. Una vez realizados los cambios especificados, el documento debe cargarse como una nueva versión y pasar por otra ronda de aprobaciones. Para obtener más información sobre cómo cargar una nueva versión, consulte [Crear una nueva versión según sea necesario](#create-a-new-version-as-needed) en este artículo.

Una vez que tome una decisión, se notifica al propietario del documento por correo electrónico.


