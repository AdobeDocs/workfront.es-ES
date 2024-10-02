---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Programar una entrega automática de informes
description: Programar una entrega automática de informes
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 1723609ce790566c072d071f9ac627dba7dc5350
workflow-type: tm+mt
source-wordcount: '1272'
ht-degree: 2%

---

# Programar una entrega automática de informes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

Puede programar informes para que se entreguen automáticamente a los usuarios según una programación definida, o puede enviar informes manualmente una vez. Cuando envía un informe desde Adobe Workfront, el usuario recibe un correo electrónico con el informe de Workfront en un archivo adjunto independiente.

Para obtener más información, incluidas las limitaciones de tamaño que pueden afectar al envío de los informes, consulte [Resumen de la entrega de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

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

## Requisitos previos

Antes de empezar, debe crear un informe. Para obtener más información sobre la creación de informes, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Programar una entrega de informes

Para programar un informe para su envío automático o editar o eliminar un envío de informe existente:&#x200B;

1. Vaya al informe que desee programar para su envío.

   >[!NOTE]
   >
   >Los envíos de informes no contienen mensajes. Si desea limitar los datos en una entrega de informes, le recomendamos que aplique filtros al informe que desea enviar.

1. Haga clic en **Acciones de informe** y luego en **Enviar informe**.

   Se muestra el cuadro de diálogo **Enviar informe**.

   >[!TIP]
   >
   >Para enviar un informe manualmente en cualquier momento dado, vaya al informe y haga clic en **Acciones de informe** > **Enviar informe** > **Enviar ahora**.

1. Seleccione la ficha **Entregas repetidas**.
1. (Condicional) Para modificar una entrega repetida de informe existente, seleccione la entrega de informe en la sección **Entregas repetidas**.
1. Especifique la siguiente información:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>Enviar a</p> </td> 
      <td> <p>Empiece escribiendo el nombre del usuario, grupo, equipo o rol al que desea enviar el informe y, a continuación, haga clic en el nombre cuando aparezca en la lista desplegable.</p> <p>O</p> <p>Especifique la dirección de correo electrónico de una persona externa al sistema de Workfront a la que desea que tenga acceso al informe.</p> <p>Repita este proceso para enviar el informe a varios usuarios, grupos, equipos o roles.</p> <p>Nota:  <p>Tenga en cuenta lo siguiente al agregar destinatarios de envío de informes:</p> 
        <ul> 
         <li>Si su organización restringe las notificaciones de Workfront a dominios de correo electrónico específicos, es posible que solo pueda enviar informes a las direcciones de correo electrónico que aparecen en la lista de permitidos de correo electrónico.<p>Para obtener información sobre cómo un administrador de Workfront actualiza la lista de permitidos de correo electrónico, consulte la sección <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">Configuración de la lista de permitidos de correo electrónico</a>.</p></li> 
         <li> <p>Añadir un gran número de usuarios como destinatarios puede provocar errores en la entrega. Si se producen errores en las entregas, se pueden programar varios envíos de informes con grupos de usuarios más pequeños.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Asunto de correo electrónico</p> </td> 
      <td> <p>Especifique un asunto para la notificación por correo electrónico.</p> <p>De forma predeterminada, el asunto del correo electrónico es:</p> <p><em>Informe de Workfront: [Nombre del informe] [Fecha]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Mensaje de correo electrónico</p> </td> 
      <td> <p>Especifique un mensaje para incluirlo en el correo electrónico.</p> <p>De forma predeterminada, el mensaje de correo electrónico es:</p> <p><em>Se ha adjuntado el informe [Frecuencia del informe] [Nombre del informe] generado por Workfront el [Fecha].</em> </p> <p>Nota: En el caso de los informes enviados únicamente como archivo de Excel, también se añade el siguiente mensaje al correo electrónico: "Tenga en cuenta que con los tipos de archivo de MS Excel (XLS), hay un límite (65 530) en el número de hipervínculos que admiten estos tipos de archivo. Si supera estos límites, el archivo no se abrirá y se recomienda reenviarlo sin los hipervínculos. Vuelva al programador de informes para eliminar los hipervínculos y reenvíe el informe". La frase "vuelva al programador de informes" es un vínculo que lleva al informe.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Entregar este informe con los derechos de acceso de</p> </td> 
      <td> <p>Empiece escribiendo el nombre de un usuario que tiene acceso al informe y, cuando aparezca en la lista desplegable, haga clic en el nombre. A los usuarios que reciban el informe se les otorgará el mismo nivel de acceso que al usuario que especifique aquí.<br> Para obtener más información, consulte <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Ejecutar y enviar un informe con los derechos de acceso de otro usuario</a>.</p> <p>Nota: Este campo no admite caracteres comodín. Por ejemplo, si se usa el comodín $$User.ID, el informe no se ejecutará con los derechos de acceso del usuario que recibe el informe.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Formato</p> </td> 
      <td> <p>Seleccione el formato que desee para el informe enviado:</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>Si selecciona esta opción, puede dar formato a la salida utilizando las opciones adicionales <strong>Tamaño de papel</strong> y <strong>Orientación</strong> que se muestran.</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Incluir enlaces</p> </td> 
      <td> <p>Esta opción solo está disponible cuando <strong>MS Excel</strong> está seleccionado en el menú desplegable <strong>Formato</strong>. Cuando esta opción está habilitada, todos los hipervínculos se incluyen en el documento de Excel exportado.</p> <p>No se pueden abrir los documentos que contienen más de 65.530 vínculos. Si el documento exportado va a contener más de 65.530 vínculos, anule la selección de esta opción.</p> <p>Esta opción está habilitada de forma predeterminada.</p> </td> 
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
      <td> <p>Seleccione la frecuencia con la que desea que se repita la entrega. El valor que seleccione para esta opción se basa en la opción seleccionada en la lista desplegable <strong>Repeticiones</strong>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Hora</p> </td> 
      <td> <p>Seleccione la hora del día a la que se enviará la entrega.</p> <p>Sugerencia: Debido a que las cargas del sistema pueden afectar a los tiempos de entrega de los informes, puede haber un retraso de hasta 24 horas entre la hora programada y la hora de entrega real. Si necesita que un informe se envíe en un momento específico, le recomendamos que programe la entrega antes del momento en que sea necesario. En general, se recomienda programar la entrega al menos un día antes de la fecha en que es necesario.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se repite el</p> </td> 
      <td> <p>Esta opción está disponible cuando la opción <strong>Repeticiones</strong> está establecida en <strong>Semanal</strong> o <strong>Mensual</strong>:</p> 
       <ul> 
        <li> <p>Cuando la opción <strong>Repite</strong> se establece en <strong>Semanal</strong>: seleccione los días de la semana en que se enviará la entrega.</p> </li> 
        <li> <p>Cuando la opción <strong>Repite</strong> se establece en <strong>Mensual</strong>: selecciona si la entrega se realiza el día del mes, el día de la semana o el último día del mes (estas opciones aprovechan la fecha que seleccionaste en el campo <strong>Comienza el </strong>).</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Se inicia los</p> </td> 
      <td>Seleccione la fecha de inicio de la entrega programada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Finaliza el</p> </td> 
      <td>Seleccione una fecha para que finalice la entrega programada.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Nunca</p> </td> 
      <td>Seleccione <strong>Nunca</strong> si desea que la entrega programada dure indefinidamente.</td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Guardar** para guardar la entrega del informe.

   El informe se muestra en la sección **Envíos repetidos** (en el cuadro de diálogo **Enviar informe**) y se enviará a la hora programada.

   Para obtener información sobre las limitaciones de tamaño que pueden afectar el envío de los informes, consulte las secciones [Límites de envío de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) y [Límites de exportación](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

>[!IMPORTANT]
>
>Los informes programados están sujetos a un límite de tiempo interno cuando se procesan para su envío. En el caso de que el envío de un informe tarde más tiempo que el límite, se le enviará una notificación y el informe dejará de entregarse, independientemente de las entregas programadas restantes. Para continuar enviando el informe, primero intente reducir el tamaño del informe mediante filtros y vistas y, a continuación, cree un nuevo envío programado.
>
>Si está utilizando una entrega de informes programada para analizar los datos de Workfront a través de una herramienta de BI, le recomendamos que utilice Workfront Data Connect en su lugar. Para obtener más información, consulte [Información general sobre Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-lake-overview.md).

1. (Opcional) Para eliminar una entrega programada:

   1. En el panel **Envíos repetidos**, haga clic en el envío programado y, a continuación, haga clic en **Eliminar**.
   1. Haga clic en **Eliminar** para confirmar.

## Introducción a los vídeos

Vea el siguiente vídeo para aprender a programar la entrega de un informe. Este vídeo se grabó en Workfront Classic. Sin embargo, el contenido también se aplica a la nueva experiencia de Workfront.

[![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)

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
