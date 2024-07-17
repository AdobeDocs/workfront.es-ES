---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Uso de flujos de trabajo en la integración de Experience Manager Assets Essentials
description: Uso de flujos de trabajo en la integración de Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 821e31b8c6023a9ec4e017cc5548bb9fd930983c
workflow-type: tm+mt
source-wordcount: '1042'
ht-degree: 0%

---

# Uso de flujos de trabajo en la integración de Experience Manager Assets

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
   <td><strong>licencias de Adobe Workfront*</strong>
   </td>
   <td>Solicitud o superior
   </td>
  </tr>
  <tr>
   <td><strong>Producto</strong>
   </td>
   <td><p>Debe tener Assets Essentials as a Cloud Service de Experience Manager Assets y se le debe agregar al producto como usuario en el Admin Console.</p><p>Debe tener acceso de escritura al repositorio en Adobe Experience Manager.</p>
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso*</strong>
   </td>
   <td>Editar acceso a documentos
<p>
<strong>Nota: </strong>Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <strong>Crear o modificar niveles de acceso personalizados</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Permisos de objeto</strong>
   </td>
   <td>Administrar el acceso o superior en el proyecto 
<p>
Para obtener información sobre cómo solicitar acceso adicional, vea <strong>Solicitar acceso a los objetos </strong>.
   </td>
  </tr>
</table>

## Requisitos previos

Antes de empezar,

