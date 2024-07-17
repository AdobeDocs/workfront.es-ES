---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Enviar un informe en el entorno de vista previa de espacio aislado
description: La información de esta página hace referencia a funcionalidades que solo están disponibles en los entornos de vista previa y zona protegida de actualización personalizada. Esta funcionalidad no está disponible en el entorno de producción.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: f6335f4e94d286681adfb50165562b2c41b5acac
workflow-type: tm+mt
source-wordcount: '658'
ht-degree: 0%

---

# Enviar un informe en el entorno de vista previa de espacio aislado

La información de esta página hace referencia a funcionalidades que solo están disponibles en los entornos de vista previa y zona protegida de actualización personalizada. Esta funcionalidad no está disponible en el entorno de producción.

Puede configurar las opciones de Entrega de informes en cualquier entorno de prueba de Adobe Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Aunque los entornos de prueba están pensados para funcionar lo más cerca posible del entorno de producción, algunas funcionalidades difieren de las del entorno de producción.

Puede programar informes en los entornos de prueba, pero la forma en que se envían difiere de cómo se envían desde el entorno de producción.

Para obtener información sobre la programación de informes para su envío en el entorno de producción, consulte [Resumen de envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Según la ubicación en la que programe los informes, la funcionalidad de entrega difiere entre los entornos limitados de Vista previa y Actualización personalizada.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, vea <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a los objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Programar informes en el entorno de vista previa

* [Programar informes en el entorno de vista previa](#schedule-reports-in-the-preview-environment)

### Programar informes en el entorno de vista previa

El que un informe enviado se produzca o no en el entorno de vista previa depende de si **Recibir correos electrónicos de este entorno de prueba** está habilitado o no.

Para obtener información sobre cómo habilitar correos electrónicos desde el entorno de espacio aislado, consulte [Habilitar el envío de correos electrónicos desde el entorno de vista previa de espacio aislado](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

Programar informes para su envío en el entorno de vista previa es idéntico a programar informes en el entorno de producción. Para obtener información sobre cómo programar la entrega de un informe, consulte [Resumen de la entrega de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Cuando se programa un informe para su envío en el entorno de vista previa, se presentan los siguientes escenarios:

* Cuando **Recibir correos electrónicos de este entorno de prueba** está deshabilitado para el usuario que recibe el informe, no se genera ningún archivo al programar el informe para su envío.
* Cuando **Recibir correos electrónicos de este entorno de prueba** está habilitado para el usuario que recibe el informe, el archivo que se genera al programar el informe para su envío se agrega en la pestaña Documentos del usuario.

## Programar informes en el entorno de espacio aislado de actualización personalizado

El que un informe entregado se produzca o no en la zona protegida de actualización personalizada depende de si la configuración Recibir correos electrónicos de este entorno de prueba está habilitada o no.

Para obtener información sobre cómo habilitar los mensajes de correo electrónico desde el entorno de vista previa, consulte la sección [Ver y modificar la configuración de las notificaciones por correo electrónico](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) en el artículo [Modificar sus propias notificaciones por correo electrónico](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La programación de informes para su envío en el entorno de espacio aislado de actualización personalizado es idéntica a la programación de informes en el entorno de producción. Para obtener información sobre cómo programar la entrega de un informe, consulte [Resumen de la entrega de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Cuando se programa el envío de un informe en el entorno de espacio aislado de actualización personalizado, se dan los siguientes escenarios:

* Cuando la opción Recibir correos electrónicos de este entorno de prueba está desactivada para el usuario que recibe el informe, no se genera ningún archivo al programar el informe para su envío.
* Cuando la opción Recibir correos electrónicos de este entorno de prueba está habilitada para el usuario que recibe el informe, este se envía por correo electrónico como archivo adjunto a la dirección de correo electrónico asociada al usuario.

## Notificación a los usuarios externos

Los usuarios externos no reciben informes enviados desde los entornos de prueba de Workfront ni notificaciones por correo electrónico.

Los usuarios externos solo reciben informes por correo electrónico si se envían desde un entorno de producción.
