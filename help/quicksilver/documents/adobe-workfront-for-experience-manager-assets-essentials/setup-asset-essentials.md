---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configuración de la integración de Experience Manager Assets Essentials
description: Conecte su trabajo a su contenido en Experience Manager Assets Essentials.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 430751f0e38c6c45145c965398990ee3652f36fe
workflow-type: tm+mt
source-wordcount: '651'
ht-degree: 96%

---

# Configurar la integración de Experience Manager Assets Essentials

Conecte su trabajo a su contenido en Experience Manager Assets Essentials:

* Inserte recursos y metadatos de Adobe Workfront en Experience Manager Assets Essentials
* Vincule recursos de Experience Manager Assets Essentials a sus proyectos y tareas de Workfront
* Facilite los flujos de trabajo de versiones para los recursos insertados en Experience Manager Assets Essentials

>[!NOTE]
>
>También puede conectar varios repositorios de Experience Manager Assets a un entorno de Workfront o varios entornos de Workfront a un repositorio de Experience Manager Assets en los ID de organización. Siga las instrucciones de configuración de este artículo para cada integración que desee configurar.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table>
  <tr>
   <td><strong>paquete de Adobe Workfront</strong>
   </td>
   <td>Cualquiera
   </td>
  </tr>
  <tr>
   <td><strong>licencias de Adobe Workfront</strong>
   </td>
   <td>
   <p>Estándar</p>
   <p>Plan</p>
   </td>
  </tr>
  <tr>
   <td><strong>Productos adicionales</strong>
   </td>
   <td>Debe tener Experience Manager Assets as a Cloud Service o Assets Essentials y se le debe añadir al producto como usuario.
   </td>
  </tr>
  <tr>
   <td><strong>Permisos de Experience Manager</strong>
   </td>
   <td>Debe tener acceso de escritura a la carpeta de destino en la integración de Experience Manager.
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso</strong>
   </td>
   <td>Debe ser administrador de Workfront para configurar una integración de Experience Manager. Una vez configurada, los usuarios con una licencia de Plan pueden configurar carpetas vinculadas en proyectos individuales.
   </td>
  </tr>
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar la integración

{{step-1-to-setup}}

1. Seleccione **Documentos** ![icono de documentos](assets/document-icon.png) en el panel izquierdo y, a continuación, seleccione **Integración de Experience Manager**.
1. Seleccione **Añadir integración de Experience Manager**.
1. Especifique lo siguiente:

   <table>
   <tr>
      <td><strong>Nombre</strong>
      </td>
      <td>Introduzca el nombre que desea que vean los usuarios en el botón Añadir nuevo del área Documentos.
      </td>
   </tr>
   <tr>
      <td><strong>URL de navegación</strong>
      </td>
      <td>El sistema rellena automáticamente la URL de navegación. Esta URL se utiliza para establecer el vínculo a la instancia de Assets Essentials de su organización desde el menú principal para un acceso rápido.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Repositorio de Experience Manager Assets</strong>
      </td>
      <td>
      El sistema rellena automáticamente el repositorio de Experience Manager asociado a su ID de organización.
      </td>
   </tr>
   </table>

1. Haga clic en **Guardar** o continúe en la sección [Configurar metadatos (opcional)](#set-up-metadata-optional) de este artículo.


## Configurar metadatos (opcional)

Asigne datos de objeto de Workfront a los campos de medios de recursos en Experience Manager Assets. Los metadatos se asignan cuando se envía un recurso desde Workfront por primera vez.


### Requisitos previos

Antes de empezar, debe

* Configure un esquema de metadatos en Experience Manager Assets Essentials como se explica en [Configurar la asignación de metadatos de recursos entre Adobe Workfront y Experience Manager Assets](https://experienceleague.adobe.com/en/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping).
* (Opcional) Configure campos de formulario personalizados en Workfront. Workfront tiene muchos campos personalizados integrados que puede utilizar. Sin embargo, también puede crear sus propios campos personalizados. Para obtener más información, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Campos compatibles de Workfront y Experience Manager Assets

### Palabra clave AEM

Puede asignar cualquier campo compatible con Workfront a una palabra clave en Experience Manager Assets Essentials.

Para vincular un campo a una palabra clave, seleccione `xcm:keywords` en la lista desplegable de campos de Experience Manager Assets situada en el área de asignación de metadatos.

Para asignar varios campos de texto de una sola línea a palabras clave, introduzca una lista separada por comas de los valores de palabras clave en el lado Workfront de la asignación de metadatos y `xcm:keywords` en el lado Experience Manager Assets. Cada valor de campo se asigna a una palabra clave independiente. Puede utilizar un campo calculado para combinar varios campos de Workfront en un único campo de texto separado por comas.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->


### Recursos

Los metadatos se asignan cuando se envía un recurso desde Workfront por primera vez. Los documentos con los campos integrados o personalizados se asignan automáticamente a los campos especificados la primera vez que se envía un recurso a Experience Manager Assets Essentials.

1. En la columna **Campo de Workfront**, elija un campo de Workfront integrado o personalizado.

   >[!NOTE]
   >
   >Puede asignar un solo campo de Workfront a varios campos de Experience Manager Assets. No se pueden asignar varios campos de Workfront a un único campo de Experience Manager Assets.

1. En el campo **Experience Manager**, elija un campo de Experience Manager Assets.

   Para asignar un campo de Workfront a una etiqueta de Experience Manager Assets, seleccione `xcm:keywords`.

1. Repita los pasos 1 y 2 según sea necesario.
   ![habilitar metadatos](assets/metadata-assets-essentials.png)
1. Haga clic en **Guardar** o continúe en la sección [Configurar carpetas vinculadas (opcional)](#set-up-linked-folders-optional) de este artículo.


## Configurar carpetas vinculadas (opcional)

{{setup-linked-folder}}
