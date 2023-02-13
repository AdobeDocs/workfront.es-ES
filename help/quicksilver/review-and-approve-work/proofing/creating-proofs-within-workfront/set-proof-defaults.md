---
product-area: documents
navigation-topic: create-proofs-within-workfront
title: Configuración de los valores predeterminados de pruebas personales
description: Puede definir la configuración predeterminada de prueba personal que se aplica a las pruebas que cree. Estos valores predeterminados se aplican cada vez que se genera una prueba por primera vez o se carga una nueva versión de prueba en Workfront.
author: Courtney
feature: Digital Content and Documents
exl-id: 278bff89-0305-407b-9def-d06820d908de
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# Configuración de los valores predeterminados de pruebas personales

Puede definir la configuración predeterminada de prueba personal que se aplica a las pruebas que cree. Estos valores predeterminados se aplican cada vez que se genera una prueba por primera vez o se carga una nueva versión de prueba en Workfront.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o superior</p> <p>o</p> <p>Plan heredado: Seleccionar o superior</p> <p>Para obtener más información sobre la prueba de acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de pruebas en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o plan</p> <p>Plan heredado: Cualquiera (debe tener las pruebas habilitadas para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Administrador o superior</td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Configuración de los valores predeterminados de pruebas personales

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Prueba**.

1. En la esquina superior derecha, haga clic en el avatar y seleccione **Configuración personal**.
1. Elija la **Valores predeterminados de prueba** y, a continuación, especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td colspan="2"><strong>Configuración predeterminada de notificaciones por correo electrónico</strong> </td> 
     </tr> 
     <tr> 
      <td>Alerta de correo electrónico predeterminada</td> 
      <td>Seleccione la frecuencia con la que el usuario recibe las actualizaciones de correo electrónico. Seleccione Toda la actividad, Respuestas a mis comentarios, Decisiones, Decisión final, Resumen por hora, Resumen diario o Deshabilitado.</td> 
     </tr> 
     <tr> 
      <td>Alerta de correo electrónico predeterminada para nuevos revisores invitados</td> 
      <td>Seleccione la frecuencia con la que los revisores invitados reciben actualizaciones de correo electrónico. Las opciones son las mismas que para la alerta de correo electrónico predeterminada.</td> 
     </tr> 
     <tr> 
      <td>Nueva notificación de prueba</td> 
      <td>Elija recibir una notificación cuando se añada a una prueba.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Configuración del mensaje</strong> </td> 
     </tr> 
     <tr> 
      <td>Plantilla del asunto de prueba</td> 
      <td>Escriba lo que desea que vean los usuarios en el asunto de un correo electrónico cuando comparta una prueba con ellos.</td> 
     </tr> 
     <tr> 
      <td>Plantilla de mensaje de prueba</td> 
      <td>Escriba lo que desea que vean los usuarios en el cuerpo de un correo electrónico cuando comparta una prueba con ellos.</td> 
     </tr> 
     <tr> 
      <td colspan="2"><strong>Configuración de prueba predeterminada</strong> </td> 
     </tr> 
     <tr> 
      <td>Bloquear la prueba cuando se toman todas las decisiones</td> 
      <td>Elija bloquear automáticamente la prueba de cambios posteriores después de tomar todas las decisiones.</td> 
     </tr> 
     <tr> 
      <td>Solo se requiere una decisión</td> 
      <td>Elija requerir una sola decisión en una prueba.</td> 
     </tr> 
     <tr> 
      <td>Inicio de sesión requerido</td> 
      <td> <p>Elija si la prueba solo está disponible para los usuarios con credenciales de inicio de sesión de prueba de Workfront.</p> <p>Nota: Las credenciales de prueba de Workfront pueden ser diferentes a las de Workfront, a menos que el SSO de los usuarios de la empresa. Solo se recomienda utilizar esta función si los usuarios de SSO de la empresa son usuarios de SSO.</p> </td> 
     </tr> 
     <tr> 
      <td>Suscripción habilitada</td> 
      <td>Permita que los revisores externos a la organización se registren para la prueba a través de la URL pública o el código incrustado. Cuando se selecciona esta opción, el suscriptor debe hacer clic en un vínculo de un correo electrónico para acceder a una prueba que también está disponible. Seleccione esta opción para requerir que el revisor externo haga clic en un vínculo dentro del correo electrónico para acceder a la prueba. Esta opción está habilitada de forma predeterminada si la opción Public sharing está seleccionada y se aplica a todas las pruebas creadas por este usuario. </td> 
     </tr> 
     <tr> 
      <td>Función predeterminada para los nuevos revisores invitados</td> 
      <td>Seleccione una función de prueba predeterminada para los revisores invitados. Las opciones son las mismas que las de la función de prueba predeterminada .</td> 
     </tr> 
     <tr> 
      <td>Bloquear la descarga del archivo original</td> 
      <td>Elija bloquear la descarga del archivo original por parte de los usuarios. </td> 
     </tr> 
     <tr> 
      <td>Mi función de prueba predeterminada</td> 
      <td>Elija la función de prueba predeterminada. </td> 
     </tr> 
     <tr> 
      <td>Mi color de marcado predeterminado</td> 
      <td>Elija el color de marcado predeterminado. </td> 
     </tr> 
    </tbody> 
   </table>
