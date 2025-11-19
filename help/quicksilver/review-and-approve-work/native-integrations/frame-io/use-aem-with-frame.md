---
product-area: documents
navigation-topic: approvals
title: Uso de Adobe Experience Manager con la integración de Frame.io
description: Uso de Adobe Experience Manager con la integración de Frame.io
author: Courtney
feature: Work Management, Digital Content and Documents
recommendations: noDisplay, noCatalog
source-git-commit: 8c5202bcdb367266d31a2e056eed9a286f286518
workflow-type: tm+mt
source-wordcount: '1615'
ht-degree: 78%

---


# Uso de Adobe Experience Manager con la integración de Frame.io

Puede usar [!DNL Experience Manager Assets]&#x200B;&#x200B; para administrar y almacenar los recursos digitales que han pasado por el ciclo de revisión y aprobación. Esta integración le permite aprovechar las capacidades de Adobe Experience Manager, Frame.io y Workfront para optimizar los procesos de colaboración y administración de contenido.

## Configuración de la integración de Experience Manager Assets

Puede conectar su trabajo con el contenido en [!DNL Experience Manager Assets]:

* Insertar recursos y metadatos de [!DNL Adobe Workfront] a [!DNL Experience Manager Assets]
* Facilitar casos de uso de versiones
* Seguimiento de metadatos para recursos
* Sincronizar metadatos de proyecto entre [!DNL Workfront] y [!DNL Experience Manager Assets]

>[!NOTE]
>
>También puede conectar varios repositorios de [!DNL Experience Manager Assets] a un entorno de [!UICONTROL Workfront] o varios entornos de [!DNL Workfront] a un repositorio de [!DNL Experience Manager Assets] en los identificadores de organización. Siga las instrucciones de configuración de este artículo para cada integración que desee configurar.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table>
  <tr>
   <td>Paquete de Adobe Workfront
   </td>
   <td> <p>PRIME o ULTIMATE</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr>
    <tr>
   <td>Licencias de Adobe Workfront
   </td>
   <td>
  <p>Para configurar la integración:</p>
   <p>Estándar</p>
   <p>Plan</p>

<p>Para enviar documentos a Experience Manager Assets:</p>
   <p>Colaborador o superior</p>
   <p>Solicitud o superior</p>
   </td>
  </tr>
  </tr>
    <tr>
   <td>Licencias de Adobe Experience Manager
   </td>
   <td>Estándar
   </td>
  </tr>
  <tr>
   <td>Productos adicionales
   </td>
   <td>Debe tener [!DNL Experience Manager Assets as a Cloud Service] y se le debe añadir al producto como usuario.
   </td>
  </tr>
   <tr>
   <td>Configuraciones de nivel de acceso
   </td>
   <td>Debe ser administrador de [!DNL Workfront].
   </td>
  </tr>
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Antes de comenzar,

* Debe tener [!DNL Workfront] y [!DNL Adobe Experience Manager Assets] asociados con un identificador de organización en [!DNL Adobe Admin Console]. Para obtener más información, consulte [Diferencias de administración basadas en la plataforma ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).
* La instancia de Workfront debe utilizar Adobe Enterprise Storage.


## Configuración de la información de integración

{{step-1-to-setup}}

1. Seleccione **[!UICONTROL Documents]** en el panel izquierdo y, a continuación, seleccione **[!UICONTROL [!DNL Experience Manager]Integration]**.
1. Seleccione **[!UICONTROL Add [!DNL Experience Manager] Integration]**.
1. En el campo **[!UICONTROL Name]**, escriba el nombre que desea que los usuarios vean al interactuar con esta integración en Workfront y Experience Manager Assets.
1. En el campo **[!UICONTROL Navigation URL]**, el sistema rellena automáticamente la URL de navegación. Esta URL de solo lectura se usa para vincular la instancia [!DNL Experience Manager] de su organización desde el [!UICONTROL Main Menu] para obtener acceso rápido.
1. Elija un repositorio en el menú desplegable **[!UICONTROL [!DNL Experience Manager]Assets repository]**. El sistema rellena automáticamente los repositorios de [!DNL Experience Manager] asociados con el identificador de organización al que está asignado el perfil de usuario.
   ![Elija repositorio de Experience manager](assets/setup-information.png)