* El administrador de Workfront debe configurar los flujos de trabajo en una integración de Adobe Experience Manager. Para obtener más información, consulte [Configuración de la as a Cloud Service de Experience Manager Assets](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Adición de un flujo de trabajo a una plantilla

Puede agregar un flujo de trabajo a una plantilla de proyecto. El flujo de trabajo se aplicará a cualquier proyecto creado a partir de la plantilla.

1. Para abrir una plantilla, haga clic en **Plantillas** en el menú principal y seleccione la plantilla en la lista.
1. Haga clic en **Experience Manager Assets** en el panel de navegación izquierdo.

   >[!NOTE]
   >
   >Si la sección Experience Manager Assets no está visible en el panel de navegación izquierdo, el administrador de Workfront no ha habilitado flujos de trabajo para su organización. <!--Is this right?-->

1. En el campo **Seleccionar una integración para flujos de trabajo automatizados**, seleccione la integración con los flujos de trabajo que desee utilizar para los proyectos creados a partir de esta plantilla.
1. (Opcional) Edite los valores de flujo de trabajo que desee aplicar a los proyectos creados a partir de esta plantilla.

   Para obtener instrucciones sobre flujos de trabajo específicos, consulte [Editar valores de flujo de trabajo en un proyecto](#edit-workflow-values-in-a-project) en este artículo.

   Solo los flujos de trabajo que se han activado en el área de Experience Manager de la configuración están disponibles en las plantillas o proyectos.

1. Los cambios se guardan automáticamente. <!-- do they though??-->

## Añadir un flujo de trabajo a un proyecto

Puede agregar un flujo de trabajo al crear un proyecto o agregar un flujo de trabajo a un proyecto existente. En ambos casos, se utiliza una plantilla de proyecto para añadir el flujo de trabajo.

### Añadir un flujo de trabajo al crear un proyecto

1. Empiece a crear un proyecto.

   Para obtener instrucciones, vea [Crear un proyecto con una plantilla](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Al seleccionar una plantilla para el proyecto, seleccione la plantilla que contiene los flujos de trabajo que desea utilizar para este proyecto.
1. (Opcional) Edite cualquier valor de flujo de trabajo del proyecto, tal como se describe en [Editar valores de flujo de trabajo en un proyecto](#edit-workflow-values-in-a-project).

   Solo los flujos de trabajo que se han activado en el área de Experience Manager de la configuración están disponibles en las plantillas o proyectos.


### Añadir un flujo de trabajo a un proyecto existente

>[!NOTE]
>
>Los flujos de trabajo que se ejecutan cuando se crea un proyecto (como la creación de carpetas vinculadas) no se ejecutan cuando la plantilla está adjunta a un proyecto existente. Solo se ejecutan cuando se crea un proyecto a partir de una plantilla.

1. Comience a añadir una plantilla al proyecto.

   Para obtener instrucciones, vea [Adjuntar una plantilla a un proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Al seleccionar una plantilla para el proyecto, seleccione la plantilla que contiene los flujos de trabajo que desea utilizar para este proyecto.
1. (Opcional) Edite cualquier valor de flujo de trabajo del proyecto, tal como se describe en [Editar valores de flujo de trabajo en un proyecto](#edit-workflow-values-in-a-project).

   Solo los flujos de trabajo que se han activado en el área de Experience Manager de la configuración están disponibles en las plantillas o proyectos.



### Edición de valores de flujo de trabajo en un proyecto

Puede editar los valores del flujo de trabajo en el nivel de proyecto. Los valores de flujo de trabajo de nivel de proyecto anulan los valores establecidos en la plantilla de proyecto, que anulan los valores predeterminados establecidos en la integración de Adobe Experience Manager Assets.

Todos los valores de flujo de trabajo se encuentran en:

* La sección Flujos de trabajo o Carpetas vinculadas de la ventana Crear proyecto o Editar proyecto.
* La sección Adobe Experience Manager de la navegación izquierda.


  >[!NOTE]
  >
  >Si estas áreas no están visibles, el administrador de Workfront no ha habilitado Flujos de trabajo para su organización.



#### Carpetas vinculadas

>[!NOTE]
>
>Dado que las carpetas vinculadas se crean cuando se crea el proyecto, la edición del flujo de trabajo de carpetas vinculadas en un proyecto existente no es eficaz. La edición de estos valores al crear un proyecto funciona según lo esperado.

Para editar el flujo de trabajo de las carpetas vinculadas:


1. Activa o desactiva **[!UICONTROL Crear carpeta vinculada]** según quieras. Si lo activa, puede editar la configuración de la carpeta vinculada.

   Para obtener más información sobre la configuración de las carpetas vinculadas, consulte [Crear carpetas vinculadas de Adobe Experience Manager](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) en el artículo [Configurar la integración de [!UICONTROL Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

1. (Opcional) Si desea que el árbol de carpetas se genere solamente si ciertos valores están presentes en un formulario personalizado adjunto al proyecto, haga clic en el **Aplicar filtro** para ese árbol de carpetas y, a continuación, seleccione el formulario personalizado que contiene el campo, el campo y el valor del campo. Si el campo del formulario personalizado adjunto al nuevo proyecto contiene el valor elegido, se crea el árbol de carpetas.
1. (Opcional) Al configurar los nombres de las carpetas, puede seleccionar las siguientes opciones:

   * **Nombre**: escriba un nombre para la carpeta.

   * **Datos de objeto**: seleccione el origen del nombre de la carpeta, como Nombre del proyecto.

   * **Datos de formulario personalizados**: seleccione los datos de formulario personalizados que se usarán como nombre de carpeta.

     El uso de datos de formulario personalizados para nombres de carpeta solo está disponible en el nivel de plantilla y no se puede configurar en el nivel de integración.

     Si el nombre de una carpeta se establece en datos personalizados que no existen en el formulario personalizado adjunto al proyecto, se asigna un ID aleatorio como nombre de la carpeta.

1. Para ver el árbol de carpetas, haga clic en el icono **Vista previa** ![Icono de vista previa](assets/preview-icon.png)
1. Haga clic en **[!UICONTROL Guardar]**.

#### Publicación de recursos

Para editar el flujo de trabajo para publicar recursos:

1. Activar o desactivar **recursos de Publish automáticamente** según lo desee.
1. (Condicional) Si está habilitando la publicación, seleccione si desea publicarla en el servicio de publicación, en el portal de marca o en ambos.
1. Haga clic en **[!UICONTROL Guardar]**.
