---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configuración del uso compartido para los usuarios
description: Como administrador de Adobe Workfront o de Workfront Proof, puede configurar las cuentas de usuario con las que se pueden compartir pruebas, si los usuarios pueden ver todas las versiones de una prueba y el momento en el que los usuarios obtienen acceso a los elementos compartidos.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '607'
ht-degree: 0%

---

# Configuración del uso compartido para los usuarios

Como administrador de Adobe Workfront o de Workfront Proof, puede configurar las cuentas de usuario con las que se pueden compartir pruebas, si los usuarios pueden ver todas las versiones de una prueba y el momento en el que los usuarios obtienen acceso a los elementos compartidos.

## Requisitos de acceso

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o superior</p> <p>o</p> <p>Plan heredado: Premium o Select</p> <p>Para obtener más información sobre la prueba de acceso con los diferentes planes, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de pruebas en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o plan</p> <p>Plan heredado: Cualquiera (debe tener las pruebas habilitadas para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe tener el administrador seleccionado en el perfil de permisos de prueba. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configuración del acceso de prueba de un usuario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Configurar el uso compartido con otras cuentas

1. En Workfront, haga clic en el menú principal ![](assets/main-menu-icon.png)y, a continuación, haga clic en Prueba ![](assets/proofing-in-main-menu.png) para acceder a Workfront Proof.

1. Haga clic en **Configuración** > **Configuración de la cuenta** y, a continuación, haga clic en el botón **Configuración** pestaña .

1. En el **Uso compartido** a la derecha de **Permitir compartir con**, haga clic en **Configuración**.

1. En la lista desplegable que aparece, seleccione una opción para especificar si desea que las pruebas estén disponibles para cualquier persona, restringir el uso compartido de las pruebas únicamente a su propia cuenta o restringirlo a su propia cuenta y a las cuentas de socio con las que esté colaborando.
1. Haga clic en **Guardar.**

## Configuración de la visibilidad de todas las versiones de una prueba compartida

1. En Workfront, haga clic en el menú principal ![](assets/main-menu-icon.png)y, a continuación, haga clic en Prueba ![](assets/proofing-in-main-menu.png) para acceder a Workfront Proof.

1. Haga clic en **Configuración** > **Configuración de la cuenta** y, a continuación, haga clic en el botón **Configuración** pestaña .

1. En el **Uso compartido** a la derecha de **Los destinatarios pueden ver todas las versiones**, seleccione **Habilitar** o **Deshabilitar** para indicar si desea permitir que los destinatarios vean todas las versiones de una prueba en el visor de pruebas cuando la URL de prueba esté habilitada.

## Configuración de la visibilidad de la prueba en función de la actividad de la fase de flujo de trabajo

Puede especificar cuándo las pruebas con un flujo de trabajo automatizado son visibles para los usuarios asociados a un escenario determinado.

>[!NOTE]
>
>* Esta opción solo está disponible cuando se utiliza la aplicación independiente de prueba de Workfront; no está disponible cuando se utiliza una instancia de prueba de Workfront integrada con Workfront o al realizar pruebas en Workfront.
>* Los usuarios reciben una notificación por correo electrónico sobre la prueba solo después de que entre en la fase a la que está asociado el usuario, independientemente de esta configuración.
>


Para configurar cuándo los usuarios pueden ver las pruebas con un flujo de trabajo automatizado:

1. En Workfront, haga clic en el menú principal ![](assets/main-menu-icon.png)y, a continuación, haga clic en Prueba ![](assets/proofing-in-main-menu.png) para acceder a Workfront Proof.

1. Haga clic en **Configuración** > **Configuración de la cuenta** y, a continuación, haga clic en el botón **Configuración** pestaña .

1. En el **Uso compartido** sección, activar o desactivar **Visibilidad de la prueba basada en la activación de la etapa**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Desactivado</strong> (predeterminado)</td> 
      <td>Las pruebas son visibles para los usuarios en el momento en que se crea la prueba.<br><p>Cualquier usuario asociado con un paso en el flujo de trabajo para la prueba puede ver la prueba en los resultados de búsqueda inmediatamente después de crear la prueba.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Habilitado</strong> </td> 
      <td> <p>Las pruebas son visibles para los usuarios solo después de que la fase con la que están asociados se convierta en <strong>activa.</strong></p> <p><b>NOTA</b>:   
        <ul> 
         <li><em style="font-style: normal;">Después de activar esta opción, las pruebas existentes siguen estando visibles para los usuarios que podrían verla cuando se crearon.</em> </li> 
         <li>Cuando un usuario obtiene acceso a una versión de una prueba (ya que el escenario con el que está asociado se activa), solo puede ver la versión en la que se activa el escenario. Si una versión anterior nunca llega a la fase a la que está asociado el usuario, este no puede ver esa versión de la prueba.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
