---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Integraciones de Adobe Experience Manager Assets
description: Puede conectar su trabajo con las siguientes integraciones de Adobe Experience Manager Assets.
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: bc58cc77-a177-417f-a5a4-eec51e305219
source-git-commit: 9080dfe7e46a3780d493b59c8f2a3c4efbc011e7
workflow-type: tm+mt
source-wordcount: '1526'
ht-degree: 0%

---

# Configure las variables [!UICONTROL Experience Manager Assets as a Cloud Service] integración

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de espacio aislado de vista previa.</span>

Puede conectar su trabajo con su contenido en [!DNL Experience Manager Assets]&#x200B;:

* Insertar recursos y metadatos desde [!DNL Adobe Workfront] a [!DNL Experience Manager Assets]&#x200B;
* Vincular recursos desde [!DNL Experience Manager Assets] a sus proyectos y tareas en [!DNL Workfront&#x200B;]
* Facilitar casos de uso de versiones
* Crear carpetas vinculadas a [!DNL Experience Manager Assets]
* Seguimiento de metadatos para recursos y carpetas
* Sincronizar metadatos de proyecto entre [!DNL Workfront] y [!DNL Experience Manager Assets]

También puede conectar varios repositorios de Experience Manager Assets a un entorno de Workfront o varios entornos de Workfront a un repositorio de Experience Manager Assets en todos los ID de organización. Siga las instrucciones de configuración de este artículo para cada integración que desee configurar.

## Requisitos de acceso

Debe tener lo siguiente:

<table>
  <tr>
   <td><strong>[!DNL Adobe Workfront] plan*</strong>
   </td>
   <td>Cualquiera
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Adobe Workfront] licencias*</strong>
   </td>
   <td>[!UICONTROL Plan]
   </td>
  </tr>
  <tr>
   <td><strong>[!DNL Experience Manager] licencia</strong>
   </td>
   <td>[!UICONTROL Standard]
   </td>
  </tr>
  <tr>
   <td><strong>Product</strong>
   </td>
   <td>Debe tener [!DNL Experience Manager Assets as a Cloud Service], y debe agregarlo al producto como usuario.
   </td>
  </tr>
  <tr>
   <td>Configuraciones de nivel de acceso*
   </td>
   <td>Debe ser [!DNL Workfront] administrador. Para obtener información sobre [!DNL Workfront] administradores, consulte <strong>Conceder a un usuario acceso administrativo completo</strong>.
   </td>
  </tr>
</table>


*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.


## Requisitos previos

Antes de empezar,

* Debe tener [!DNL Workfront] y [!DNL Adobe Experience Manager Assets] asociado a un ID de organización en la variable [!DNL Adobe Admin Consol]e. Para obtener más información, consulte [Diferencias de administración basadas en plataformas ([!DNL Adobe Workfront]/[!DNL Adobe Business Platform])](/help/quicksilver/administration-and-setup/get-started-wf-administration/actions-in-admin-console.md).


## Configuración de la información de integración

1. Haga clic en el **[!UICONTROL Menú principal]** en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **[!UICONTROL Configuración]** .
1. Select **[!UICONTROL Documentos]** en el panel izquierdo, seleccione **[!UICONTROL [!DNL Experience Manager]Integración]**.
   >[!NOTE]
   >
   >Esta área de configuración solo aparece si su [!DNL Workfront] el entorno se incluye en un [!DNL Adobe Admin Console].

1. Select **[!UICONTROL Agregar [!DNL Experience Manager] Integración]**.
1. En el **[!UICONTROL Nombre]** , introduzca el nombre que desea que vean los usuarios al interactuar con esta integración en Workfront y Experience Manager Assets.
1. En el **[!UICONTROL URL de navegación]** , el sistema rellena automáticamente la URL de navegación. Esta dirección URL de solo lectura se utiliza para vincular la [!DNL Experience Manager] de la variable [!UICONTROL Menú principal] para acceso rápido.
1. Elija un repositorio de **[!UICONTROL [!DNL Experience Manager]Repositorio de recursos]** menú desplegable. El sistema rellena automáticamente cualquier [!DNL Experience Manager] repositorios asociados con el ID de organización al que está asignado su perfil de usuario.
   ![elegir repositorio de experience manager](assets/setup-information.png)

