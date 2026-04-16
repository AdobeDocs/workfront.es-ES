---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Vincule contenido y carpetas con el Asesor de contenido con tecnología de Experience Manager Assets
description: Puede utilizar el Asesor de contenido para vincular contenido o carpetas de Experience Manager Assets a cualquier objeto de Adobe Workfront que admita documentos. El Asesor de contenido lleva la detección inteligente según el contexto directamente a Workfront, lo que le ayuda a encontrar rápidamente contenido relevante y aprobado.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: ab868314aef0924906ca69e82a10ece130484ba7
workflow-type: tm+mt
source-wordcount: '1226'
ht-degree: 22%

---

# Vinculación de contenido y carpetas con el Asesor de contenido de Experience Manager Assets

El Asesor de contenido lleva la detección inteligente según el contexto directamente a Workfront, lo que le ayuda a encontrar rápidamente contenido relevante y aprobado según el contexto. Con funciones como sugerencias inteligentes, representaciones de Dynamic Media y metadatos de recursos detallados, le permite evaluar y reutilizar contenido de forma eficaz sin salir de Workfront, lo que acelera la creación de contenido y mantiene la coherencia de la marca.

Puede utilizar el Asesor de contenido para vincular contenido y carpetas de Experience Manager Assets a Workfront. Una vez enlazado, puede ver y administrar el contenido en Workfront, y los cambios realizados en el contenido en Experience Manager Assets se reflejarán en Workfront.

>[!IMPORTANT]
>
>Si su organización rechaza firmar el acuerdo GenAI Rider, puede seguir utilizando el Asesor de contenido para elegir recursos y carpetas en Experience Manager Assets, pero no tendrá acceso a funciones con tecnología de IA, como Búsqueda por IA, sugerencias inteligentes o análisis de informes de campaña.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p> Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencias de Adobe Workfront</td> 
   <td> 
   <p>Colaborador o superior</p> 
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Productos adicionales</td> 
   <td>Debe tener Experience Manager as a Cloud Service o Assets Essentials, además de estar añadido al producto como usuario en Admin Console.</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Permisos de Experience Manager</td> 
    <td>Debe tener acceso de escritura a la carpeta.</td> 
   </tr>
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a documentos</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Acceso de visualización o superior</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de empezar:

