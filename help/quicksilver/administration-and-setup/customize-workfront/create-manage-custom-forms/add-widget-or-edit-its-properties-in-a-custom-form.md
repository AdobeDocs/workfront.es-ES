---
title: Agregar o editar una imagen u otro widget de recursos en un formulario personalizado
description: Puede agregar o editar las propiedades de cualquiera de las siguientes utilidades de recursos, como imágenes, vídeos, archivos PDF y archivos Adobe XD, en un formulario personalizado. Resulta útil cuando necesita incluir contenido visual, como imágenes de marca, un vídeo instructivo o un prototipo interactivo para una aplicación que está diseñando.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 62a2f9a1-80de-40e7-9d8b-46ed9df083c1
source-git-commit: eeff0c8a3f7cbccd942c978d771d24f4cf9c425d
workflow-type: tm+mt
source-wordcount: '1325'
ht-degree: 1%

---

# Agregar o editar una imagen u otro widget de recursos en un formulario personalizado

Puede agregar o editar las propiedades de cualquiera de los siguientes widgets de recursos en un formulario personalizado:

* Imagen
* Vídeo
* archivo PDF
* Archivo Adobe XD

Resulta útil cuando necesita incluir contenido visual, como imágenes de marca, un vídeo instructivo o un prototipo interactivo para una aplicación que está diseñando.

Cuando un formulario personalizado que contiene un widget está adjunto a un objeto, los usuarios que trabajan con él pueden verlo en las siguientes áreas:

* El área Detalles del objeto (por ejemplo, para un proyecto, el área Detalles del proyecto)
* El cuadro Editar del objeto, si tiene el nuevo aspecto y presentación de la experiencia de Adobe Workfront (por ejemplo, los cuadros Editar proyecto y Editar tarea)

Actualmente, los usuarios no pueden ver el widget en las siguientes áreas: &#x200B;

* Listas e informes
* Inicio y resumen
* El cuadro Editar del objeto, si no tiene el aspecto y la presentación de la nueva experiencia de Adobe Workfront (por ejemplo, el cuadro Editar gasto)
* La aplicación móvil de Workfront


## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Agregar o editar un widget de recursos en un formulario personalizado

