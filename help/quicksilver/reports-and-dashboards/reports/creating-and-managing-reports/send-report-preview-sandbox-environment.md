---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Enviar un informe en el entorno de zona protegida de vista previa
description: 'La información de esta página hace referencia a una funcionalidad que solo está disponible en los entornos de zona protegida de vista previa y de actualización personalizada. Esta funcionalidad no está disponible en el entorno de producción. '
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 70bda5a7186abfa7e8cbd26e25a4c58583a322b4
workflow-type: tm+mt
source-wordcount: '625'
ht-degree: 98%

---

# Enviar un informe en el entorno de zona protegida de vista previa

<!-- Audited: 11/2024 -->

La información de esta página hace referencia a una funcionalidad que solo está disponible en los entornos de zona protegida de vista previa y de actualización personalizada. Esta funcionalidad no está disponible en el entorno de producción. 

Puede configurar las opciones de Envío de informes en cualquier entorno de prueba de Adobe Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Aunque los entornos de prueba están pensados para funcionar lo más estrechamente posible con el entorno de producción, algunas funcionalidades difieren de las del entorno de producción.

Puede programar informes en los entornos de prueba, pero la forma en que se envían difiere de cómo se envían desde el entorno de producción.

Para obtener información sobre la programación de informes para su envío en el entorno de producción, consulte [Información general sobre el envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Según la ubicación en la que programe los informes, la funcionalidad de envío difiere entre las zonas protegidas de Vista previa y Actualización personalizada.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
      <td> 
      <p>Nuevo:</p>
         <ul>
         <li><p>Estándar</p></li>
         </ul>
      <p>Actual:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso de edición a informes, paneles y calendarios</p> <p>Acceso de edición a filtros, vistas y agrupaciones</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p></td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Programar informes en el entorno de vista previa

* [Programar informes en el entorno de vista previa](#schedule-reports-in-the-preview-environment)

### Programar informes en el entorno de vista previa

El hecho de que un informe enviado se produzca o no en el entorno de vista previa depende de si la opción **Recibir correos electrónicos de este entorno de prueba** está habilitada o no.

Para obtener información sobre cómo habilitar correos electrónicos desde el entorno de zona protegida, consulte [Habilitar el envío de correos electrónicos desde el entorno de zona protegida de vista previa](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![Recibir correos electrónicos de la opción de espacio aislado](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

Programar informes para su envío en el entorno de vista previa es idéntico a la programación de informes en el entorno de producción. Para obtener información sobre cómo programar el envío de un informe, consulte [Información general sobre el envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Cuando se programa un informe para su envío en el entorno de vista previa, se presentan los siguientes escenarios:

* Cuando **Recibir correos electrónicos de este entorno de prueba** está deshabilitado para el usuario que va a recibir el informe, no se genera ningún archivo al programar el informe para su envío.
* Cuando **Recibir correos electrónicos de este entorno de prueba** está habilitado para el usuario que va a recibir el informe, el archivo que se genera al programar el informe para su envío se añade a la pestaña Documentos del usuario.

## Programar informes en el entorno de zona protegida de actualización personalizada

El hecho de que un informe enviado se produzca o no en la zona protegida de actualización personalizada depende de si la opción Recibir correos electrónicos de este entorno de prueba está habilitada o no.

Para obtener información sobre cómo habilitar los mensajes de correo electrónico del entorno de vista previa, consulte la sección [Ver y modificar la configuración de las notificaciones por correo electrónico](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) en el artículo [Modificar sus propias notificaciones por correo electrónico](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![Recibir correos electrónicos de la opción de espacio aislado](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La programación de informes para su envío en el entorno de zona protegida de actualización personalizada es idéntica a la programación de informes en el entorno de producción. Para obtener información sobre cómo programar el envío de un informe, consulte [Información general sobre el envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Cuando se programa un informe para su envío en el entorno de zona protegida de actualización personalizada, se presentan los siguientes escenarios:

* Cuando la opción Recibir correos electrónicos de este entorno de prueba está desactivada para el usuario que va a recibir el informe, no se genera ningún archivo al programar el informe para su envío.
* Cuando la opción Recibir correos electrónicos de este entorno de prueba está habilitada para el usuario que va a recibir el informe, el informe se envía por correo electrónico como archivo adjunto a la dirección de correo electrónico asociada al usuario.

## Cómo se notifica a los usuarios externos

Los usuarios externos no reciben informes enviados desde los entornos de prueba de Workfront ni notificaciones por correo electrónico.

Los usuarios externos solo reciben informes por correo electrónico si se envían desde un entorno de producción.
