---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Uso de flujos de trabajo en la integración de Experience Manager Assets Essentials
description: Uso de flujos de trabajo en la integración de Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 83cd0960947108186f8d1d8ef2ad6c35c89820bd
workflow-type: tm+mt
source-wordcount: '1114'
ht-degree: 0%

---

# Uso de flujos de trabajo en la integración de Experience Manager Assets

<span class="preview">La información resaltada en esta página hace referencia a funcionalidades que aún no están disponibles de forma general. Solo está disponible en el entorno de vista previa de espacio aislado.</span>

Un flujo de trabajo es un conjunto de acciones que conectan Workfront con Adobe Experience Manager as a Cloud Service. Un administrador de Workfront puede configurar flujos de trabajo en Workfront y, a continuación, asignarlos a plantillas de proyecto. Cuando se crea un proyecto utilizando una plantilla de proyecto a la que se asigna un flujo de trabajo, se activan las acciones definidas en el flujo de trabajo.

>[!NOTE]
>
>Los flujos de trabajo solo están disponibles en una integración de Adobe Experience Manager as a Cloud Service. No están disponibles en integraciones con Adobe Experience Manager Assets Essentials.


## Requisitos de acceso

Debe tener lo siguiente:

<table>
  <tr>
   <td><strong>plan Adobe Workfront*</strong>
   </td>
   <td>Cualquiera
   </td>
  </tr>
  <tr>
   <td><strong>Licencias de Adobe Workfront*</strong>
   </td>
   <td>Solicitud o superior
   </td>
  </tr>
  <tr>
   <td><strong>Product</strong>
   </td>
   <td><p>Debe tener Experience Manager Assets as a Cloud Service o Assets Essentials, y se le debe añadir al producto como usuario en el Admin Console.</p><p>Debe tener acceso de escritura al repositorio en Adobe Experience Manager.</p>
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso*</strong>
   </td>
   <td>Editar acceso a documentos
<p>
<strong>Nota: </strong>Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <strong>Crear o modificar niveles de acceso personalizados</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Permisos de objeto</strong>
   </td>
   <td>Administrar el acceso o superior en el proyecto 
<p>
Para obtener información sobre cómo solicitar acceso adicional, consulte <strong>Solicitud de acceso a objetos </strong>.
   </td>
  </tr>
</table>

## Requisitos previos

Antes de empezar,

* El administrador de Workfront debe configurar los flujos de trabajo en una integración de Adobe Experience Manager. Para obtener más información, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Adición de un flujo de trabajo a una plantilla

Puede agregar un flujo de trabajo a una plantilla de proyecto. El flujo de trabajo se aplicará a cualquier proyecto creado a partir de la plantilla.

1. Abra una plantilla haciendo clic en **Plantillas** en el menú principal y, a continuación, seleccione la plantilla en la lista.
1. Clic **Experience Manager Assets** en el panel de navegación izquierdo.

   >[!NOTE]
   >
   >Si la sección Experience Manager Assets no está visible en el panel de navegación izquierdo, el administrador de Workfront no ha habilitado flujos de trabajo para su organización. <!--Is this right?-->

