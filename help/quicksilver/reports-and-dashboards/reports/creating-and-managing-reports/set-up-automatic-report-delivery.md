---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Programar un envío automático de informes
description: Programar un envío automático de informes
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 3%

---

# Programar un envío automático de informes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

Los informes se pueden programar para que se entreguen automáticamente a los usuarios según una programación definida, o bien se pueden enviar manualmente de forma única. Cuando se envía un informe desde Adobe Workfront, el usuario recibe un mensaje de correo electrónico con el informe de Workfront en un archivo adjunto independiente.

Para obtener más información, incluidas las limitaciones de tamaño que pueden afectar a la entrega de los informes, consulte [Resumen del envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

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

## Requisitos previos

Antes de comenzar, debe crear un informe. Para obtener más información sobre la creación de informes, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Programar el envío de informes

Para programar un informe para su envío automático o para editar o eliminar un envío de informe existente: &#x200B;

1. Vaya a un informe que desee programar para su envío.

   >[!NOTE]
   >
   >Los envíos de informes no contienen mensajes. Si desea limitar los datos de un envío de informe, le recomendamos que aplique filtros al informe que desea enviar.

1. Haga clic en **Acciones de informe**, luego **Enviar informe**.

   La variable **Enviar informe** se abre.

   >[!TIP]
   >
   >Para enviar un informe manualmente en un momento dado, vaya al informe y haga clic en **Acciones de informe** > **Enviar informe** > **Enviar ahora**.

1. Seleccione el **Repetición de envíos** pestaña .
1. (Condicional) Para modificar un envío de informe repetido existente, seleccione el envío de informe en la **Repetición de envíos** para obtener más información.
1. Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Enviar a</p> </td> 
      <td> <p>Comience a escribir el nombre del usuario, grupo, equipo o función al que desee enviar el informe y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.</p> <p>O</p> <p>Especifique la dirección de correo electrónico de una persona externa al sistema de Workfront a la que desee tener acceso al informe.</p> <p>Repita este proceso para enviar el informe a varios usuarios, grupos, equipos o funciones.</p> <p>Nota:  <p>Tenga en cuenta lo siguiente al agregar destinatarios de envíos de informes:</p> 
        <ul> 
         <li>Si su organización restringe las notificaciones de Workfront a dominios de correo electrónico específicos, es posible que solo pueda enviar informes a las direcciones de correo electrónico enumeradas en la lista de permitidos de correo electrónico.<p>Para obtener información sobre cómo un administrador de Workfront actualiza la lista de permitidos de correo electrónico, consulte la sección <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Configurar la lista de permitidos de correo electrónico</a>.</p></li> 
         <li> <p>Añadir un gran número de usuarios como destinatarios puede provocar que la entrega falle. Si se producen errores en la entrega, puede programar varios envíos de informes con grupos de usuarios más pequeños.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Asunto de correo electrónico</p> </td> 
      <td> <p>Especifique un asunto para la notificación por correo electrónico.</p> <p>De forma predeterminada, el asunto del correo electrónico es:</p> <p><em>Informe de Workfront: [Nombre del informe] [Fecha]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Mensaje de correo electrónico</p> </td> 
      <td> <p>Especifique un mensaje para incluirlo en el correo electrónico.</p> <p>De forma predeterminada, el mensaje de correo electrónico es:</p> <p><em>Se adjunta el informe [frecuencia del informe] [Nombre del informe] generado por Workfront el [Fecha].</em> </p> <p>Nota: Para los informes entregados solo como archivo de Excel, también se agrega el siguiente mensaje al correo electrónico: "Tenga en cuenta que con los tipos de archivo de Microsoft Excel (XLS), hay un límite (65.530) en el número de hipervínculos que admiten estos tipos de archivo. Si supera estos límites, el archivo no se abrirá y se recomienda volver a enviar sin los hipervínculos. Vuelva al programador de informes para eliminar los hipervínculos y reenviar el informe". La frase "por favor, vuelva al programador de informes" es un vínculo al informe.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Entregar este informe con los derechos de acceso de</p> </td> 
      <td> <p>Empiece a escribir el nombre de un usuario que tenga acceso al informe y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable. A los usuarios que reciban el informe se les otorgará el mismo nivel de acceso que al usuario especificado aquí.<br> Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Ejecutar y enviar un informe con los derechos de acceso de otro usuario</a>.</p> <p>Nota: Este campo no admite caracteres comodín. Por ejemplo, el uso del comodín $$User.ID no ejecuta el informe con los derechos de acceso del usuario que recibe el informe.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Formato</p> </td> 
      <td> <p>Seleccione el formato que desee para el informe enviado:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Si selecciona esta opción, puede dar formato a la salida utilizando el complemento <strong>Tamaño del papel</strong> y <strong>Orientación</strong> opciones que se muestran.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Incluir enlaces</p> </td> 
      <td> <p>Esta opción solo está disponible cuando <strong>MS Excel</strong> se selecciona en la variable <strong>Formato</strong> menú desplegable. Cuando esta opción está activada, los hipervínculos se incluyen en el documento de Excel exportado.</p> <p>Los documentos que contienen más de 65.530 vínculos no se pueden abrir. Si el documento exportado contiene más de 65.530 vínculos, anule la selección de esta opción.</p> <p>Esta opción está activada de forma predeterminada.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Resumen</p> </td> 
      <td> <p>Muestra un resumen de cuándo se repite la entrega.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se repite</p> </td> 
      <td> <p>Seleccione si el informe debe entregarse diariamente, semanalmente, mensualmente o anualmente.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se repite cada</p> </td> 
      <td> <p>Seleccione la frecuencia con la que desea que se repita la entrega. El valor que seleccione para esta opción se basa en la opción seleccionada en la variable <strong>Repetidas</strong> lista desplegable.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Hora</p> </td> 
      <td> <p>Seleccione la hora del día para el envío.</p> <p>Sugerencia: Como las cargas del sistema pueden afectar a los tiempos de entrega de los informes, puede haber un retraso entre la hora programada y la hora de entrega real. Si necesita que un informe se envíe en un momento específico, recomendamos programar la entrega antes del momento en que sea necesario. Por ejemplo, se recomienda programar la entrega un día antes de la fecha en la que es necesario.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se repite el</p> </td> 
      <td> <p>Esta opción está disponible cuando la variable <strong>Repetidas</strong> se configura como <strong>Semanal</strong> o <strong>Mensual</strong>:</p> 
       <ul> 
        <li> <p>Cuando la variable <strong>Repetidas</strong> está configurada en <strong>Semanal</strong>: Seleccione los días de la semana en que se realiza la entrega.</p> </li> 
        <li> <p>Cuando la variable <strong>Repetidas</strong> está configurada en <strong>Mensual</strong>: Seleccione si la entrega se realiza el día del mes, el día de la semana o el último día del mes (estas opciones aprovechan la fecha seleccionada en la variable <strong>Comienza en</strong> ).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se inicia los</p> </td> 
      <td>Seleccione la fecha en la que comenzará la entrega programada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Finaliza el</p> </td> 
      <td>Seleccione una fecha para finalizar el envío programado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Nunca</p> </td> 
      <td>Select <strong>Nunca</strong> si desea que la entrega programada dure indefinidamente.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar** para guardar el envío de informes.

   El informe se muestra en la sección **Repetición de envíos** (en la sección **Enviar informe** ) y se enviará a la hora programada.

   Para obtener información sobre las limitaciones de tamaño que pueden afectar a la entrega de los informes, consulte las secciones [Límites de entrega de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) y [Límites de exportación](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

1. (Opcional) Para eliminar un envío programado:

   1. En el **Repetición de envíos** , haga clic en el envío programado y, a continuación, haga clic en **Eliminar**.
   1. Haga clic en **Eliminar** para confirmar.

## Tutorial de vídeo

Vea el siguiente vídeo para aprender a programar una entrega de informes. Este vídeo se grabó en Workfront Classic. Sin embargo, el contenido también se aplica a la nueva experiencia de Workfront.

[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->
