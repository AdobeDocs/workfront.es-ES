---
user-type: administrator
product-area: system-administration;setup
navigation-topic: configure-proofing-functionality
title: Configuración de la revisión predeterminada
description: Esta configuración le permite establecer valores predeterminados que se aplican a todas las pruebas nuevas creadas por los usuarios. Sin embargo, los usuarios pueden anular la mayoría de estos ajustes al crear una prueba.
author: Courtney
feature: System Setup and Administration, Digital Content and Documents
role: Admin
exl-id: cfccb120-8759-49f2-8b7b-dabcd57d4fda
source-git-commit: 5676910e53f1c4f49cab196e42bfbce8704887ca
workflow-type: tm+mt
source-wordcount: '557'
ht-degree: 7%

---

# Configurar ajustes de prueba predeterminados

Esta configuración le permite establecer valores predeterminados que se aplican a todas las pruebas nuevas creadas por los usuarios. Sin embargo, los usuarios pueden anular la mayoría de estos ajustes al crear una prueba.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td>
   <p>Nuevo: estándar</p>
   o
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Debe ser administrador de Workfront. Para obtener información sobre los administradores de Workfront, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo total a un usuario</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

+++

## Configurar nueva configuración predeterminada de revisión

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Pruebas** > **Configuración de pruebas**.
1. En la sección **Nuevos valores predeterminados de prueba**, configure las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Destinatarios</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Inicio de sesión obligatorio</td> 
      <td> <p>Los revisores deben iniciar sesión con su correo electrónico y contraseña antes de poder ver las pruebas creadas en la cuenta de su organización. Cuando está habilitada, los usuarios no pueden compartir la prueba con los revisores invitados.</p> <p><b>IMPORTANT</b>: cuando está habilitada, se requiere el inicio de sesión para todas las revisiones recién creadas.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Copiar propietario de la prueba original para las nuevas versiones</td> 
      <td> <p>El propietario de la primera versión de una prueba es también el propietario de todas las versiones consecutivas de la prueba, independientemente de quién cree estas versiones. Esta opción está habilitada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permite a los usuarios eliminar los comentarios sobre las pruebas</td> 
      <td>Los usuarios pueden eliminar sus propios comentarios. Esta opción está habilitada de forma predeterminada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Requerir que las decisiones se firmen electrónicamente </td> 
      <td> <p>Los responsables de la toma de decisiones deben introducir sus credenciales de inicio de sesión de Workfront cuando tomen una decisión sobre una prueba.</p> <p><b>IMPORTANTE</b>: cuando está habilitada, los usuarios no pueden compartir la revisión con revisores invitados que no tengan credenciales de inicio de sesión.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Fecha límite</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Establecer la fecha límite predeterminada</td> 
      <td> <p>El sistema aplica esta fecha límite a todas las pruebas nuevas de la cuenta que no tengan un flujo de trabajo automatizado.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Notificar a los destinatarios antes de que la prueba esté en riesgo</td> 
      <td>Se notifica a los destinatarios por correo electrónico antes de que la prueba se considere en riesgo según el plazo especificado anteriormente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"><b>Notificaciones por correo electrónico</b></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Informar a los destinatarios cuando se les añada a una prueba</td> 
      <td>Se notifica a los destinatarios por correo electrónico cuando se añaden a una prueba.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar**.

## Configuración de decisiones de prueba

Los usuarios pueden utilizar las decisiones sobre pruebas para indicar el estado de la prueba después de la revisión.

>[!NOTE]
>
>La lógica detrás de las decisiones de prueba se utiliza para calcular el estado general de un flujo de trabajo de prueba si hay varias decisiones en varios niveles. Las decisiones &quot;Aprobado&quot; y &quot;Aprobado con cambios&quot; se aplican al déclencheur de la siguiente etapa de un flujo de trabajo automático.

Para configurar las decisiones de prueba:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Pruebas** > **Configuración de pruebas**.
1. En la sección **Decisiones**, puede

   1. **Cambie el nombre de la decisión**: haga clic en el texto dentro del cuadro de decisión y empiece a escribir la nueva etiqueta de decisión.

      >[!TIP]
      >
      >Conserve la lógica de una decisión cuando le cambie el nombre. Por ejemplo, la decisión predeterminada Rechazado se puede cambiar a *Se requiere una nueva versión*, pero no se debe cambiar a *Enviar a las impresoras*.

      ![](assets/rename-decision-350x109.png)

   1. **Reorganizar el orden de decisión**: arrastre los cuadros de decisión en el orden en que desee que aparezcan en el visor de revisión.

      ![](assets/move-decision-350x110.png)

   1. **Ocultar una decisión**: Pase el ratón sobre el cuadro de decisión y haga clic en el icono Ocultar situado en la esquina superior derecha.

      ![](assets/hide-decision-350x109.png)

1. (Opcional) Para volver a los valores predeterminados de Workfront, haga clic en **Restaurar valores predeterminados**.
1. Haga clic en **Guardar**.
