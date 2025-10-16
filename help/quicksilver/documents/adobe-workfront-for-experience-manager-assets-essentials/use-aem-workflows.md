---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Uso de flujos de trabajo en la integración de Experience Manager Assets Essentials
description: Uso de flujos de trabajo en la integración de Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 4c1e5ec1-3fd1-4527-ba8a-9db1a2350f69
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '1012'
ht-degree: 97%

---

# Uso de flujos de trabajo en la integración de Experience Manager Assets

Un flujo de trabajo es un conjunto de acciones que conectan Workfront con Adobe Experience Manager as a Cloud Service. Un administrador de Workfront puede configurar flujos de trabajo en Workfront y, a continuación, asignarlos a plantillas de proyecto.

Cuando se crea un proyecto utilizando una plantilla de proyecto a la que se asigna un flujo de trabajo, se activan las acciones definidas en el flujo de trabajo.

>[!NOTE]
>
>Los flujos de trabajo solo están disponibles en una integración de Adobe Experience Manager as a Cloud Service. No están disponibles en integraciones con Adobe Experience Manager Assets Essentials.


## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
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

Antes de comenzar,

* El administrador de Workfront debe configurar los flujos de trabajo en una integración de Adobe Experience Manager. Para obtener más información, consulte [Configuración de la integración de Experience Manager Assets as a Cloud Service](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Añadir un flujo de trabajo a una plantilla

Puede añadir un flujo de trabajo a una plantilla de proyecto. El flujo de trabajo se aplicará a cualquier proyecto creado a partir de la plantilla.

1. Para abrir una plantilla, haga clic en **Plantillas** en el menú principal y seleccione la plantilla en la lista.
1. Haga clic en **Experience Manager Assets** en el panel de navegación izquierdo.

   >[!NOTE]
   >
   >Si la sección Experience Manager Assets no está visible en el panel de navegación izquierdo, el administrador de Workfront no ha habilitado flujos de trabajo para su organización. <!--Is this right?-->

1. En el campo **Seleccionar una integración para flujos de trabajo automatizados**, seleccione la integración con los flujos de trabajo que desee utilizar para los proyectos creados a partir de esta plantilla.
1. (Opcional) Edite los valores de flujo de trabajo que desee aplicar a los proyectos creados a partir de esta plantilla.

   Para obtener instrucciones sobre flujos de trabajo específicos, consulte [Editar valores de flujo de trabajo en un proyecto](#edit-workflow-values-in-a-project) en este artículo.

   Solo los flujos de trabajo que se han activado en el área Configuración de Experience Manager están disponibles en las plantillas o proyectos.

1. Los cambios se guardan automáticamente. <!-- do they though??-->

## Añadir un flujo de trabajo a un proyecto

Puede añadir un flujo de trabajo al crear un proyecto, o añadir un flujo de trabajo a un proyecto existente. En ambos casos, se utiliza una plantilla de proyecto para añadir el flujo de trabajo.

### Añadir un flujo de trabajo al crear un proyecto

1. Empiece a crear un proyecto.

   Para obtener instrucciones, consulte [Crear un proyecto con una plantilla](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Al seleccionar una plantilla para el proyecto, seleccione la plantilla que contiene los flujos de trabajo que desea utilizar para este proyecto.
1. (Opcional) Edite cualquier valor del flujo de trabajo del proyecto, como se describe en [Editar valores de flujo de trabajo en un proyecto](#edit-workflow-values-in-a-project).

   Solo los flujos de trabajo que se han activado en el área Configuración de Experience Manager están disponibles en las plantillas o proyectos.


### Añadir un flujo de trabajo a un proyecto existente

>[!NOTE]
>
>Los flujos de trabajo que se ejecutan cuando se crea un proyecto (como la creación de carpetas vinculadas) no se ejecutan cuando la plantilla se adjunta a un proyecto existente. Solo se ejecutan cuando se crea un proyecto desde una plantilla.

1. Empiece a añadir una plantilla al proyecto.

   Para obtener instrucciones, consulte [Adjuntar una plantilla a un proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Al seleccionar una plantilla para el proyecto, seleccione la plantilla que contiene los flujos de trabajo que desea utilizar para este proyecto.
1. (Opcional) Edite cualquier valor del flujo de trabajo del proyecto, como se describe en [Editar valores de flujo de trabajo en un proyecto](#edit-workflow-values-in-a-project).

   Solo los flujos de trabajo que se han activado en el área Configuración de Experience Manager están disponibles en las plantillas o proyectos.



### Editar valores de flujo de trabajo en un proyecto

Puede editar los valores del flujo de trabajo a nivel de proyecto. Los valores de flujo de trabajo a nivel de proyecto anulan los valores establecidos en la plantilla de proyecto, que anulan los valores predeterminados establecidos en la integración de Adobe Experience Manager Assets.

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

1. Active o desactive **[!UICONTROL Crear carpeta vinculada]** según desee. Si activa esta opción, puede editar la configuración de la carpeta vinculada.

   Para obtener información detallada sobre la configuración de las carpetas vinculadas, consulte [Crear carpetas vinculadas de Adobe Experience Manager](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md#create-adobe-experience-manager-linked-folders) en el artículo [Configurar la integración de [!UICONTROL Experience Manager Assets as a Cloud Service]](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md).

1. (Opcional) Si desea que el árbol de carpetas se genere solamente si determinados valores están presentes en un formulario personalizado adjunto al proyecto, haga clic en **Aplicar filtro** para ese árbol de carpetas y, a continuación, seleccione el formulario personalizado que contiene el campo, el campo y el valor del campo. Si el campo del formulario personalizado adjunto al nuevo proyecto contiene el valor elegido, se creará el árbol de carpetas.
1. (Opcional) Al configurar los nombres de las carpetas, puede seleccionar las siguientes opciones:

   * **Nombre**: escriba un nombre para la carpeta.

   * **Datos de objeto**: seleccione el origen del nombre de la carpeta, como, por ejemplo, el nombre del proyecto.

   * **Datos de formulario personalizados**: seleccione los datos de formulario personalizados que se utilizarán como nombre de carpeta.

     El uso de datos de formulario personalizados para nombres de carpeta solo está disponible a nivel de plantilla y no se puede configurar a nivel de integración.

     Si el nombre de una carpeta se establece en datos personalizados que no existen en el formulario personalizado adjunto al proyecto, se asigna un ID aleatorio como nombre de la carpeta.

1. Para ver el árbol de carpetas, haga clic en el icono de **Vista previa** ![Icono de vista previa](assets/preview-icon.png)
1. Haga clic en **[!UICONTROL Guardar]**.

#### Publicación de recursos

Para editar el flujo de trabajo para publicar recursos:

1. Active o desactive **Publicar recursos automáticamente** según desee.
1. (Condicional) Si está habilitando la publicación, seleccione si desea publicarla en el servicio de publicación, en Brand Portal o ambos.
1. Haga clic en **[!UICONTROL Guardar]**.
