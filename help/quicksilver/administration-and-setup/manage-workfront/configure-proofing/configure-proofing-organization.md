---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configuración de revisión para su organización
description: Como administrador de Adobe Workfront o de Workfront Proof, puede personalizar la configuración de revisión predeterminada para su organización. Esta configuración incluye opciones de uso compartido predeterminadas, personalización de marca y mucho más.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 29405172-c3dd-431f-a242-fd38b53a307d
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '1221'
ht-degree: 0%

---

# Configure las opciones de prueba para su organización

Como administrador de Adobe Workfront o de Workfront Proof, puede personalizar la configuración de revisión predeterminada para su organización. Esta configuración incluye opciones de uso compartido predeterminadas, personalización de marca y mucho más.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o Superior</p> <p>o</p> <p>Plan heredado: Premium o Select</p> <p>Para obtener más información sobre cómo revisar el acceso con los diferentes planes, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o Plan</p> <p>Plan heredado: Cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe haber seleccionado Administrador en el perfil de permisos de revisión. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurar el acceso de revisión de un usuario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Configuración de acciones

Para obtener información acerca del uso de acciones en el visor de revisión, vea [Usar acciones en comentarios sobre revisión](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/use-actions-on-comments-in-viewer.md).

Puede configurar acciones para su organización de las siguientes maneras:

