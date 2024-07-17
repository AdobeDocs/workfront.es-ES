---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configuración del acceso de revisión de un usuario
description: Como administrador de Adobe Workfront o de Workfront Proof, puede configurar el acceso de un usuario para crear y ver pruebas en Workfront y Workfront Proof.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 98c90139-f31a-41bc-af0b-577dd8b254e3
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# Configuración del acceso de revisión de un usuario

Como administrador de Adobe Workfront o de Workfront Proof, puede configurar el acceso de un usuario para crear y ver pruebas en Workfront y Workfront Proof.

Para obtener información acerca de la funcionalidad de revisión disponible para la revisión básica e integrada, consulte [Acceso a la funcionalidad de revisión en Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de Workfront o de Workfront Proof. Para obtener información sobre los administradores de Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo total a un usuario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Habilitar y deshabilitar la revisión para un usuario (solo para planes heredados) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Si su organización utiliza un plan Select o Premium Workfront heredado, como administrador de Workfront, puede habilitar y deshabilitar la funcionalidad de revisión para el usuario.

Al habilitar la revisión para un usuario, Workfront habilita la opción para que las pruebas del usuario se generen automáticamente.

Aunque puede habilitar a un usuario como usuario de revisión, debe tener permisos de administrador para navegar directamente a la interfaz de Workfront Proof desde el menú principal de Workfront. Para obtener información sobre cómo habilitar esta opción para todos los usuarios de revisión de su sistema Workfront, consulte [Configuración del acceso a Workfront Proof a través del menú principal de Workfront para todos los usuarios](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. En el **Menú principal**, seleccione **Usuarios**.

1. Seleccione un usuario y luego haga clic en el icono **Editar**.
1. En la sección **Acceder**, seleccione o anule la selección de **El usuario puede generar pruebas**.

## Configuración del perfil de permiso de revisión de un usuario

El perfil de permiso seleccionado se concede a los usuarios para cada prueba que exista dentro de su organización.

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y luego haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).
1. Seleccione uno o más usuarios y luego haga clic en **Editar**.

1. En la sección **Acceso**, haga clic en una de las siguientes opciones de permiso de Workfront Proof en el menú desplegable **Perfil de permiso de revisión**:

   >[!NOTE]
   >
   >Si tiene un plan Workfront heredado, asegúrese de que la opción **El usuario puede generar pruebas** esté habilitada, como se explica más arriba en la sección [Habilitar y deshabilitar la revisión para un usuario (solo para planes heredados)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Los usuarios pueden administrar y ver todas las pruebas creadas en la cuenta de la organización. También pueden editar los revisores agregados a estas pruebas. Los usuarios con este perfil de permiso no pueden administrar usuarios ni editar la configuración de Workfront Proof.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Responsable</strong> </td> 
      <td> <p> Los usuarios pueden administrar y ver las pruebas creadas o que pertenecen a la cuenta de su organización. Solo pueden ver las pruebas de otros usuarios cuando se agregan como revisores. Esta es una configuración predeterminada. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrador</strong> </td> 
      <td> Los usuarios tienen permisos de administrador en Workfront Proof y pueden editar la configuración de la cuenta. Los usuarios pueden administrar y ver todas las pruebas creadas en la cuenta de la organización. Esto incluye agregar y eliminar revisores, pruebas y comentarios.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personalizado</strong> </td> 
      <td> <p>Solo está disponible si ha configurado un perfil de permiso personalizado en Workfront Proof.</p> <p><b>NOTA</b>:  <p>Asegúrese de que el perfil de permiso que concede aquí no proporcione un acceso mayor que la configuración de nivel de acceso del usuario en Workfront (consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>). Si proporciona un acceso mayor, el usuario puede acceder a pruebas en Workfront Proof a las que no puede acceder en Workfront.</p> <p>Esto es especialmente importante si planea permitir que todos los usuarios de Workfront accedan a Workfront Proof directamente desde Workfront, tal como se describe en <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Acceder a Workfront Proof desde Adobe Workfront</a>.</p> <p>De forma predeterminada, solo los administradores de Workfront tienen acceso a un vínculo directo al sitio de Workfront Proof desde la barra de navegación global de Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   El perfil de permiso seleccionado se concede a los usuarios para cada prueba que exista dentro de su organización.

1. Haga clic en **Guardar cambios** para completar la actualización de la configuración del usuario.

   >[!NOTE]
   >
   >Cuando crea o actualiza un usuario en Workfront y su dirección de correo electrónico de Workfront coincide con la de un usuario con licencia de Workfront Proof, el sistema permite realizar pruebas para el usuario en Workfront. Para obtener más información, consulte [Sincronización de usuarios entre Adobe Workfront y Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Consideraciones

Tenga en cuenta la siguiente información al configurar permisos:

* Si cambia el perfil de permiso de un usuario a un perfil con menos permisos, es posible que el usuario pierda visibilidad de las pruebas existentes en Workfront. Esto puede ocurrir cuando alguien comparte una tarea con un usuario de Workfront, pero no comparte la revisión adjunta a la tarea (consulte [Compartir una revisión en Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) en [Compartir una revisión en Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* Solo puede establecer permisos de Workfront Proof desde Workfront si su entorno de Workfront está integrado con una cuenta de Workfront Proof Premium. Si no puede utilizar la revisión como se describe en esta sección, póngase en contacto con su administrador de Workfront.
* Al menos un usuario del entorno de Workfront debe tener permisos de administrador para la revisión. Aparecerá un mensaje de error si intenta quitar a todos los usuarios los permisos de administrador para la revisión.
* Al cambiar el nivel de acceso de Workfront de un usuario a cualquier nivel distinto del de administrador del sistema, el perfil de permisos de Workfront Proof del usuario toma el valor predeterminado de Administrador.

* Al cambiar el nivel de acceso de Workfront a Administrador del sistema, el perfil de permisos de cambia a Administrador.

## Configure el acceso a Workfront Proof a través del menú principal de Workfront para todos los usuarios {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

De manera predeterminada, solo los usuarios con derechos administrativos en Workfront pueden acceder a Workfront Proof como se describe [Acceder a Workfront Proof desde Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Puede otorgar a todos los usuarios acceso al botón Workfront Proof dentro del menú principal de Workfront poniéndose en contacto con el Soporte técnico de Workfront y enviando una solicitud.

>[!IMPORTANT]
>
> Si planea permitir que todos los usuarios de Workfront accedan a Workfront Proof directamente desde la barra de navegación global de Workfront, asegúrese de que el perfil de permiso de cada usuario no proporcione más acceso que el nivel de acceso del usuario dentro de Workfront. Esto evita que los usuarios accedan a pruebas dentro de Workfront Proof a las que no pueden acceder dentro de Workfront. Para obtener más información, consulte [Habilitar y deshabilitar la revisión para un usuario (solo planes heredados)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Configuración del acceso de los usuarios al Visor de corrección de escritorio

Si los usuarios de su organización prefieren utilizar el Visor de pruebas de escritorio en lugar del Visor de pruebas web para revisar el contenido interactivo, puede configurar el Visor de pruebas de escritorio para que se inicie automáticamente cuando los usuarios abran pruebas de contenido interactivo. Para obtener información acerca de esto en el Visor de corrección de escritorio y en qué se diferencia del Visor de corrección de web, vea [Comprender el Visor de corrección de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) y [Diferencias entre el Visor de corrección de web y la descripción general del Visor de corrección de escritorio](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. En Workfront, haga clic en el icono Workfront Proof de la barra de navegación global para acceder a Workfront Proof.

   ![](assets/proof-access-proofhq-350x39.png)

1. Haga clic en **Configuración de la cuenta** cerca de la esquina superior derecha de Workfront Proof y, a continuación, haga clic en la ficha **Configuración**.

1. En **Valores predeterminados de revisión**, al final de la fila **Visor de revisión de escritorio para revisión interactiva**, haga clic en **Configurar**.

1. Modifique la configuración del Visor de pruebas de escritorio, tal como se describe en [Visor de pruebas de escritorio](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) en el artículo [Configurar las opciones de pruebas para su organización](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Haga clic en **Guardar**.

## Configuración de dispositivos personalizados para pruebas interactivas

Puede agregar cualquier dispositivo personalizado al sistema, lo que permite a los usuarios revisar el contenido interactivo y simular cómo aparece el contenido en un dispositivo específico cuando utilizan el Visor de corrección de escritorio. (Esta funcionalidad no está disponible en el Visor de pruebas web, donde los usuarios pueden revisar el contenido interactivo, pero solo como aparece en varias resoluciones, no en varios dispositivos).

Para obtener más información, consulte [Cambiar la resolución de prueba interactiva en el visor de revisión](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Desde Workfront, accede a la interfaz de Workfront Proof como se describe en [Acceder a Workfront Proof desde Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modifique la configuración del Visor de revisión de escritorio, tal como se describe en [Configurar dispositivos personalizados para pruebas](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) en el artículo [Configurar la configuración de revisión para su organización](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
