---
user-type: administrator
product-area: system-administration;setup;user-management
navigation-topic: configure-proofing-functionality
title: Configuración del acceso de prueba de un usuario
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

# Configuración del acceso de prueba de un usuario

Como administrador de Adobe Workfront o de Workfront Proof, puede configurar el acceso de un usuario para crear y ver pruebas en Workfront y Workfront Proof.

Para obtener información sobre la funcionalidad de pruebas disponible para pruebas básicas e integradas, consulte [Acceso a la funcionalidad de pruebas en Workfront](../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de Workfront o administrador de Workfront Proof. Para obtener información sobre los administradores de Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Habilitar y deshabilitar las pruebas para un usuario (solo planes heredados) {#enable-and-disable-proofing-for-a-user-legacy-plans-only}

Si su organización utiliza un plan heredado de Select o Premium Workfront, como administrador de Workfront, puede habilitar y deshabilitar la funcionalidad de pruebas para el usuario.

Al habilitar la prueba para un usuario, Workfront habilita la opción para que las pruebas del usuario se generen automáticamente.

Aunque puede habilitar un usuario como usuario de pruebas, debe tener permisos de administrador para navegar directamente a la interfaz de Workfront Proof desde el menú principal de Workfront. Para obtener información sobre cómo habilitar esta opción para todos los usuarios de prueba del sistema Workfront, consulte [Configuración del acceso a Workfront Proof a través del menú principal de Workfront para todos los usuarios](#configure-workfront-proof-access-via-workfront-main-menu-for-all-users).

1. En el **Menú principal**, seleccione **Usuarios**.

1. Seleccione un usuario y, a continuación, haga clic en el **Editar** icono.
1. En el **Acceso** , seleccione o anule la selección **El usuario puede generar pruebas**.

## Configuración del perfil de permiso de prueba de un usuario

El perfil de permiso seleccionado se concede a los usuarios para cada prueba que exista dentro de su organización.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Usuarios** ![](assets/users-icon-in-main-menu.png).
1. Seleccione uno o varios usuarios y haga clic en **Editar**.

1. En el **Acceso** , haga clic en una de las siguientes opciones de permiso de Workfront Proof en la **Perfil de permiso de prueba** menú desplegable:

   >[!NOTE]
   >
   >Si está en un plan de Workfront heredado, asegúrese de que la variable **El usuario puede generar pruebas** está activada, tal como se explica más arriba en la sección [Habilitar y deshabilitar las pruebas para un usuario (solo planes heredados)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Supervisor</strong> </td> 
      <td>Los usuarios pueden administrar y ver todas las pruebas creadas en la cuenta de la organización. También pueden editar los revisores agregados a estas pruebas. Los usuarios con este perfil de permisos no pueden administrar usuarios ni editar la configuración de Workfront Proof.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Gerente</strong> </td> 
      <td> <p> Los usuarios pueden administrar y ver las pruebas creadas o que se poseen en la cuenta de la organización. Solo pueden ver las pruebas de otros usuarios cuando se añaden como revisores. Se trata de una configuración predeterminada. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Administrador</strong> </td> 
      <td> Los usuarios reciben permisos de administrador en Workfront Proof y pueden editar la configuración de la cuenta. Los usuarios pueden administrar y ver todas las pruebas creadas en la cuenta de la organización. Esto incluye agregar y eliminar revisores, pruebas y comentarios.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Personalizada</strong> </td> 
      <td> <p>Solo está disponible si ha configurado un perfil de permiso personalizado en Workfront Proof.</p> <p><b>NOTA</b>:  <p>Asegúrese de que el perfil de permiso que concede aquí no proporcione un acceso mayor que el del nivel de acceso del usuario en Workfront (consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>). Si proporciona un acceso más alto, el usuario puede acceder a las pruebas de Workfront de que no puede acceder dentro de Workfront.</p> <p>Esto es especialmente importante si planea permitir que todos los usuarios de Workfront accedan a Workfront Proof directamente desde Workfront, tal como se describe en <a href="../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md" class="MCXref xref">Acceso a la prueba de Workfront desde Adobe Workfront</a>.</p> <p>De forma predeterminada, solo los administradores de Workfront tienen acceso a un vínculo directo al sitio de prueba de Workfront desde la barra de navegación global de Workfront.</p> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   El perfil de permiso seleccionado se concede a los usuarios para cada prueba que exista dentro de su organización.

1. Haga clic en **Guardar cambios** para completar la actualización de la configuración de usuario.

   >[!NOTE]
   >
   >Cuando crea o actualiza un usuario en Workfront y la dirección de correo electrónico de Workfront del usuario coincide con la de un usuario con licencia de Workfront Proof, el sistema habilita la prueba para el usuario en Workfront. Para obtener más información, consulte [Sincronización de usuarios entre Adobe Workfront y Workfront Proof](../../../administration-and-setup/manage-workfront/configure-proofing/user-sync-proofing.md).

### Consideraciones

Tenga en cuenta la siguiente información al configurar permisos:

* Si cambia el perfil de permisos de un usuario a un perfil con menos permisos, el usuario podría perder la visibilidad de las pruebas existentes en Workfront. Esto puede ocurrir cuando alguien comparte una tarea con un usuario dentro de Workfront, pero no comparte la prueba adjunta a la tarea (consulte [Compartir una prueba en Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md) en [Compartir una prueba en Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md)).
* Solo puede establecer permisos de prueba de Workfront desde Workfront si su entorno de Workfront está integrado con una cuenta de Workfront Proof Premium . Si no puede utilizar pruebas como se explica en esta sección, póngase en contacto con el administrador de Workfront.
* Al menos un usuario del entorno de Workfront debe tener permisos de administrador para realizar pruebas. Aparece un mensaje de error si intenta eliminar los permisos de administrador para pruebas de todos los usuarios.
* Cuando cambia el nivel de acceso de Workfront de un usuario a cualquier nivel que no sea el administrador del sistema, el perfil de permiso de Workfront Proof del usuario toma el valor predeterminado de Manager.

* Cuando cambia el nivel de acceso de Workfront a Administrador del sistema, el perfil de permisos de prueba cambia a Administrador.

## Configuración del acceso a Workfront Proof a través del menú principal de Workfront para todos los usuarios {#configure-workfront-proof-access-via-workfront-main-menu-for-all-users}

De forma predeterminada, solo los usuarios con derechos administrativos dentro de Workfront pueden acceder a Workfront Proof tal como se describe  [Acceso a la prueba de Workfront desde Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).

Puede conceder acceso a todos los usuarios al botón Prueba de Workfront del menú principal de Workfront poniéndose en contacto con el servicio de asistencia de Workfront y enviando una solicitud.

>[!IMPORTANT]
>
> Si planea permitir que todos los usuarios de Workfront accedan a Workfront Proof directamente desde la barra de navegación global de Workfront, asegúrese de que el perfil de permisos de cada usuario no proporcione más acceso que el nivel de acceso del usuario en Workfront. Esto impide que los usuarios accedan a pruebas en Workfront Proof a las que no pueden acceder desde Workfront. Para obtener más información, consulte [Habilitar y deshabilitar las pruebas para un usuario (solo planes heredados)](#enable-and-disable-proofing-for-a-user-legacy-plans-only).

## Configuración del acceso del usuario al Visor de prueba de escritorio

Si los usuarios de su organización prefieren utilizar el Visor de prueba de escritorio en lugar del Visor de prueba web para revisar contenido interactivo, puede configurar el Visor de prueba de escritorio para que se inicie automáticamente cuando los usuarios abran pruebas de contenido interactivo. Para obtener información sobre esto, el Visor de prueba de escritorio y cómo difiere del Visor de prueba web, consulte [Comprender el Visor de pruebas de escritorio](../../../workfront-proof/wp-work-proofsfiles/review-proofs-dpv/destop-proofing-viewer.md) y [Diferencias entre el visor de pruebas web y el visor de pruebas de escritorio](../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md).

1. En Workfront, haga clic en el icono de prueba de Workfront en la barra de navegación global para acceder a la prueba de Workfront.

   ![](assets/proof-access-proofhq-350x39.png)

1. Haga clic en **Configuración de la cuenta** cerca de la esquina superior derecha de la prueba de Workfront y, a continuación, haga clic en la **Configuración** pestaña .

1. En **Valores predeterminados de prueba**, al final del **Visor de pruebas de escritorio para pruebas interactivas** fila, haga clic en **Configuración**.

1. Modifique la configuración del Visor de prueba de escritorio, tal como se describe en [Visor de prueba de escritorio](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#desktop-proofing-viewer) en el artículo [Configuración de pruebas para su organización](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).

1. Haga clic en **Guardar**.

## Configuración de dispositivos personalizados para pruebas interactivas

Puede añadir cualquier dispositivo personalizado al sistema, lo que permite a los usuarios revisar el contenido interactivo y simular cómo aparece el contenido en un dispositivo específico cuando utilizan el Visor de prueba de escritorio. (Esta funcionalidad no está disponible en el visor de pruebas web, donde los usuarios pueden revisar el contenido interactivo, pero solo tal y como aparece en varias resoluciones, no en varios dispositivos).

Para obtener más información, consulte [Cambiar la resolución de prueba interactiva en el visor de pruebas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md).

1. Desde Workfront, acceda a la interfaz de prueba de Workfront, tal como se describe en [Acceso a la prueba de Workfront desde Adobe Workfront](../../../review-and-approve-work/proofing/managing-proofs-within-workfront/access-wf-proof-in-workfront.md).
1. Modifique la configuración del Visor de prueba de escritorio, tal como se describe en [Configuración de dispositivos personalizados para pruebas](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md#custom-devices-for-proofs) en el artículo [Configuración de pruebas para su organización](../../../administration-and-setup/manage-workfront/configure-proofing/configure-proofing-organization.md).