1. En el **Seleccione un campo Integration for automated workflows**, seleccione la integración con los flujos de trabajo que desee utilizar para los proyectos creados a partir de esta plantilla.
1. (Opcional) Edite los valores de flujo de trabajo que desee aplicar a los proyectos creados a partir de esta plantilla.

   Para obtener instrucciones sobre flujos de trabajo específicos, consulte [Edición de valores de flujo de trabajo en un proyecto](#edit-workflow-values-in-a-project) en este artículo.

   Solo los flujos de trabajo que se han activado en el área de Experience Manager de la configuración están disponibles en las plantillas o proyectos.

1. Los cambios se guardan automáticamente. <!-- do they though??-->

## Añadir un flujo de trabajo a un proyecto

Puede agregar un flujo de trabajo al crear un proyecto o agregar un flujo de trabajo a un proyecto existente. En ambos casos, se utiliza una plantilla de proyecto para añadir el flujo de trabajo.

### Añadir un flujo de trabajo al crear un proyecto

1. Empiece a crear un proyecto.

   Para obtener instrucciones, consulte [Creación de un proyecto con una plantilla](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Al seleccionar una plantilla para el proyecto, seleccione la plantilla que contiene los flujos de trabajo que desea utilizar para este proyecto.
1. (Opcional) Edite los valores de flujo de trabajo del proyecto, tal como se describe en [Edición de valores de flujo de trabajo en un proyecto](#edit-workflow-values-in-a-project).

   Solo los flujos de trabajo que se han activado en el área de Experience Manager de la configuración están disponibles en las plantillas o proyectos.


### Añadir un flujo de trabajo a un proyecto existente

>[!NOTE]
>
>Los flujos de trabajo que se ejecutan cuando se crea un proyecto (como la creación de carpetas vinculadas) no se ejecutan cuando la plantilla está adjunta a un proyecto existente. Solo se ejecutan cuando se crea un proyecto a partir de una plantilla.

1. Comience a añadir una plantilla al proyecto.

   Para obtener instrucciones, consulte [Adjuntar una plantilla a un proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Al seleccionar una plantilla para el proyecto, seleccione la plantilla que contiene los flujos de trabajo que desea utilizar para este proyecto.
1. (Opcional) Edite los valores de flujo de trabajo del proyecto, tal como se describe en [Edición de valores de flujo de trabajo en un proyecto](#edit-workflow-values-in-a-project).

   Solo los flujos de trabajo que se han activado en el área de Experience Manager de la configuración están disponibles en las plantillas o proyectos.



### Edición de valores de flujo de trabajo en un proyecto

Puede editar los valores del flujo de trabajo en el nivel de proyecto. Los valores de flujo de trabajo de nivel de proyecto anulan los valores establecidos en la plantilla de proyecto, que anulan los valores predeterminados establecidos en la integración de Adobe Experience Manager Assets.

Todos los valores de flujo de trabajo se encuentran en:

* La sección Flujos de trabajo de la ventana Crear proyecto o Editar proyecto.
* La sección Adobe Experience Manager de la navegación izquierda.


  >[!NOTE]
  >
  >Si estas áreas no están visibles, el administrador de Workfront no ha habilitado Flujos de trabajo para su organización.



#### Carpetas vinculadas

>[!NOTE]
>
>Dado que las carpetas vinculadas se crean cuando se crea el proyecto, la edición del flujo de trabajo de carpetas vinculadas en un proyecto existente no es eficaz. La edición de estos valores al crear un proyecto funciona según lo esperado.

Para editar el flujo de trabajo de las carpetas vinculadas:

En el entorno de producción:

1. Alternar **[!UICONTROL Crear carpeta vinculada]** active o desactive según desee.
1. (Condicional) Si está habilitando carpetas vinculadas, elija una ruta de carpeta para indicar dónde desea que estén asociadas todas las carpetas vinculadas con esta integración.
1. Clic **[!UICONTROL Guardar]** si está utilizando el [!UICONTROL Crear proyecto] o [!UICONTROL Editar proyecto] ventana.

   O

   Si está en la [!DNL Adobe Experience Manager area], los cambios se guardan automáticamente. <!--Do they though?-->

En el entorno de vista previa de espacio aislado:

<div class="preview">

1. Alternar el **[!UICONTROL Crear carpeta vinculada]** active o desactive según desee. Si lo activa, puede editar la configuración de la carpeta vinculada.

   Para obtener más información sobre la configuración de la carpeta vinculada, consulte [Crear carpetas vinculadas de Adobe Experience Manager](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) en el artículo [Configure las variables [!UICONTROL Experience Manager Assets as a Cloud Service] integración](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

1. (Opcional) Si desea que el árbol de carpetas se cree únicamente si determinados valores están presentes en un formulario personalizado adjunto al proyecto, haga clic en **Aplicar filtro** para ese árbol de carpetas, seleccione el formulario personalizado que contiene el campo, el campo y el valor del campo. Si el campo del formulario personalizado adjunto al nuevo proyecto contiene el valor elegido, se crea el árbol de carpetas.
1. (Opcional) Al configurar los nombres de las carpetas, puede seleccionar las siguientes opciones:

   * **Nombre**: escriba un nombre para la carpeta.

   * **Datos de objeto**: seleccione el origen del nombre de la carpeta, como Nombre del proyecto.

   * **Datos de formulario personalizados**: seleccione los datos del formulario personalizado que se utilizarán como nombre de la carpeta.

     El uso de datos de formulario personalizados para nombres de carpeta solo está disponible en el nivel de plantilla y no se puede configurar en el nivel de integración.

     Si el nombre de una carpeta se establece en datos personalizados que no existen en el formulario personalizado adjunto al proyecto, se asigna un ID aleatorio como nombre de la carpeta.

1. Haga clic en **[!UICONTROL Guardar]**.

</div>


#### Publicación de recursos

Para editar el flujo de trabajo para publicar recursos:

1. Alternar **Publicar recursos automáticamente** active o desactive según desee.
1. (Condicional) Si está habilitando la publicación, seleccione si desea publicarla en el servicio de publicación, en el portal de marca o en ambos.
1. Haga clic en **[!UICONTROL Guardar]**.