1. Empiece a trabajar en un formulario personalizado, tal como se describe en [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Con la variable **Añadir un campo** abra la pestaña , realice una de las siguientes acciones:

   * Si va a añadir un nuevo widget, seleccione **Imagen**, **PDF** o **Vídeo** para agregarlo en la parte inferior del formulario o arrástrelo donde desee en el formulario.

      ![](assets/add-widget.png)


   * Si desea agregar un widget que ya se haya agregado a otro formulario personalizado, haga clic en **Biblioteca de campos** y, a continuación, haga clic en el nombre del widget en la lista que aparece. Para obtener más información, consulte [Reutilizar un campo o un widget personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   * Si está editando un widget ya agregado al formulario personalizado, selecciónelo.

1. Escriba o edite cualquiera de las siguientes propiedades para el widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del widget. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: Evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>(Obligatorio) Este nombre es el modo en que el sistema identifica el widget.</p> <p>Cuando configura la utilidad por primera vez y escribe la etiqueta, el campo Nombre se rellena automáticamente para que coincida con ella. Sin embargo, los campos Etiqueta y Nombre no están sincronizados: esto le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p> <p><b>IMPORTANTE</b>: Aunque es posible hacerlo, le recomendamos que no cambie este nombre después de que usted u otros usuarios empiecen a usar el formulario personalizado en un widget. Si lo hace, el sistema ya no reconocerá el widget donde podría hacerse referencia a él en otras áreas de Workfront. </p> <p>Cada nombre de widget debe ser único en la instancia de Workfront de su organización. De este modo, puede reutilizar una que ya se haya creado para otro formulario personalizado. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dirección URL</td> 
      <td> <p>(Obligatorio) Escriba o pegue la dirección URL del widget donde se almacena en Internet.</p> 
      <p>Si está agregando un widget de vídeo, actualmente puede hacerlo agregando lo siguiente en el cuadro URL:</p> 
      <ul> 
      <li> <p>Vínculo de YouTube o Vimeo</p> </li> 
      <li> <p>Vínculo de vídeo de Google Drive</p> </li> 
      <li> <p>Vínculo a vídeo con extensión MP4 y MOV</p> </li> 
      <li> <p>Vínculo a vídeo ya cargado en el área Documentos de la instancia de Workfront. Para obtener instrucciones, consulte <a href="#add-a-video-widget-to-a-custom-form-from-the-documents-area" class="MCXref xref">Agregue un widget de vídeo a un formulario personalizado desde el área Documentos</a> en este artículo.</p> </li> 
      </ul> 
       </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instrucciones</td> 
      <td> <p>Escriba cualquier información adicional sobre el widget. Cuando los usuarios rellenen el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver una información que contenga la información que escriba aquí.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tamaño</td> 
      <td>Cambie el tamaño de visualización del widget según sea necesario.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Aplicar**.
1. Si desea seguir creando el formulario personalizado de otras formas, continúe con uno de los siguientes artículos:

   * [Colocación de campos y widgets personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Reutilizar un campo o un widget personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Reutilizar un campo personalizado calculado existente en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Agregar lógica de visualización y de omisión de lógica a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Obtener una vista previa y completar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)


## Agregar un archivo XD a un formulario personalizado

1. Empiece a trabajar en un formulario personalizado, tal como se describe en [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Con la variable **Añadir un campo** abrir ficha, seleccione **Adobe XD**.
1. Escriba o edite cualquiera de las siguientes propiedades para el widget:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del widget. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: Evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>(Obligatorio) Este nombre es el modo en que el sistema identifica el widget.</p> <p>Cuando configura la utilidad por primera vez y escribe la etiqueta, el campo Nombre se rellena automáticamente para que coincida con ella. Sin embargo, los campos Etiqueta y Nombre no están sincronizados: esto le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p> <p><b>IMPORTANTE</b>: Aunque es posible hacerlo, le recomendamos que no cambie este nombre después de que usted u otros usuarios empiecen a usar el formulario personalizado en un widget. Si lo hace, el sistema ya no reconocerá el widget donde podría hacerse referencia a él en otras áreas de Workfront. </p> <p>Cada nombre de widget debe ser único en la instancia de Workfront de su organización. De este modo, puede reutilizar una que ya se haya creado para otro formulario personalizado. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dirección URL</td> 
      <td> <p>(Obligatorio) Escriba o pegue un vínculo de prototipo de XD válido.</p> 
      <p>Nota: La configuración de Acceso a vínculos de la ficha Compartir de Adobe XD debe establecerse en Cualquiera que tenga el vínculo. De lo contrario, los usuarios no podrán ver el prototipo. 
   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Instrucciones</td> 
      <td> <p>(Opcional) Escriba cualquier información adicional sobre el widget. Cuando los usuarios rellenen el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver una información que contenga la información que escriba aquí.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tamaño</td> 
      <td>(Opcional) Cambie el tamaño de visualización del widget según sea necesario.</td> 
     </tr> 
    </tbody> 
   </table>

1. Si desea seguir creando el formulario personalizado de otras formas, continúe con uno de los siguientes artículos:

   * [Colocación de campos y widgets personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)
   * [Reutilizar un campo o un widget personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)
   * [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Reutilizar un campo personalizado calculado existente en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Agregar lógica de visualización y de omisión de lógica a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Obtener una vista previa y completar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

## Agregue un widget de vídeo a un formulario personalizado desde el área Documentos {#add-a-video-widget-to-a-custom-form-from-the-documents-area}

>[!IMPORTANT]
>
>Cuando agrega un vídeo a un formulario personalizado de esta forma, solo los permisos establecidos para el formulario personalizado se aplican al vídeo cuando los usuarios acceden al formulario en un objeto, no a los permisos establecidos para el vídeo en el área Documentos.

1. Vaya al vídeo en el área Documentos y genere una prueba para él, tal como se describe en [Crear una prueba interactiva para un sitio web u otro contenido web](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/generate-interactive-proof-for-website-or-other-web-content.md).
1. Abra la prueba.
1. Haga clic con el botón derecho en cualquier lugar del vídeo y seleccione **Copiar dirección de vídeo**.
1. En el formulario personalizado en el que va a añadir el widget de vídeo, pegue la dirección copiada en la **URL** en la ventana
