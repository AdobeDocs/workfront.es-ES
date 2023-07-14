---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configuración de la integración de Experience Manager Assets Essentials
description: 'Conecte su trabajo con el contenido de Experience Manager Assets Essentials: EDITARME.'
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: a6cb6d4780f2b1c3e77547caf7324e882d2dab4f
workflow-type: tm+mt
source-wordcount: '643'
ht-degree: 4%

---

# Configuración de la integración de Experience Manager Assets Essentials

Conecte su trabajo con el contenido de Experience Manager Assets Essentials&#x200B;:

* Inserción de recursos y metadatos de Adobe Workfront en Experience Manager Assets Essentials&#x200B;
* Vincule recursos de Experience Manager Assets Essentials a sus proyectos y tareas en Workfront&#x200B;
* Facilitar los flujos de trabajo de versiones para los recursos insertados en Experience Manager Assets Essentials

>[!NOTE]
>
>También puede conectar varios repositorios de Experience Manager Assets a un entorno de Workfront o varios entornos de Workfront a un repositorio de Experience Manager Assets en los ID de organización. Siga las instrucciones de configuración de este artículo para cada integración que desee configurar.

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
   <td>Plan
   </td>
  </tr>
  <tr>
   <td><strong>licencia de Experience Manager</strong>
   </td>
   <td>Estándar
   </td>
  </tr>
  <tr>
   <td><strong>Product</strong>
   </td>
   <td>Debe tener Experience Manager Assets Essentials y se le debe añadir al producto como usuario en el Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso</strong>
   </td>
   <td>Debe ser administrador de Workfront. Para obtener información sobre los administradores de Workfront, consulte <strong>Conceder a un usuario acceso administrativo completo</strong>.
   </td>
  </tr>
</table>


*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.


## Configuración de la integración

1. Haga clic en **Menú principal** en la esquina superior derecha de Adobe Workfront y haga clic en **Configurar**.
1. Seleccionar  **Documentos** ![icono de documentos](assets/document-icon.png) en el panel izquierdo, seleccione **Integración de Experience Manager**.
1. Seleccionar **Añadir integración de Experience Manager**.
1. Especifique lo siguiente:

   <table>
   <tr>
      <td><strong>Nombre</strong>
      </td>
      <td>Escriba el nombre que desea que vean los usuarios en el botón Agregar nuevo del área Documentos.
      </td>
   </tr>
   <tr>
      <td><strong>URL de navegación</strong>
      </td>
      <td>El sistema rellena automáticamente la URL de navegación. Esta URL se utiliza para vincular a la instancia de Assets Essentials de su organización desde el menú principal para acceder rápidamente.
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

1. Clic **Guardar** o continúe con la [Configuración de metadatos (opcional)](#set-up-metadata-optional) de este artículo.


## Configuración de metadatos (opcional)

Asigne datos de objeto de Workfront a los campos de medios de recursos en Experience Manager Assets. Los metadatos se asignan cuando se envía un recurso desde Workfront por primera vez.


### Requisitos previos

Antes de empezar, debe

* Configure un esquema de metadatos en Experience Manager Assets Essentials como se explica en [Configuración de la asignación de metadatos de recursos entre Adobe Workfront y Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Opcional) Configure campos de formulario personalizados en Workfront. Workfront tiene muchos campos personalizados integrados que puede utilizar. Sin embargo, también puede crear sus propios campos personalizados. Para obtener más información, consulte [Crear o editar un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

+++ **Campos compatibles de Workfront y Experience Manager Assets**

**AEM Palabra clave**

Puede asignar cualquier campo compatible con Workfront a una palabra clave en Experience Manager Assets Essentials.

Para vincular un campo a una palabra clave, seleccione `dc:subject` en el menú desplegable del campo Experience Manager Assets, en el área de asignación de metadatos.

Para asignar varios campos de texto de una sola línea a palabras clave, introduzca una lista separada por comas de los valores de las palabras clave en el lado Workfront de la asignación de metadatos, y `dc:subject` en el lado de Experience Manager Assets. Cada valor de campo se asigna a una palabra clave independiente. Puede utilizar un campo calculado para combinar varios campos de Workfront en un único campo de texto separado por comas.

<!--
Look for essentials article
For more information on keywords in Experience Manager Assets, including how to create and manage keywords, see [Administering Tags]( https://experienceleague.adobe.com/docs/experience-manager-64/administering/contentmanagement/tags.html?lang=en).
-->

+++


### Assets

Los metadatos se asignan cuando se envía un recurso desde Workfront por primera vez. Los documentos con los campos integrados o personalizados se asignan automáticamente a los campos especificados la primera vez que se envía un recurso a Experience Manager Assets Essentials.

1. En el **Campo de Workfront** , elija un campo integrado o personalizado de Workfront.
   >[!NOTE]
   >
   >Puede asignar un solo campo de Workfront a varios campos de Experience Manager Assets. No se pueden asignar varios campos de Workfront a un único campo de Experience Manager Assets.
1. En el **Experience Manager** , seleccione un campo de Experience Manager Assets.

   Para asignar un campo Workfront a una etiqueta Experience Manager Assets, seleccione `dc:subject`.
1. Repita los pasos 1 y 2 según sea necesario.
   ![habilitar metadatos](assets/metadata-assets-essentials.png)
1. Clic **Guardar** o continúe con la [Configurar carpetas vinculadas (opcional)](#set-up-linked-folders-optional) de este artículo.


## Configurar carpetas vinculadas (opcional)

{{setup-linked-folder}}
