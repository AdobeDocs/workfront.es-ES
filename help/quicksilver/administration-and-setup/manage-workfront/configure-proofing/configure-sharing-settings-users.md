---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configurar opciones de uso compartido para los usuarios
description: Como administrador de Adobe Workfront o de Workfront Proof, es posible configurar las cuentas de usuario con las que se pueden compartir las pruebas, si los usuarios podrán ver todas las versiones de una prueba y el momento en el que los usuarios obtendrán acceso a los elementos compartidos.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: 505c183b-6252-4367-898f-2429824860be
TQID: https://experienceleague.adobe.com/fPxvbgeLZYUO6SU1WUOdU4BJYuGO4pSYWK-4QHSnueU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 580
ht-degree: 98%

---

# Configurar las opciones de uso compartido de los usuarios

Como administrador de Adobe Workfront o de Workfront Proof, es posible configurar las cuentas de usuario con las que se pueden compartir las pruebas, si los usuarios podrán ver todas las versiones de una prueba y el momento en el que los usuarios obtendrán acceso a los elementos compartidos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener lo siguiente:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: pro o superior</p> <p>o</p> <p>Plan heredado: Premium o Select</p> <p>Para obtener más información sobre el acceso de revisión con los diferentes planes, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: trabajo o plan</p> <p>Plan heredado: cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe haber seleccionado Administrador en el perfil de permisos de prueba. Para obtener más información, consulte <a href="../../../administration-and-setup/manage-workfront/configure-proofing/configure-a-users-proofing-access.md" class="MCXref xref">Configurar el acceso de revisión de un usuario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Configurar el uso compartido con otras cuentas

{{step1-to-proofing}}

1. Haga clic en **Configuración** > **Configuración de la cuenta** y, a continuación, haga clic en la pestaña **Configuración**.

1. En la sección **Uso compartido**, a la derecha de **Permitir el uso compartido con**, haga clic en **Configurar**.

1. En la lista desplegable que aparezca, seleccione una opción para especificar si desea que las pruebas estén disponibles para cualquier persona, restringir el uso compartido de las pruebas únicamente a su propia cuenta o restringirlo a su propia cuenta y a cualquier cuenta de socio con la que esté colaborando.
1. Haga clic en **Guardar.**

## Configurar la visibilidad de todas las versiones de una revisión compartida

{{step1-to-proofing}}

1. Haga clic en **Configuración** > **Configuración de la cuenta** y, a continuación, haga clic en la pestaña **Configuración**.

1. En la sección **Uso compartido**, a la derecha de **Los destinatarios pueden ver todas las versiones**, seleccione **Habilitar** o **Deshabilitar** para indicar si desea permitir que los destinatarios vean todas las versiones de una prueba dentro del visualizador de revisión cuando la URL de prueba esté habilitada.

## Configure la visibilidad de la prueba en función de la actividad de fase del flujo de trabajo

Especifique cuándo los usuarios asociados a una fase determinada podrán ver las pruebas con un flujo de trabajo automatizado.

>[!NOTE]
>
>* Esta opción solo estará disponible cuando se utilice la aplicación independiente de Workfront Proof. No estará disponible cuando se utilice una instancia de Workfront Proof integrada con Workfront o cuando se realicen revisiones en Workfront.
>* Los usuarios recibirán una notificación por correo electrónico sobre la prueba solo después de que entre en la fase a la que esté asociado el usuario, independientemente de esta configuración.
>

Para configurar cuándo los usuarios podrán ver las pruebas con un flujo de trabajo automatizado:

{{step1-to-proofing}}

1. Haga clic en **Configuración** > **Configuración de la cuenta** y, a continuación, haga clic en la pestaña **Configuración**.

1. En la sección **Uso compartido**, habilite o deshabilite **Visibilidad de la prueba según la activación de la fase**.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Deshabilitado</strong> (predeterminado)</td> 
      <td>Los usuarios pueden ver las pruebas en el momento en que se crean.<br><p>Cualquier usuario asociado con una fase del flujo de trabajo para la prueba podrá verla en los resultados de búsqueda inmediatamente después de su creación.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Habilitado</strong> </td> 
      <td> <p>Los usuarios solo podrán ver las pruebas una vez que la fase con la que estén asociados se <strong>active.</strong></p> <p><b>NOTA</b>:   
        <ul> 
         <li><em style="font-style: normal;">Después de habilitar esta opción, las revisiones existentes seguirán siendo visibles para los usuarios que puedan verlas cuando se crearon.</em> </li> 
         <li>Una vez que un usuario obtenga acceso a una versión de una prueba (porque la fase con la que esté asociado se active), solo podrá ver la versión en la que esté activada la fase. Si una versión anterior nunca llegó a la fase a la que esté asociado el usuario, este no podrá ver esa versión de la prueba.</li> 
        </ul> </p> </td> 
     </tr> 
    </tbody> 
   </table>
