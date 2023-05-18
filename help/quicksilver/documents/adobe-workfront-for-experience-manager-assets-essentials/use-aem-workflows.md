---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Uso de flujos de trabajo en la integración de Experience Manager Assets Essentials
description: Uso de flujos de trabajo en la integración de Experience Manager Assets Essentials
author: Courtney, Becky
feature: Digital Content and Documents, Workfront Integrations and Apps
source-git-commit: 038f5f3c941ea69feb43492a30b5abea39f7c932
workflow-type: tm+mt
source-wordcount: '738'
ht-degree: 0%

---

# Uso de flujos de trabajo en la integración de Experience Manager Assets

Un flujo de trabajo es un conjunto de acciones que conectan Workfront con Adobe Experience Manager as a Cloud Service. Un administrador de Workfront puede configurar flujos de trabajo en Workfront y, a continuación, asignarlos a plantillas de proyecto. Cuando se crea un proyecto con una plantilla de proyecto a la que se asigna un flujo de trabajo, se activan las acciones definidas en el flujo de trabajo.

>[!NOTE]
>
>Los flujos de trabajo solo están disponibles en una integración con Adobe Experience Manager as a Cloud Service. No están disponibles en integraciones con Adobe Experience Manager Assets Essentials.


## Requisitos de acceso

Debe tener lo siguiente:

<table>
  <tr>
   <td><strong>plan de Adobe Workfront*</strong>
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
   <td><p>Debe tener Experience Manager Assets as a Cloud Service o Assets Essentials, y debe agregarlo al producto como usuario en el Admin Console.</p><p>Debe tener acceso de escritura al repositorio en Adobe Experience Manager para crear carpetas vinculadas.</p>&gt;
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso*</strong>
   </td>
   <td>Editar acceso a documentos
<p>
<strong>Nota: </strong>Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <strong>Crear o modificar niveles de acceso personalizados</strong>.
   </td>
  </tr>
  <tr>
   <td><strong>Permisos de objeto</strong>
   </td>
   <td>Administrar acceso o superior en el proyecto 
<p>
Para obtener información sobre la solicitud de acceso adicional, consulte <strong>Solicitar acceso a objetos </strong>.
   </td>
  </tr>
</table>

## Requisitos previos

Antes de empezar,

* El administrador de Workfront debe configurar los flujos de trabajo en una integración de Adobe Experience Manager. Para obtener más información, consulte [Configuración de la integración as a Cloud Service de Experience Manager Assets](../../administration-and-setup/configure-integrations/configure-aacs-integration.md#set-up-workflows-optional).

## Añadir un flujo de trabajo a una plantilla

Puede añadir un flujo de trabajo a una plantilla de proyecto. El flujo de trabajo se aplica a cualquier proyecto creado a partir de la plantilla.

1. <!-- main menu snippet??--> Abra una plantilla haciendo clic en **Plantillas** en el menú principal y, a continuación, seleccione la plantilla en la lista.
1. Haga clic en **Experience Manager Assets** en el panel de navegación izquierdo.

   >[!NOTE]
   >
   >Si la sección Experience Manager Assets no está visible en el panel de navegación izquierdo, el administrador de Workfront no ha habilitado los flujos de trabajo para su organización. <!--Is this right?-->

1. En el **Seleccionar un campo de integración para flujos de trabajo automatizados**, seleccione la integración con los flujos de trabajo que desea utilizar para los proyectos creados a partir de esta plantilla.
1. (Opcional) Edite los valores de flujo de trabajo que desee aplicar a los proyectos creados a partir de esta plantilla.

   Por ejemplo, para crear una carpeta vinculada en una ubicación distinta del valor predeterminado, introduzca la ubicación de la carpeta vinculada.

   Solo los flujos de trabajo activados en el área de Experience Manager de Configuración están disponibles en plantillas o proyectos.

1. Los cambios se guardan automáticamente. <!-- do they though??-->

## Añadir un flujo de trabajo a un proyecto

Puede añadir un flujo de trabajo al crear un proyecto o añadir un flujo de trabajo a un proyecto existente. En ambos casos, se utiliza una plantilla de proyecto para añadir el flujo de trabajo.

### Añadir un flujo de trabajo al crear un proyecto

1. Empiece a crear un proyecto.

   Para obtener instrucciones, consulte [Creación de un proyecto mediante una plantilla](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md).

1. Al seleccionar una plantilla para el proyecto, seleccione la plantilla que contiene los flujos de trabajo que desea utilizar para este proyecto.
1. (Opcional) Edite los valores de flujo de trabajo del proyecto, tal como se describe en [Editar valores de flujo de trabajo en un proyecto](#edit-workflow-values-in-a-project).

   Solo los flujos de trabajo activados en el área de Experience Manager de Configuración están disponibles en plantillas o proyectos.


### Añadir un flujo de trabajo a un proyecto existente

1. Empiece agregando una plantilla al proyecto.

   Para obtener instrucciones, consulte [Adjuntar una plantilla a un proyecto](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md).

1. Al seleccionar una plantilla para el proyecto, seleccione la plantilla que contiene los flujos de trabajo que desea utilizar para este proyecto.
1. (Opcional) Edite los valores de flujo de trabajo del proyecto, tal como se describe en [Editar valores de flujo de trabajo en un proyecto](#edit-workflow-values-in-a-project).

### Editar valores de flujo de trabajo en un proyecto

Puede editar los valores del flujo de trabajo en el nivel de proyecto. Los valores del flujo de trabajo de nivel de proyecto anulan los valores establecidos en la plantilla de proyecto, que anulan los valores predeterminados establecidos en la integración de Adobe Experience Manager Assets.

Todos los valores de flujo de trabajo se encuentran en:

* La sección Flujos de trabajo de la ventana Crear proyecto o Editar proyecto .
* Sección Adobe Experience Manager del panel de navegación izquierdo.


   >[!NOTE]
   >
   >Si estas áreas no están visibles, el administrador de Workfront no habilitó Flujos de trabajo para su organización.

#### Carpetas vinculadas

Para editar el flujo de trabajo de las carpetas vinculadas:

1. Alternar el **[!UICONTROL Crear carpeta vinculada]** en.
1. Elija una ruta de carpeta para indicar dónde desea asociar todas las carpetas vinculadas con esta integración.
1. Haga clic en Guardar si está utilizando la ventana Crear proyecto o Editar proyecto .

   O

   Si se encuentra en el área de Adobe Experience Manager, los cambios se guardarán automáticamente. <!--Do they though?-->

