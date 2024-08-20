---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configurar opciones de uso compartido para los usuarios
description: Como administrador de Adobe Workfront o de Workfront Proof, puede configurar las cuentas de usuario con las que se pueden compartir las pruebas, si los usuarios pueden ver todas las versiones de una prueba y el momento en el que los usuarios obtienen acceso a los elementos compartidos.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
source-git-commit: ab774e937a15aaa04704e872579df880a9b80aaf
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 0%

---

# Configure las opciones de uso compartido para los usuarios

Como administrador de Adobe Workfront o de Workfront Proof, puede configurar las cuentas de usuario con las que se pueden compartir las pruebas, si los usuarios pueden ver todas las versiones de una prueba y el momento en el que los usuarios obtienen acceso a los elementos compartidos.

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

## Configurar el uso compartido con otras cuentas

{{step1-to-proofing}}

1. Haga clic en **Configuración** > **Configuración de la cuenta** y, a continuación, haga clic en la ficha **Configuración**.

1. En la sección **Compartir**, a la derecha de **Permitir compartir con**, haga clic en **Configurar**.

1. En la lista desplegable que aparece, seleccione una opción para especificar si desea que las pruebas estén disponibles para cualquier persona, restringir el uso compartido de las pruebas solo a su propia cuenta o restringirlo a su propia cuenta y a cualquier cuenta de socio con la que esté colaborando.
1. Haga clic en **Guardar.**

## Configurar la visibilidad de todas las versiones de una revisión compartida

{{step1-to-proofing}}

1. Haga clic en **Configuración** > **Configuración de la cuenta** y, a continuación, haga clic en la ficha **Configuración**.

1. En la sección **Compartir**, a la derecha de **Los destinatarios pueden ver todas las versiones**, seleccione **Habilitar** o **Deshabilitar** para indicar si desea permitir que los destinatarios vean todas las versiones de una prueba dentro del visor de revisión cuando la URL de prueba esté habilitada.

## Configure la visibilidad de la prueba en función de la actividad de fase del flujo de trabajo

Puede especificar cuándo los usuarios asociados a una fase determinada pueden ver las pruebas con un flujo de trabajo automatizado.

>[!NOTE]
>
>* Esta opción solo está disponible cuando se utiliza la aplicación independiente de Workfront Proof; no está disponible cuando se utiliza una instancia de Workfront Proof integrada con Workfront o cuando se realiza una prueba en Workfront.
>* Los usuarios reciben una notificación por correo electrónico sobre la prueba solo después de que entre en la fase a la que está asociado el usuario, independientemente de esta configuración.
>

Para configurar cuándo los usuarios pueden ver las pruebas con un flujo de trabajo automatizado:

{{step1-to-proofing}}

1. Haga clic en **Configuración** > **Configuración de la cuenta** y, a continuación, haga clic en la ficha **Configuración**.

1. En la sección **Compartir**, habilite o deshabilite la **visibilidad de la prueba según la activación de la fase**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Deshabilitado</strong> (predeterminado)</td> 
      <td>Los usuarios pueden ver las pruebas en el momento en que se crean.<br><p>Cualquier usuario asociado con una fase del flujo de trabajo para la prueba puede verla en los resultados de búsqueda inmediatamente después de crearla.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Habilitado</strong> </td> 
      <td> <p>Los usuarios solo pueden ver las pruebas una vez que la fase con la que están asociados se haya vuelto <strong>activa.</strong></p> <p><b>NOTA</b>:   
        <ul> 
         <li><em style="font-style: normal;">Después de habilitar esta opción, las revisiones existentes seguirán siendo visibles para los usuarios que puedan verlas cuando se crearon.</em> </li> 
         <li>Una vez que un usuario obtiene acceso a una versión de una prueba (porque la fase con la que está asociado se activa), solo puede ver la versión en la que está activada la fase. Si una versión anterior nunca llegó a la fase a la que está asociado el usuario, este no podrá ver esa versión de la prueba.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
