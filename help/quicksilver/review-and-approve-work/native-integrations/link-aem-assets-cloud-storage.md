---
product-area: documents;workfront-integrations
navigation-topic: native-integrations
title: Vinculación de recursos de Experience Manager Assets con Adobe Cloud Storage
description: Si su organización utiliza el almacenamiento en la nube de Adobe, puede vincular recursos de Experience Manager Assets a cualquier objeto de Adobe Workfront que admita documentos.
author: Courtney
source-git-commit: b9eb36bbe792919e975cf27c06524755a3ef550b
workflow-type: tm+mt
source-wordcount: '935'
ht-degree: 12%

---

# Vinculación de recursos de Experience Manager Assets con Adobe Cloud Storage

Si su organización utiliza el almacenamiento en la nube de Adobe, puede vincular recursos de Experience Manager Assets a Workfront. Una vez enlazados, puede ver y administrar los recursos en Workfront, y los cambios realizados en los recursos en Experience Manager Assets se reflejarán en Workfront.

>[!IMPORTANT]
>
>Si su organización rechaza firmar el acuerdo GenAI Rider, aún puede utilizar el Asesor de contenido para elegir recursos en Experience Manager Assets, pero no tendrá acceso a funciones con tecnología de IA, como Búsqueda por IA, sugerencias inteligentes o análisis de informes de campaña.

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
   <td>Debe tener Experience Manager as a Cloud Service y se le debe añadir al producto como usuario en Admin Console.</td> 
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

* El administrador de Workfront debe configurar una integración de Experience Manager. Para obtener más información, consulte [Usar Adobe Experience Manager con la integración de Frame.io](/help/quicksilver/review-and-approve-work/native-integrations/frame-io/use-aem-with-frame.md).

* Para utilizar las sugerencias inteligentes o la funcionalidad de los informes de campaña, debe firmar un GenAI Rider. Para obtener más información, consulte [Usar el Asesor de contenido para obtener acceso al contenido de AEM en las aplicaciones de Adobe](https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search).

## Vincular contenido desde Experience Manager Assets

Para vincular contenido:

1. Vaya al objeto de Workfront donde desea vincular el contenido.
1. Haga clic en la sección **Documentos** del panel izquierdo.
1. Haga clic en **Nuevo** en el lado derecho de la página y, a continuación, haga clic en **Archivos de AEM** para vincular un recurso individual.
   ![Agregar archivos AEM al área de documentos](assets/aem-files.png)