1. Haga clic en **[!UICONTROL Guardar]** o continúe con la sección [Configurar metadatos (opcional)](#set-up-metadata-optional) de este artículo.

   >[!IMPORTANT]
   >
   >Debido a la complejidad de la integración, no puede cambiar el repositorio después de guardar la configuración inicial.


## Configurar metadatos (opcional)

Puede asignar [!DNL Workfront] datos de objeto a campos de medios de recursos en [!DNL Experience Manager] Assets.

>[!NOTE]
>
>Solo puede asignar metadatos en una dirección: de [!DNL Workfront] a [!DNL Experience Manager]. Los metadatos de los documentos vinculados a [!DNL Workfront] desde [!DNL Experience Manager] no se pueden transferir a [!DNL Workfront].

### Configuración de los campos de metadatos

Antes de empezar a asignar campos de metadatos, debe configurarlos tanto en Workfront como en Experience Manager Assets.

Para configurar campos de metadatos:

1. Configure un esquema de metadatos en [!DNL Experience Manager Assets] como se explica en [Configurar la asignación de metadatos de recursos entre Adobe [!DNL Workfront]  y  [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).


1. Configure campos de formulario personalizados en Workfront. [!DNL Workfront] tiene muchos campos personalizados integrados que puede utilizar. Sin embargo, también puede crear sus propios campos personalizados, tal como se explica en [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

+++ **Amplíe para ver más información sobre los campos Workfront y Experience Manager Assets compatibles** 

**Etiquetas de Experience Manager Assets**

Puede asignar cualquier campo compatible con Workfront a una etiqueta de Experience Manager Assets. Para ello, debe asegurarse de que los valores de las etiquetas en Experience Manager Assets coinciden con Workfront.

* Los valores de los campos Etiquetas y de Workfront deben coincidir exactamente en cuanto a ortografía y formato.
* Los valores de los campos de Workfront asignados a las etiquetas de Experience Manager Assets deben estar en minúsculas, incluso si la etiqueta de Experience Manager Assets parece tener letras mayúsculas.
* Los valores de los campos de Workfront no deben incluir espacios.
* El valor del campo en Workfront también debe incluir la estructura de carpetas de la etiqueta Experience Manager Assets.
* Para asignar varios campos de texto de una sola línea a las etiquetas, escriba una lista separada por comas de los valores de las etiquetas en el lado Workfront de la asignación de metadatos y `xcm:keywords` en el lado de Experience Manager Assets. Cada valor de campo se asigna a una etiqueta independiente. Puede utilizar un campo calculado para combinar varios campos de Workfront en un único campo de texto separado por comas.
* Puede asignar valores de los campos desplegables, botón de opción o casilla de verificación introduciendo una lista separada por comas de los valores disponibles en ese campo.


>[!INFO]
>
>**Ejemplo**: Para que coincida con la etiqueta mostrada en la estructura de carpetas, el valor del campo en Workfront sería `landscapes:trees/spruce`. Tenga en cuenta las letras minúsculas en el valor del campo Workfront.
>
>Si desea que la etiqueta sea el elemento situado más a la izquierda en el árbol de etiquetas, debe ir seguida de dos puntos. En este ejemplo, para asignar a la etiqueta de paisajes, el valor del campo en Workfront sería `landscapes:`.
>
>![Estructura de carpetas en AEM](assets/aem-folder-structure-with-red-boxes.png)


Una vez creadas las etiquetas en Experience Manager Assets, aparecerán en la lista desplegable Etiquetas de la sección Metadatos. Para vincular un campo a una etiqueta, seleccione `xcm:keywords` en la lista desplegable de campos de Experience Manager Assets en el área de asignación de metadatos.

Para obtener más información sobre las etiquetas en Experience Manager Assets, incluyendo cómo crear y administrar etiquetas, consulte [Administración de etiquetas](https://experienceleague.adobe.com/en/docs/experience-manager-64/administering/contentmanagement/tags).

**Campos de esquema de metadatos personalizados de Experience Manager Assets**

Puede asignar campos de Workfront integrados y personalizados a campos de esquema de metadatos personalizados en Experience Manager Assets.

Los campos de metadatos personalizados creados en Experience Manager Assets se organizan en su propia sección, en el área Configuración de metadatos.

![sección de metadatos personalizados](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Campos de Workfront**

Puede asignar campos de Workfront integrados y personalizados a Experience Manager Assets. Los siguientes valores de campo deben coincidir en ambos casos y en la ortografía entre Workfront y Experience Manager Assets:

* Campos desplegables
* Campos de selección múltiple

>[!TIP]
>
> Para comprobar si los valores del campo coinciden exactamente, vaya a
>
> * Configuración > Formularios personalizados en Workfront o el campo en el objeto
> * Recursos > Esquemas de metadatos en Experience Manager Assets

+++

### Asignar metadatos a los recursos

Los metadatos se asignan cuando se inserta un recurso desde [!DNL Workfront] por primera vez. Los documentos con los campos integrados o personalizados se asignan automáticamente a los campos especificados la primera vez que se envía un recurso a [!DNL Experience Manager Assets].

Para asignar metadatos a los recursos:

<!--
1. Select **[!UICONTROL Assets]** above the metadata table.
-->
1. En la columna **[!UICONTROL [!DNL Workfront]campo]**, elija un campo Workfront integrado o personalizado.

   >[!NOTE]
   >
   >Puede asignar un solo campo [!DNL Workfront] a varios campos de [!UICONTROL Experience Manager Assets]. No se pueden asignar varios campos de [!DNL Workfront] a un único campo de [!DNL Experience Manager Assets].
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->

1. En el campo [!DNL Experience Manager Assets], busque en las categorías previamente completadas o escriba al menos dos letras en el campo de búsqueda para acceder a categorías adicionales.
1. Repita los pasos 2 y 3 según sea necesario.
   ![campos de metadatos](assets/metadata-no-asset-toggle.png)
1. Haz clic en [!UICONTROL **Guardar**] o desplázate a la sección [Sincronización de metadatos de objetos](#object-metadata-sync) de este artículo.



### Sincronización de metadatos de objeto

Los campos de [!DNL Experience Manager] asignados a [!DNL Workfront] campos de portafolio, programa, proyecto, tarea, problema y documento se actualizan automáticamente cuando el campo se cambia en [!DNL Workfront].

Cuando esta opción está habilitada, cualquier recurso que se haya insertado en Adobe Experience Manager muestra una vista en tiempo real de los metadatos de Adobe Experience Manager del documento en la página Detalles del documento en Workfront.

1. Habilite el campo **[!UICONTROL Sincronizar metadatos de objeto]** y haga clic en **Guardar**.

>[!IMPORTANT]
>
>Los usuarios deben tener acceso de escritura en [!DNL Experience Manager] para los recursos que residen en el objeto a fin de que los metadatos se sincronicen cuando se actualicen.


## Enviar documentos a Experience Manager Assets o Assets Essentials

Es posible enviar documentos desde Workfront a Experience Manager Assets o Assets Essentials. Los documentos cargados y enviados desde Workfront a Assets Essentials siguen contando para el almacenamiento general de documentos.

Assets enviado a Experience Manager mediante esta integración tiene un límite de tamaño de **5o TB**.

<!--In the Preview environment, Assets sent to Experience Manager through this integration have a size limit of **30 GB**.-->

Los campos de metadatos se asignan por primera vez al enviar un recurso desde Workfront a Experience Manager Assets o a Assets Essentials. También se envían los metadatos configurados para asignar a objetos principales. Para obtener más información sobre la configuración de la asignación de metadatos, consulte [Configuración de la integración de Experience Manager Assets as a Cloud Service](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) o [Configuración de la integración de Experience Manager Assets Essentials](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**Ejemplo**: la primera vez que envía un recurso adjunto a un proyecto, los metadatos se asignan a Experience Manager Assets o Assets Essentials, así como cualquier metadato asignado de objetos principales, como un portafolio y un programa.



### Enviar documentos desde Workfront

Cuando un usuario envía un documento desde Workfront a Experience Manager Assets o a Assets Essentials, los metadatos asignados se transfieren a lo largo del documento. Una vez enviado el documento, los cambios realizados en los metadatos del documento en Workfront no se reflejarán en Assets ni en Assets Essentials. Si se cambia un campo asignado en Workfront, se debe enviar una nueva versión del documento con los metadatos actualizados a Assets o Assets Essentials.

Para enviar documentos:

1. Vaya al área **Documentos** de Workfront y seleccione el documento que quiera enviar.
1. Haga clic en **Enviar a** y, a continuación, elija la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente los recursos ni a Assets Essentials.

   ![Enviar a](assets/send-to-aem.png)

1. Elija dónde desea que vaya el recurso y haga clic en **Seleccionar carpeta**.
1. Al encontrar el destino deseado, haga clic en **Guardar**.

### Enviar una nueva versión

Es posible añadir una nueva versión a un documento que se haya cargado anteriormente en Workfront. Para obtener más información, consulte [Cargar una nueva versión de un documento](/help/quicksilver/documents/managing-documents/upload-new-document-version.md). Una vez cargada la versión más reciente, puede enviarla a Assets Essentials. Si un campo asignado en Workfront ha cambiado, la nueva versión actualiza los metadatos en Assets Essentials cuando los envía.

>[!IMPORTANT]
>
>Antes de cargar una nueva versión en Workfront, le recomendamos que cambie el nombre del archivo. Si carga una nueva versión con el mismo nombre de archivo que una versión anterior, solo se puede descargar la versión más reciente desde Workfront. Todas las versiones se pueden descargar desde Experience Manager Assets o Assets Essentials, independientemente del nombre del archivo. <!--Is this still a thing with ESM?-->

Para enviar la versión más reciente:

1. Vaya al área de **Documentos** en Workfront y busque el documento.
1. Seleccione **Enviar a** y, a continuación, elija la integración de Experience Manager que configuró el administrador.

   >[!NOTE]
   >
   >El administrador de Workfront puede elegir cualquier nombre para esta integración, por lo que es posible que no mencione específicamente los recursos ni a Assets Essentials.

   ![Enviar a](assets/send-to-aem.png)

1. Haga clic en **Guardar**. La nueva versión se guarda en la misma ubicación que la versión anterior.