* [Agregar o cambiar el nombre de una acción](#add-or-rename-an-action)
* [Desactivar o reactivar una acción](#deactivate-or-reactivate-an-action)
* [Reordenar acciones](#reorder-actions)

### Agregar o cambiar el nombre de una acción {#add-or-rename-an-action}

{{step1-to-proofing}}

1. Haga clic en **Configuración** > **Configuración de la cuenta** en la esquina superior derecha de la interfaz de Workfront Proof y, a continuación, haga clic en la ficha **Configuración**.

1. Realice una de las acciones siguientes:

   * Para crear una acción nueva, en la sección **Acciones**, haga clic en **Nueva acción**.

     No hay límite en la cantidad de acciones que puede configurar en su cuenta.

   * Para cambiar el nombre de una acción existente, haga clic en **Configuración** junto a la acción.

1. Escriba un nombre para la acción y haga clic en **Guardar**.
1. Haga clic en **Guardar.**

### Desactivar o reactivar una acción {#deactivate-or-reactivate-an-action}

{{step1-to-proofing}}

1. Haga clic en **Configuración** > **Configuración de la cuenta** en la esquina superior derecha de la interfaz de Workfront Proof y, a continuación, haga clic en la ficha **Configuración**.

1. Haga clic en **Configuración** junto a la acción que desee desactivar o reactivar.
1. Seleccione **Activar** o **Desactivar** y luego haga clic en **Guardar**.

### Reordenar acciones {#reorder-actions}

{{step1-to-proofing}}

1. Haga clic en **Configuración** > **Configuración de la cuenta** en la esquina superior derecha de la interfaz de Workfront Proof y, a continuación, haga clic en la ficha **Configuración**.

1. Haga clic en las flechas azules arriba y abajo junto a **Configuración** para reordenar las acciones.

   ![Reordenar_acciones.png](assets/re-order-actions-350x103.png)

## Configuración de dispositivos personalizados para pruebas

Puede añadir cualquier dispositivo personalizado al sistema, lo que permite a los usuarios revisar el contenido interactivo y simular cómo aparece el contenido en un dispositivo específico.

Para obtener información sobre cómo los usuarios pueden seleccionar dispositivos al revisar el contenido interactivo, consulte [Cambiar la resolución de la prueba interactiva en el visor de revisión](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md)

Para agregar un dispositivo personalizado:

{{step1-to-proofing}}

1. Haga clic en **Configuración** > **Configuración de la cuenta** en la esquina superior derecha de la interfaz de Workfront Proof y, a continuación, haga clic en la ficha **Configuración**.

1. En la sección **Dispositivos personalizados para pruebas**, haga clic en **Agregar nuevo dispositivo**.

1. En el cuadro **Agregar nuevo dispositivo** que aparece, especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td>El nombre que ven los usuarios al seleccionar el dispositivo en el Visor de corrección de escritorio, como se describe en <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-a-proof/view-interactive-content-as-it-appears-in-device.md" class="MCXref xref">Cambiar la resolución interactiva de la revisión en el Visor de revisión</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dimensiones</td> 
      <td>Especifique las dimensiones que desea utilizar para este dispositivo. Los usuarios ven las dimensiones que se muestran debajo del nombre del dispositivo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Proporción</td> 
      <td>Especifique la proporción del dispositivo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo</td> 
      <td>Seleccione si el dispositivo es móvil, tableta o escritorio.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cadena del agente de usuario</td> 
      <td>Introduzca el agente de usuario del dispositivo para proporcionar información que haga que el software se ejecute y muestre según lo diseñado para el dispositivo.<p>Puede obtener el agente de usuario yendo a <a href="https://www.whatismybrowser.com/detect/what-is-my-user-agent">https://www.whatismybrowser.com/detect/what-is-my-user-agent</a> desde el dispositivo.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Deshabilitado</td> 
      <td>Si se selecciona esta opción, el dispositivo no está disponible para que los usuarios lo seleccionen al revisar las pruebas interactivas.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Crear**.

## Configuración de mensajes emergentes para pruebas

Puede configurar mensajes emergentes en las pruebas para comunicar información general a todos los revisores de su organización.

Puede configurar los mensajes para que aparezcan en las siguientes situaciones:

* **Mensaje al cargar**: Muestra cuándo se abre por primera vez la prueba. Útil para explicar a los usuarios cómo revisar una prueba o proporcionar un descargo de responsabilidad u otro texto legal.
* **Mensaje de decisión**: se muestra cuando un usuario selecciona una decisión sobre una prueba. Útil para proporcionar a los usuarios listas de comprobación para tareas como el cumplimiento de la marca o la normativa. Para obtener información acerca de las decisiones, consulte [Tomar una decisión sobre una prueba en el visor de pruebas](../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).

* **Confirmar texto de botón**: La etiqueta que aparece en el botón del mensaje emergente Al cargar explicado anteriormente.

Para crear mensajes emergentes para las pruebas:

1. Haga clic en **Editar** a la derecha del mensaje que desea personalizar.
1. Especifique un mensaje, incluya el formato adecuado y luego haga clic en **Guardar**.
1. (Opcional) Si personalizó el mensaje Al cargar y también desea personalizar la etiqueta del botón de confirmación, haga clic en **Editar** a la derecha de **Confirmar texto del botón**, especifique una etiqueta y, a continuación, haga clic en **Guardar**.

## Configurar valores predeterminados de revisión

Para obtener información acerca de cómo configurar los valores predeterminados de prueba para su organización, consulte [Configurar los valores predeterminados de prueba](../../../administration-and-setup/manage-workfront/configure-proofing/configure-default-proof-settings.md).


## Configurar valores predeterminados de uso compartido

Puede especificar con quién se pueden compartir las pruebas de su organización, qué versiones están disponibles para los revisores y cuándo las pruebas con un flujo de trabajo automatizado son visibles para los usuarios asociados a una fase determinada.

Para obtener información más detallada sobre cómo compartir la configuración en Workfront Proof, consulte [Configurar opciones de uso compartido para los usuarios](../../../administration-and-setup/manage-workfront/configure-proofing/configure-sharing-settings-users.md).

## Marcar el sitio de Workfront Proof

Si utiliza Workfront Proof, puede configurar la promoción de la marca en las siguientes áreas del sitio:

* La página de bienvenida que se muestra cuando se carga la prueba
* Pantallas de inicio y cierre de sesión
* Notificaciones por correo electrónico

Para obtener información detallada sobre cómo personalizar la marca del sitio de Workfront Proof, consulte [Crear una marca en el sitio de Workfront Proof](../../../workfront-proof/wp-acct-admin/branding/brand-wp-site.md).

## Configuración avanzada de contraseñas

>[!IMPORTANT]
>
>Esta opción solo está disponible para planes Workfront heredados. Si tiene un plan Pro, Business o Enterprise Workfront, ya no puede establecer la configuración de contraseña avanzada.

En **Configuración avanzada de contraseñas**, puede mejorar la seguridad de las contraseñas de los usuarios.

1. Haga clic en **Configuración** a la derecha de la configuración que desee configurar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Longitud mínima de la contraseña</td> 
      <td>La longitud predeterminada de la contraseña de Workfront Proof es de seis caracteres. Es posible que desee aumentar el número, según las políticas de su organización.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Mezcla de caracteres</strong> </td> 
      <td>Puede obligar a los usuarios a utilizar una combinación de minúsculas, mayúsculas, números y símbolos en sus contraseñas. Usted decide cuántos caracteres debe contener la contraseña.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Máxima repetición de caracteres</strong> </td> 
      <td>Puede especificar cuántos caracteres se pueden repetir en la contraseña de cada usuario.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Vencimiento automático de contraseña</td> 
      <td>Obliga a los usuarios a cambiar su contraseña con regularidad. Tú decides con qué frecuencia lo harán.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>No se permiten repeticiones de contraseña</strong> </td> 
      <td>Configure el número de repeticiones de contraseña no permitidas en su cuenta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Bloqueo de perfil</strong> </td> 
      <td>Bloquea a los usuarios fuera de la cuenta después de una serie de intentos de inicio de sesión erróneos que especifique. También puede especificar cuánto tiempo deben esperar antes de que puedan acceder a su cuenta de nuevo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear usuario si la contraseña no se restablece después de 30 días</td> 
      <td>Si el usuario no cambia su contraseña inicial en un plazo de 30 días a partir de la activación de su perfil, se le bloquea la cuenta.<br><p>Los administradores de cuentas pueden desbloquear (reactivar) a los usuarios que el sistema bloquee automáticamente. Esto les dará siete días adicionales para cambiar su contraseña.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Bloquear cuenta de usuario si está inactiva durante 120 días</td> 
      <td>Si el usuario no inicia sesión en Workfront Proof o si se requiere una revisión para el inicio de sesión durante 120 días, se le bloquea la cuenta.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Cambiar contraseña después del primer inicio de sesión</strong> </td> 
      <td>Requiere que los usuarios cambien su contraseña temporal después de iniciar sesión por primera vez.<p>Los administradores de cuentas pueden desbloquear (reactivar) a los usuarios que el sistema haya bloqueado automáticamente.</p><p>Para obtener más información sobre la contraseña, consulta <a href="../../../workfront-proof/wp-getstarted/faqs/log-in-change-password.md" class="MCXref xref">Iniciar sesión y cambiar la contraseña y el correo electrónico para Workfront Proof</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>