* El administrador de Workfront debe configurar una integración de Experience Manager. Para obtener más información, consulte [Configuración de la integración de Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

* Para utilizar las sugerencias inteligentes o la funcionalidad de los informes de campaña, debe firmar un GenAI Rider. Para obtener más información, consulte [Usar el Asesor de contenido para obtener acceso al contenido de AEM en las aplicaciones de Adobe](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search).



## Vinculación de contenido desde Experience Manager Assets con el Asesor de contenido

Ahora puede utilizar el Asesor de contenido para vincular contenido de Experience Manager Assets directamente en Workfront. El Asesor de contenido no está disponible para Assets Essentials.

Para vincular contenido:

1. Vaya al área de **Documentos** de Workfront donde desea añadir el documento.
1. Seleccione **Añadir nuevo** y luego, la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente Experience Manager Assets.

1. Con el Asesor de contenido, puede:


   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>Busque recursos mediante la Búsqueda por IA.</strong> Use la búsqueda basada en IA que entienda el significado y la intención detrás de las consultas y que admita varios idiomas, errores tipográficos y sinónimos.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">Búsqueda por IA para una detección de recursos más inteligente</a>.</td>
      </tr>
      <tr>
         <td><strong>Ver sugerencias inteligentes basadas en el contexto y la intención.</strong> Descubra recursos que se alinean con sus necesidades de contenido mediante recomendaciones según el contexto desde la aplicación host de Adobe.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">Sugerencias inteligentes basadas en el contexto y la intención</a>.</td>
      </tr>
      <tr>
         <td><strong>Cargue un informe de campaña para descubrir los recursos relevantes.</strong> Cargar un documento de resumen de campaña de PDF, DOCX o TXT para que el Asesor de contenido pueda analizarlo y recomendar recursos relevantes.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">Informes de Campaign para descubrir recursos relevantes</a>.</td>
      </tr>
      <tr>
         <td><strong>Ver y seleccionar representaciones de recursos de Dynamic Media.</strong> Examine representaciones optimizadas para canales, incluidos ajustes preestablecidos de imagen, recortes inteligentes y tipos de formato, y aplique modificadores de Dynamic Media para obtener una vista previa de los ajustes en tiempo real.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Representaciones de recursos de Dynamic Media disponibles para usar</a>.</td>
      </tr>
      <tr>
         <td><strong>Aplicar modificadores de Dynamic Media a las representaciones.</strong> Agregue modificadores para transformar las representaciones de recursos en tiempo real y previsualice los resultados antes de seleccionar una representación para la aplicación host.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Representaciones de recursos de Dynamic Media disponibles para usar</a>.</td>
      </tr>
      <tr>
         <td><strong>Descubrir y examinar fragmentos de contenido.</strong>: busque a través de fragmentos de contenido, vea vistas previas de miniaturas activas, compruebe el estado (Borrador, Modificado o Publicado) e inspeccione las propiedades, referencias y variaciones detalladas.</td>
         <td>Para obtener más información, vea <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Descubrimiento de fragmentos de contenido</a>.</td>
      </tr>
      <tr>
         <td><strong>Acceder a metadatos de recursos.</strong>: revise las propiedades del recurso, como el título, la descripción, el formato, el tamaño y otras pestañas de metadatos (Producto, Campaña, Etiquetas) compatibles con la vista de Assets.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Acceder a metadatos de recursos compatibles con la vista de Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Filtre recursos mediante filtros predefinidos.</strong> Restringir los resultados de los recursos mediante filtros como Tipo de archivo, Formato de archivo, Estado del recurso, Tamaño de archivo, Anchura de imagen, Altura de imagen, Fecha de modificación y Fecha de creación.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Filtros de acceso compatibles con la vista de Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Guardar y reutilizar búsquedas.</strong>: para crear búsquedas guardadas, especifique un término de búsqueda y opciones de filtro y, a continuación, vuelva a utilizarlas en Experience Manager Assets y otras aplicaciones de Adobe.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">Acceder y reutilizar búsquedas recientes y guardadas</a>.</td>
      </tr>
      <tr>
         <td><strong>Busque recursos en las colecciones y entre ellas.</strong>: buscar recursos o colecciones en todas las colecciones, o limitar la búsqueda a una colección específica.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">Buscar recursos en las colecciones y entre ellas</a>.</td>
      </tr>
   </tbody>
   </table>


### Vincular una nueva versión de Experience Manager Assets con el Asesor de contenido

Puede extraer nuevo contenido de Experience Manager Assets o Assets Essentials y añadirlo a un recurso existente como una nueva versión. Si el documento ya está vinculado y se agrega una nueva versión en Experience Manager Assets o Assets Essentials, la nueva versión aparece automáticamente en Workfront.

Para vincular una nueva versión:

1. Vaya al área de **Documentos** de Workfront donde desea añadir el documento.
1. Seleccione el recurso que desea reemplazar con una nueva versión. No puede crear una nueva versión de un recurso en una carpeta vinculada.
1. Seleccione **Añadir nuevo**> **Versión** y, a continuación, seleccione la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente a Experience Manager Assets.

1. Seleccione el contenido que desea vincular:

   * Seleccione la pestaña Assets para examinar recursos, carpetas o colecciones en Experience Manager Assets o Assets Essentials.

     ![Asesor de contenido](assets/content-advisor-full.png)

   * Los fragmentos de contenido no admiten versiones. Si selecciona un fragmento de contenido, la nueva versión reemplazará el fragmento de contenido existente en lugar de crear una nueva versión.

1. Haga clic en **Seleccionar**.

## Vincular una carpeta desde Experience Manager Assets con el Asesor de contenido

Los permisos para ver recursos individuales dentro de una carpeta dependen de los permisos de Experience Manager Assets.

Para vincular una carpeta:

1. Vaya al área de **Documentos** de Workfront donde desee colocar la carpeta.
1. Seleccione **Añadir nuevo** y luego seleccione la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente a Experience Manager Assets.

1. Haga clic en **Assets** > **Archivos y carpetas**.

1. Haga clic en el icono **Filtrar** y, a continuación, en la sección **Tipo de recurso**, elija **Carpetas**.

1. Seleccione la carpeta que desea vincular.

1. Haga clic en **Seleccionar**.

## Consideraciones

* La funcionalidad de Asesor de contenido no está disponible para objetos que utilicen Adobe Enterprise Storage. Si su organización utiliza Adobe Enterprise Storage, aún puede vincular recursos y carpetas desde Experience Manager Assets o Assets Essentials, pero no tendrá acceso a las funciones del Asesor de contenido, como Búsqueda por IA, sugerencias inteligentes o representaciones de Dynamic Media. Para obtener más información, consulte [Usar Adobe Experience Manager con la integración de Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* La funcionalidad de Asesor de contenido no está disponible para Assets Essentials. Para vincular recursos y carpetas desde Assets Essentials, consulte [Vincular recursos y carpetas desde Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/link-to-aem-essentials.md).

* Los campos de metadatos se asignan por primera vez al enviar un recurso de Workfront a Experience Manager Assets. Si el administrador de Workfront ha habilitado la sincronización de metadatos de objetos, los campos permanecen actualizados si se modifican en alguna de las aplicaciones.
