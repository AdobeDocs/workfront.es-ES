---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Configuración de la integración de Experience Manager Assets Essentials
description: Conecte su trabajo con su contenido en Experience Manager Assets Essentials - EDIT ME.
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: abaa76e2-bbf1-47d0-8bdc-4e950df4f7ea
source-git-commit: 059cfa79c57f071b3c7efd690b583099f46c99fb
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 5%

---

# Configuración de la integración de Experience Manager Assets Essentials

Conecte su trabajo con el contenido de Experience Manager Assets Essentials &#x200B;:

* Insertar recursos y metadatos de Adobe Workfront en Experience Manager Assets Essentials &#x200B;
* Vincule recursos de Experience Manager Assets Essentials a sus proyectos y tareas en Workfront &#x200B;
* Facilitar los flujos de trabajo de versiones para los recursos insertados en Experience Manager Assets Essentials


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
   <td>Debe tener Experience Manager Assets Essentials y ser añadido al producto como usuario en el Admin Console.
   </td>
  </tr>
  <tr>
   <td><strong>Configuraciones de nivel de acceso</strong>
   </td>
   <td>Debe ser administrador de Workfront. Para obtener información sobre los administradores de Workfront, consulte <strong>Conceder a un usuario acceso administrativo completo</strong>.
   </td>
  </tr>
</table>


*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.


## Configuración de la integración

1. Haga clic en el **Menú principal** en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configuración**.
1. Select  **Documentos** ![icono de documentos](assets/document-icon.png) en el panel izquierdo, seleccione **Integración de Experience Manager**.
1. Select **Agregar integración de Experience Manager**.
1. Especifique lo siguiente:

   <table>
   <tr>
      <td><strong>Nombre</strong>
      </td>
      <td>Escriba el nombre que desea que vean los usuarios en el botón Agregar nuevo del área Documentos .
      </td>
   </tr>
   <tr>
      <td><strong>URL de navegación</strong>
      </td>
      <td>El sistema rellena automáticamente la URL de navegación. Esta URL se utiliza para vincular la instancia de Assets Essentials de su organización desde el menú principal para obtener acceso rápido.
      </td>
   </tr>
   <tr>
      <td>
      <strong>Repositorio de Experience Manager Assets</strong>
      </td>
      <td>
      El sistema rellena automáticamente el repositorio de Experience Manager asociado con su ID de organización.
      </td>
   </tr>
   </table>

1. Haga clic en **Guardar** o pase al [Configuración de metadatos (opcional)](#set-up-metadata-optional) en este artículo.


## Configuración de metadatos (opcional)

Asigne datos de objeto de Workfront a los campos de medios de recursos en Experience Manager Assets. Los metadatos se asignan cuando se envía un recurso desde Workfront por primera vez.


### Requisitos previos

Antes de empezar, debe

* Configure un esquema de metadatos en Experience Manager Assets Essentials tal como se explica en [Configuración de la asignación de metadatos de recursos entre Adobe Workfront y Experience Manager Assets](https://experienceleague.adobe.com/docs/experience-manager-cloud-service/content/assets/integrations/configure-asset-metadata-mapping.html?lang=en).
* (Opcional) Configure los campos de formulario personalizados en Workfront. Workfront tiene muchos campos personalizados integrados que puede utilizar. Sin embargo, también puede crear sus propios campos personalizados. Para obtener más información, consulte [Crear o editar un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).


### Assets

Los metadatos se asignan cuando un recurso se inserta desde Workfront por primera vez. Los documentos con los campos integrados o personalizados se asignan automáticamente a los campos especificados la primera vez que se envía un recurso a Experience Manager Assets Essentials.

1. En el **Campo Workfront** , elija un campo de Workfront integrado o personalizado.
   >[!NOTE]
   >
   >Puede asignar un solo campo de Workfront a varios campos de Experience Manager Assets. No se pueden asignar varios campos de Workfront a un único campo de Experience Manager Assets.
1. En el **Experience Manager** , seleccione un campo Experience Manager Assets .
1. Repita los pasos 1 y 2 según sea necesario.
   ![habilitar metadatos](assets/metadata-assets-essentials.png)
1. Haga clic en **Guardar** o pase al [Configuración de carpetas vinculadas (opcional)](#set-up-linked-folders-optional) en este artículo.


## Configuración de carpetas vinculadas (opcional)

{{setup-linked-folder}}