1. Haga clic en **[!UICONTROL Guardar]** o pase al [Configuración de metadatos (opcional)](#set-up-metadata-optional) en este artículo.

   >[!NOTE]
   >
   >Debido a la complejidad de la integración, no puede cambiar el repositorio después de guardar la configuración inicial.

## Configuración de metadatos (opcional)

Puede asignar [!DNL Workfront] datos de objeto a campos de medios de recurso [!DNL Experience Manager] Recursos.

>[!IMPORTANT]
>
>Los metadatos solo se pueden asignar en una dirección: from [!DNL Workfront] a [!DNL Experience Manager]. Metadatos de los documentos vinculados a [!DNL Workfront] from [!DNL Experience Manager] no se puede transferir a [!DNL Workfront].

### Configuración de campos de metadatos

Antes de empezar a asignar campos de metadatos, debe configurar los campos de metadatos tanto en Workfront como en Experience Manager Assets.

Para configurar los campos de metadatos:

1. Configurar un esquema de metadatos en [!DNL Experience Manager Assets] tal como se explica en [Configuración de la asignación de metadatos de recursos entre Adobes [!DNL Workfront] y [!DNL Experience Manager Assets]](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).


1. Configure los campos de formulario personalizados en Workfront. [!DNL Workfront] tiene muchos campos personalizados integrados que puede utilizar. Sin embargo, también puede crear sus propios campos personalizados, tal como se explica en [Crear o editar un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **Expandir para ver más información sobre los campos admitidos de Workfront y Experience Manager Assets**

**Etiquetas de Experience Manager Assets**

Puede asignar cualquier campo admitido de Workfront a una etiqueta en Experience Manager Assets. Para ello, debe asegurarse de que los valores de las etiquetas en Experience Manager Assets coinciden con Workfront.

* Las etiquetas y los valores de los campos de Workfront deben coincidir exactamente en ortografía y formato.
* Los valores de campo de Workfront asignados a etiquetas de recursos de experience Manager deben estar todos en minúsculas, incluso si la etiqueta de Experience Manager Assets parece tener letras mayúsculas.
* Los valores de campo de Workfront no deben incluir espacios.
* El valor del campo en Workfront también debe incluir la estructura de carpetas de la etiqueta Experience Manager Assets.
* Para asignar varios campos de texto de una sola línea a etiquetas, introduzca una lista separada por comas de los valores de las etiquetas en el lado Workfront de la asignación de metadatos y `xcm:keywords` en el lado de Experience Manager Assets. Cada valor de campo se asigna a una etiqueta independiente. Puede utilizar un campo calculado para combinar varios campos de Workfront en un único campo de texto separado por coma.
* Puede asignar valores de los campos desplegable, botón de opción o casilla de verificación introduciendo una lista separada por comas de los valores disponibles en ese campo.


>[!INFO]
>
>**Ejemplo**: Para que coincida con la etiqueta que se muestra en la estructura de carpetas, el valor del campo en Workfront sería `landscapes:trees/spruce`. Observe las letras minúsculas en el valor del campo Workfront.
>
>Si desea que la etiqueta sea el elemento de la izquierda en el árbol de etiquetas, debe ir seguida de dos puntos. En este ejemplo, para asignar a la etiqueta de paisajes, el valor de campo en Workfront sería `landscapes:`.
>
>![Estructura de carpetas en AEM](assets/aem-folder-structure-with-red-boxes.png)


Después de crear las etiquetas en Experience Manager Assets, estas aparecerán en el menú desplegable Etiquetas de la sección Metadatos . Para vincular un campo a una etiqueta, seleccione `xcm:keywords` en la lista desplegable de campos Experience Manager Assets del área de asignación de metadatos.

Para obtener más información sobre las etiquetas en Experience Manager Assets, incluido cómo crear y administrar las etiquetas, consulte [Administración de etiquetas](https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html).

**Campos de esquema de metadatos personalizados de Experience Manager Assets**

Puede asignar campos Workfront integrados y personalizados a campos de esquema de metadatos personalizados en Experience Manager Assets.

Los campos de metadatos personalizados creados en Experience Manager Assets se organizan en su propia sección del área de configuración de metadatos.

![sección de metadatos personalizados](assets/custom-metadata.png)

<!-- 
link to documentation about creating schema - waiting on response from Anuj about best article to link to
-->

**Campos Workfront**

Puede asignar campos Workfront integrados y personalizados a Experience Manager Assets. Los siguientes valores de campo deben coincidir tanto en mayúsculas como en ortografía entre Workfront y Experience Manager Assets:

* Campos desplegables
* Campos de selección múltiple

>[!TIP]
>
> Para comprobar si los valores de los campos coinciden exactamente, vaya a
>
> * Configuración > Forms personalizado en Workfront o el campo del objeto
> * Recursos > esquemas de metadatos en Experience Manager Assets


+++

### Asignación de metadatos para recursos

Los mapas de metadatos cuando se inserta un recurso [!DNL Workfront] por primera vez. Los documentos con los campos integrados o personalizados se asignan automáticamente a los campos especificados la primera vez que se envía un recurso a [!DNL Experience Manager Assets].

Para asignar metadatos para los recursos:

1. Select **[!UICONTROL Recursos]** encima de la tabla de metadatos.
1. En el **[!UICONTROL [!DNL Workfront]field]** , elija un campo de Workfront integrado o personalizado.

   >[!NOTE]
   >
   >Puede asignar una sola [!DNL Workfront] campo a varios [!UICONTROL Experience Manager Assets] campos. No se pueden asignar varios [!DNL Workfront] campos a un único [!DNL Experience Manager Assets] campo .
   ><!--To map a Workfront field to an Experience Manager Assets tag, see -->


1. En el [!DNL Experience Manager Assets] , busque en las categorías previamente rellenadas o escriba al menos dos letras en el campo de búsqueda para acceder a categorías adicionales.
1. Repita los pasos 2 y 3 según sea necesario.
   ![campos de metadatos](assets/asset-metadata.png)
1. Haga clic en [!UICONTROL Guardar] o pase al [Carpetas](#folders) en este artículo.

### Asignación de metadatos para carpetas

Cuando los usuarios crean una carpeta vinculada en un proyecto, los datos de proyecto, portafolio y programa asociados se asignan a campos de metadatos de carpeta en [!DNL Experience Manager Assets].

>[!NOTE]
>
>Esta integración no admite metadatos personalizados de [!DNL Adobe Experience Manager].

Para asignar metadatos para carpetas:

1. Select **[!UICONTROL Carpetas]** encima de la tabla de metadatos.
1. En el **[!UICONTROL [!DNL Workfront]field]** , elija un campo de Workfront integrado o personalizado.

   >[!NOTE]
   >
   >Puede asignar un solo campo de Workfront a varios campos de Experience Manager Assets. No se pueden asignar varios [!DNL Workfront] campos a un único [!DNL Experience Manager Assets] campo .

1. En el **[!DNL Experience Manager Assets]** , busque en las categorías previamente rellenadas o escriba al menos dos letras en el campo de búsqueda para acceder a categorías adicionales.
1. Repita los pasos 2 y 3 según sea necesario.
   ![metadatos de carpeta](assets/folder-metadata.png)
1. Haga clic en **[!UICONTROL Guardar]** o pase al [Sincronización de metadatos del proyecto](#project-metadata-sync) en este artículo.


### Sincronización de metadatos de objeto

Un [!DNL Experience Manager] campos asignados a [!DNL Workfront] los campos portafolio, programa, proyecto, tarea, problema y documento se actualizan automáticamente cuando se cambia el campo en [!DNL Workfront].

>[!IMPORTANT]
>
>Los usuarios deben tener acceso de escritura en [!DNL Experience Manager] para los recursos que residen en el objeto para que los metadatos se sincronicen cuando se actualicen.

1. Active la variable **[!UICONTROL Metadatos del objeto de sincronización]** campo .
1. Haga clic en **Guardar** o pase al [Configuración de flujos de trabajo (opcional)](#set-up-workflows-optional) en este artículo.

<!--Courtney start here-->

<div class="preview">

## Configuración de flujos de trabajo (opcional)

Un flujo de trabajo es un conjunto de acciones que conectan Workfront con Adobe Experience Manager as a Cloud Service. Como administrador de Workfront, puede configurar los flujos de trabajo en Workfront y, a continuación, asignarlos a las plantillas de proyecto. Cuando se crea un proyecto con una plantilla de proyecto a la que se asigna un flujo de trabajo, se activan las acciones definidas en el flujo de trabajo.

Los valores de flujo de trabajo predeterminados que se establecen en la integración se pueden sobrescribir en los niveles Plantilla de proyecto y Proyecto .

### Configuración de un flujo de trabajo para la creación de carpetas vinculadas de Adobe Experience Manager

1. Alternar el **[!UICONTROL Crear carpeta vinculada]** en.
1. Elija una ruta de carpeta para indicar dónde desea asociar todas las carpetas vinculadas con esta integración.
   ![Navegación de carpetas vinculadas](assets/select-folder-aem-integration.png)
1. Active la variable **Anexar Portfolio y nombres de programa** para incluir automáticamente los nombres de Portfolio y Programa al final del nombre de la carpeta vinculada.
1. Haga clic en **Guardar** o pase al [Configuración de carpetas vinculadas (opcional)](#set-up-linked-folders-optional) en este artículo.

</div>

<!--Courtney end here-->

## Configuración de carpetas vinculadas (opcional)

Puede permitir a los usuarios crear carpetas vinculadas a [!DNL Experience Manager] while en un [!DNL Workfront] proyecto. Cuando una carpeta está vinculada, cualquier recurso añadido a la carpeta se muestra automáticamente en ambas [!DNL Workfront] y [!DNL Experience Manager]. Cuando se agrega un recurso a la carpeta vinculada en [!DNL Workfront] por primera vez, los metadatos del recurso se insertan en [!DNL Experience Manager Assets].

En los pasos siguientes, se indica dónde desea crear las carpetas vinculadas. Cada integración solo puede tener una ubicación para todas las carpetas vinculadas.

Para configurar carpetas vinculadas:

1. Alternar el **[!UICONTROL Habilitar carpeta vinculada]** en.
1. Elija una ruta de carpeta para indicar dónde desea asociar todas las carpetas vinculadas con esta integración.

   >[!NOTE]
   >
   >Los usuarios necesitan acceso de escritura en [!DNL Adobe Experience Manager Assets] a la carpeta especificada para crear una carpeta vinculada.

1. Haga clic en **[!UICONTROL Guardar]**.
