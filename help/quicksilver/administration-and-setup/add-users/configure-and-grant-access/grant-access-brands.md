---
title: Conceder acceso a los permisos de marca
user-type: administrator
product-area: system-administration;documents
navigation-topic: configure-access-to-workfront
description: Como administrador de Adobe Workfront, puede configurar permisos de marca creando un grupo de usuarios en Admin Console y asignando el perfil de producto de GenStudio system manager.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 727efbd6-79b4-42c5-bfa2-e5350f30ff23
source-git-commit: f74c567505dbdf6b2d1d8a85a62ba40d919be7b3
workflow-type: tm+mt
source-wordcount: '707'
ht-degree: 9%

---

# Conceder acceso a los permisos de marca

{{highlighted-preview-article-level}}

A los usuarios se les otorgan los permisos de creación, edición y publicación de marca de los administradores del sistema de Adobe GenStudio cuando se agregan a un grupo de usuarios.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Estándar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de Admin Console</td> 
   <td> <p>Debe ser administrador del sistema en Adobe Admin Console.</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos

* La instancia de Workfront debe tener habilitadas las aprobaciones unificadas.

* Su organización debe tener GenStudio Foundation.
   * El Revisor de contenido de Workfront proporciona la funcionalidad disponible en GenStudio Foundation para los flujos de trabajo de revisión y aprobación de recursos. No es necesario que acceda directamente a GenStudio Foundation para completar su trabajo. El acceso a la funcionalidad de GenStudio Foundation a través del Revisor de contenido se encuentra dentro de los términos del contrato de Workfront.
* Adobe debe tener registrado un acuerdo de Adobe Gen AI.
Para obtener más información sobre la firma del acuerdo, consulte [Firmar el acuerdo de Adobe Gen AI](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement).

## &#x200B;1. Configurar los permisos de marca en Admin Console

### Paso 1: Crear un grupo de usuarios

Cree un nuevo grupo de usuarios en Admin Console para administrar permisos de creación y edición de marcas.

### Paso 2: Asignar un perfil de producto al grupo de usuarios

La asignación de derechos asociada al perfil asignado otorga permisos a todos los usuarios de este grupo para GenStudio Brands (crear, actualizar y eliminar marcas).

Para asignar un perfil:

1. Vaya al grupo de usuarios recién creado.
1. Haga clic en la ficha **Perfiles de producto asignados**.
1. Haga clic en **Asignar perfil**.
1. En la ventana emergente, selecciona **Adobe GenStudio** de la lista de productos y luego haz clic en **Aplicar**.
1. Seleccione el perfil **Adobe GenStudio Foundation editors**.
1. Haga clic en **Aplicar**.
1. Haga clic en **Guardar**.

### Paso 3: Agregar usuarios al grupo de usuarios

Para asignar a los usuarios permisos para crear, editar y publicar marcas, agréguelos al grupo de usuarios.

>[!NOTE]
>
>Debe agregar al menos un usuario antes de agregar el grupo a un proyecto, como se describe en el paso 4.

Para agregar usuarios:

1. Vaya a **Admin Console** > **Usuarios** > **Grupos de usuarios**.
1. Seleccione el grupo de usuarios.
1. Agregar usuarios por nombre de usuario o dirección de correo electrónico.
1. Seleccione entre las coincidencias sugeridas para los usuarios existentes.

### Paso 4: Crear un proyecto de marcas

Un proyecto proporciona una ubicación de almacenamiento en la que los usuarios pueden guardar los recursos de la marca.

Para crear un proyecto:

1. Vaya a la ficha **Almacenamiento** en Admin Console.
1. Haga clic en **Proyectos**.
1. Haga clic en **Crear proyecto**.
1. En la ventana emergente, escriba el nombre del proyecto: **Adobe GenStudio Brands**.

   >[!IMPORTANT]
   >
   >Introduzca el nombre del proyecto exactamente como se muestra. No agregue espacios adicionales ni cambie las mayúsculas y minúsculas.

1. Haga clic en **Crear**.

### Paso 5: Invitar al grupo de usuarios al proyecto

Agregue el grupo de usuarios al proyecto de marcas para que puedan acceder y administrar los recursos.

1. En la ventana emergente **Invitar al proyecto**, agregue el grupo de usuarios que creó.
1. Seleccione **Puede editar** permisos.
1. Haga clic en **Invitar**.

### Resultado

Los usuarios del grupo ahora tienen permisos para crear, editar y publicar recursos de marca en Workfront.

## &#x200B;2. Conceder acceso a marcas en los niveles de acceso de Workfront

Debe completar todos los pasos de la sección anterior antes de conceder acceso a usuarios individuales a marcas en los niveles de acceso de Workfront.

>[!IMPORTANT]
>
>* Solo los usuarios asignados al grupo de usuarios con el perfil de producto de GenStudio system manager en Admin Console pueden crear, editar y publicar marcas en Workfront, aunque otros usuarios tengan acceso a las marcas habilitado en su configuración de nivel de acceso.
>* Los usuarios añadidos al nivel de acceso con acceso a marcas habilitado, pero no agregados al grupo de usuarios en Admin Console, solo pueden ver marcas.


Para conceder acceso a marcas en niveles de acceso de Workfront:

{{step-1-to-setup}}

1. Haga clic en **Niveles de acceso** en el panel izquierdo.
1. Busque el nivel de acceso que desea editar y luego haga clic en el icono de edición ![editar icono](assets/edit-icon.png) para editarlo.

   O

   Haga clic en **Nuevo nivel de acceso** para crear un nuevo nivel de acceso. Para obtener más información acerca de cómo crear niveles de acceso, vea [Crear o modificar niveles de acceso personalizados](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).
1. Desplácese hacia abajo hasta **Establecer restricciones adicionales** y, a continuación, seleccione **Permitir que los usuarios tengan acceso a marcas**.
   ![permitir acceso a la configuración de marcas](assets/access-for-brands.png)
1. Haga clic en **Guardar**.

Una vez configuradas las marcas, puede crear un Revisor de contenido para revisar los recursos según las directrices de marca en el flujo de trabajo de revisión y aprobación. Para obtener más información, consulte [Configuración de colaboradores de IA](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/configure-ai-collaborators.md).
