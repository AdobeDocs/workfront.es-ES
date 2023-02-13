---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Enviar un informe en el entorno de la zona de pruebas de vista previa
description: La información de esta página hace referencia a funciones que solo están disponibles en los entornos de espacio aislado de vista previa y actualización personalizada. Esta funcionalidad no está disponible en el entorno de producción.
author: Nolan
feature: Reports and Dashboards
exl-id: 568360df-bec9-4767-8b5a-32a294d05d47
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '660'
ht-degree: 0%

---

# Enviar un informe en el entorno de la zona de pruebas de vista previa

La información de esta página hace referencia a funciones que solo están disponibles en los entornos de espacio aislado de vista previa y actualización personalizada. Esta funcionalidad no está disponible en el entorno de producción.

Puede configurar las opciones de Entrega de informes en cualquier entorno de prueba de Adobe Workfront.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For information about the Workfront test environments, see the "Workfront Testing Environments" section. (NOTE:&nbsp;drafted - link this section)</p>
-->

Aunque los entornos de prueba están pensados para funcionar lo más cerca posible del entorno de producción, algunas funcionalidades difieren del entorno de producción.

Puede programar informes en los entornos de prueba, pero la forma en que se entregan difiere de cómo se entregan en el entorno de producción.

Para obtener información sobre la programación de informes para su envío en el entorno Producción, consulte [Resumen del envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Según el lugar donde se programen los informes, la funcionalidad de envío difiere entre los entornos limitados Vista previa y Actualización personalizada.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Programar informes en el entorno de vista previa

* [Programar informes en el entorno de vista previa](#schedule-reports-in-the-preview-environment)

### Programar informes en el entorno de vista previa

Si un informe enviado se produce o no en el entorno de Vista previa depende de si **Recibir correos electrónicos de este entorno de prueba** está activada o no.

Para obtener información sobre cómo habilitar correos electrónicos desde el entorno de espacio aislado, consulte [Habilitar el envío de correos electrónicos desde el entorno de Preview Sandbox](../../../workfront-basics/using-notifications/enable-delivery-emails-from-preview-sandbox-environment.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La programación de informes para su envío en el entorno de Vista previa es idéntica a la programación de informes en el entorno de producción. Para obtener información sobre cómo programar un informe para su envío, consulte [Resumen del envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Cuando se programa un informe para su envío en el entorno de Vista previa, existen las siguientes situaciones:

* When **Recibir correos electrónicos de este entorno de prueba** está desactivado para el usuario que recibe el informe, no se genera ningún archivo al programar el informe para su envío.
* When **Recibir correos electrónicos de este entorno de prueba** está habilitado para el usuario que recibe el informe, el archivo que se genera al programar el informe para su envío se agrega en la pestaña del usuario Documentos .

## Programar informes en el entorno de espacio aislado de actualización personalizada

El hecho de que un informe enviado se produzca o no en el Simulador para pruebas de actualización personalizado depende de si la configuración Recibir correos electrónicos de esta prueba está activada o no.

Para obtener información sobre la activación de correos electrónicos desde el entorno de vista previa, consulte la sección [Ver y modificar la configuración de las notificaciones por correo electrónico](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md#view) en el artículo [Activar o desactivar sus propias notificaciones de eventos](../../../workfront-basics/using-notifications/activate-or-deactivate-your-own-event-notifications.md).

![](assets/receive-emails-from-sandbox-setting-edit-350x223.png)

La programación de informes para su envío en el entorno de espacio aislado de actualización personalizado es idéntica a la programación de informes en el entorno de producción. Para obtener información sobre cómo programar un informe para su envío, consulte [Resumen del envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

Cuando se programa un informe para su envío en el entorno de espacio aislado de actualización personalizado, existen las siguientes situaciones:

* Cuando se deshabilita la opción Recibir correos electrónicos de esta prueba para el usuario que recibe el informe, no se genera ningún archivo al programar el envío del informe.
* Cuando la opción Recibir correos electrónicos de este entorno de prueba está habilitada para el usuario que recibe el informe, este se envía por correo electrónico como datos adjuntos a la dirección de correo electrónico asociada al usuario.

## Notificación a los usuarios externos

Los usuarios externos no reciben informes enviados desde los entornos de prueba de Workfront ni reciben una notificación por correo electrónico.

Los usuarios externos solo reciben informes por correo electrónico si se entregan desde un entorno de producción.