1. Con el Asesor de contenido, puede:

   <table style="table-layout:auto">
   <tbody>
      <tr>
         <td><strong>Buscar recursos mediante la Búsqueda por IA.</strong> Utilice búsquedas impulsadas por IA que entiendan el significado y la intención que hay detrás de las consultas, y que admitan varios idiomas, errores tipográficos y sinónimos.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-advisor-ai-search">Búsqueda por IA para una detección de recursos más inteligente</a>.</td>
      </tr>
      <tr>
         <td><strong>Ver sugerencias inteligentes basadas en el contexto y la intención.</strong> Descubra recursos que se alinean con sus necesidades de contenido mediante recomendaciones según el contexto desde la aplicación host de Adobe.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#smart-suggestions-content-advisor">Sugerencias inteligentes basadas en el contexto y la intención</a>.</td>
      </tr>
      <tr>
         <td><strong>Cargue un informe de campaña para descubrir los recursos relevantes.</strong> Cargue un documento de resumen de campaña de PDF, DOCX o TXT para que el Asesor de contenido pueda analizarlo y recomendar recursos relevantes.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#campaign-briefs-content-advisor">Informes de Campaign para descubrir recursos relevantes</a>.</td>
      </tr>
      <tr>
         <td><strong>Ver y seleccionar representaciones de recursos de Dynamic Media.</strong> Explore representaciones optimizadas para canales, incluidos ajustes preestablecidos de imagen, recortes inteligentes y tipos de formato, y aplique modificadores de Dynamic Media para previsualizar los ajustes en tiempo real.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Representaciones de recursos de Dynamic Media disponibles para usar</a>.</td>
      </tr>
      <tr>
         <td><strong>Aplicar modificadores de Dynamic Media a las representaciones.</strong> Añada modificadores para transformar las representaciones de recursos en tiempo real y previsualizar los resultados antes de seleccionar una representación para la aplicación host.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#dynamic-media-renditions-content-advisor">Representaciones de recursos de Dynamic Media disponibles para usar</a>.</td>
      </tr>
      <!--
      <tr>
         <td><strong>Discover and browse Content Fragments.</strong> Search through Content Fragments, view live thumbnail previews, check status (Draft, Modified, or Published), and inspect detailed properties, references, and variations.</td>
         <td>For more information, see <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#content-fragments-discovery-content-advisor">Discovery of Content Fragments</a>.</td>
      </tr>
      -->
      <tr>
         <td><strong>Acceder a los metadatos del recurso.</strong> Revise las propiedades del recurso, como título, descripción, formato, tamaño y otras pestañas de metadatos (Producto, Campaña, Etiquetas) coherentes con la vista de Assets.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#asset-metadata-content-advisor">Acceder a metadatos de recursos compatibles con la vista de Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Filtrar recursos mediante filtros predefinidos.</strong> Restrinja los resultados de los recursos mediante filtros como Tipo de archivo, Formato de archivo, Estado del recurso, Tamaño de archivo, Anchura de imagen, Altura de imagen, Fecha de modificación y Fecha de creación.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#filters-content-advisor">Filtros de acceso compatibles con la vista de Assets</a>.</td>
      </tr>
      <tr>
         <td><strong>Guardar y reutilizar búsquedas.</strong> Cree búsquedas guardadas especificando un término de búsqueda y opciones de filtro y, a continuación, vuelva a utilizarlas en Experience Manager Assets y otras aplicaciones de Adobe.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#saved-searches-content-advisor">Acceder y reutilizar búsquedas recientes y guardadas</a>.</td>
      </tr>
      <tr>
         <td><strong>Busque recursos en las colecciones y entre ellas.</strong> Busque recursos o colecciones en todas las colecciones, o bien limite la búsqueda a una colección específica.</td>
         <td>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/experience-manager-cloud-service/content/assets/manage/content-advisor-adobe-applications#search-collections-content-advisor">Buscar recursos en las colecciones y entre ellas</a>.</td>
      </tr>
   </tbody>
   </table>

   >[!NOTE]
   >
   >El contenido recomendado en el Asesor de contenido utiliza datos de los siguientes elementos para determinar el contenido sugerido en Workfront:
   >
   >* Campos de nombre y descripción de objeto de Workfront
   >* Campos de formulario personalizados marcados como obligatorios
   >* Datos de documentos adjuntos

<!--
### Link a new version from Experience Manager Assets

You can pull new content over from Experience Manager Assets and add it to an existing asset as a new version. If the document is already linked and a new version is added in Experience Manager Assets, the new version appears automatically in Workfront.

To link a new version:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Select the asset you want to replace with a new version. You can't create a new version of an asset in a linked folder.
1. Select **Add New** > **Version**, then select the Experience Manager integration your administrator set up.

   >[!NOTE]
   >
   >The Workfront administrator can choose any name for this integration, so it might not specifically mention Experience Manager Assets.

1. Select the content you want to link.
1. Click **Select**.
-->

<!--
## Link a folder from Experience Manager Assets

Permissions to view individual assets inside of a folder rely on Experience Manager Assets permissions.

To link a folder:

1. Go to the Workfront object where you want to link content.
1. Click the **Documents** section in the left panel.
1. Click **Assets** > **Files & Folders**.
1. Click the **Filter** icon, then in the **Asset Type** section, choose **Folders**.
1. Select the folder you want to link.
1. Click **Select**.
-->

## Consideraciones

* Los flujos de trabajo de revisión y aprobación no son compatibles con los recursos de AEM vinculados.
* Los campos de metadatos se asignan por primera vez al enviar un recurso de Workfront a Experience Manager Assets. Si el administrador de Workfront ha habilitado la sincronización de metadatos de objetos, los campos permanecen actualizados si se modifican en alguna de las aplicaciones.
