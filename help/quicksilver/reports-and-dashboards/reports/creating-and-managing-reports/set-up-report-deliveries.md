---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: Resumen del envío de informes
description: Resumen del envío de informes
author: Nolan
feature: Reports and Dashboards
exl-id: 1637df59-ca1d-4cf6-b83d-2b27936cdb96
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1528'
ht-degree: 0%

---

# Resumen del envío de informes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This is linked to the UI in the Send Report box inside the Preview sandbox. If you change title, log bug for Dev to fix the link) </p>
-->

Los informes se pueden programar para que se envíen automáticamente a los usuarios según una programación definida, o bien se pueden enviar de forma manual y única. Cuando se envía un informe desde Adobe Workfront, el usuario recibe un mensaje de correo electrónico con el informe de Workfront en un archivo adjunto independiente.

Para obtener información sobre la configuración de un informe para su envío, consulte el artículo [Programar un envío automático de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

No es posible programar informes para su envío ni enviarlos manualmente en el entorno de espacio aislado de vista previa. Para obtener más información sobre el Simulador para pruebas de vista previa, consulte el artículo [Entorno de espacio aislado de vista previa de Adobe Workfront](../../../administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md).\
Para obtener más información sobre la entrega de informes en el entorno de la zona de pruebas de vista previa, consulte el artículo [Enviar un informe en el entorno de la zona de pruebas de vista previa](../../../reports-and-dashboards/reports/creating-and-managing-reports/send-report-preview-sandbox-environment.md).

## Límites de entrega de informes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: [! This information is shared between "Exporting Data" and "Setting Up Report Deliveries."])</p>
-->

Tenga en cuenta lo siguiente al programar informes para su envío:

* Se pueden programar hasta 10 envíos de informes repetitivos para un informe determinado.
* Puede programar el envío de un informe únicamente si es el creador del informe. Si necesita enviar un informe que no ha creado, puede enviarlo manualmente.

## Límites de exportación

Existen varios límites de tamaño que afectan a la forma en que se muestran los informes en Workfront y a su exportación mediante una exportación manual, un informe entregado o la API:

* **Tamaño de archivo de 5 MB:** Límite de tamaño de archivo para cualquier informe exportado programado para su envío. Si un archivo exportado adjunto a un correo electrónico supera los 5 MB, se envía un vínculo en el que se puede descargar el archivo por correo electrónico en lugar del informe exportado adjunto. 

   >[!NOTE]
   >
   >Los archivos .xlsx de Excel de más de 5 MB no generan correos electrónicos. Puede exportar manualmente el informe a este formato. Para obtener información sobre la exportación de informes, consulte [Exportar datos](../../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md).

* **50 000 filas:** Número de filas de datos permitidas en una exportación de informe para archivos .pdf y Delimitados por tabuladores.

   Para los archivos .xls de Excel, este límite es **65 000 filas**.

   Para los archivos .xlsx de Excel, este límite es **100 000 filas**.

   Estos límites excluyen los encabezados de columna, así como las filas para las agrupaciones en el informe. Por ejemplo, si tiene 6 agrupaciones en un informe y 50 000 filas o datos, el archivo exportado tendrá 50 000 filas.

   Si el informe tiene más elementos que estos límites, se produce un error que indica que la exportación y el envío del informe no se han realizado correctamente. Reduzca el número de elementos que ve en la pantalla a un número menor o igual que estos límites para poder ofrecer los resultados. Si desea exportar todos los datos, le sugerimos que utilice filtros para obtener cargas de datos más pequeñas y, a continuación, realice varias exportaciones. Para obtener más información, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

   Estos límites se aplican a:

   * Exportación manual de un informe.
   * Un informe programado.
   * Una exportación a través de una integración de API. 
   * Datos exportados mediante un inicio.

      Para obtener más información sobre la exportación de datos mediante los primeros pasos, consulte el artículo [Exportar datos de Adobe Workfront mediante Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

      >[!NOTE]
      Puede exportar 50 000 filas en un archivo de inicio inicial, pero solo en un archivo en formato Excel. 

   * Exportación de información de uso para un proyecto.

      Para obtener más información sobre la exportación de información de uso para un proyecto, consulte [Resumen del informe de Utilización de Recursos](../../../reports-and-dashboards/reports/using-built-in-reports/resource-utilization-report.md).

* **65.530 hipervínculos:** Este es un límite impuesto por Excel a los documentos que contienen más de 65.530 hipervínculos. Estos documentos no se pueden abrir cuando se exportan manualmente o se envían en un informe enviado. Tenga en cuenta que un documento de Excel puede tener solo 200 filas de datos, pero si hay más de 65.530 vínculos dentro del documento, el documento no se abre. Este límite existe solo en archivos de Excel, no en los demás formatos admitidos. 
* **256 columnas**: Este es un límite impuesto por Excel a los documentos que contienen más de 256 columnas. Estos documentos no se pueden exportar manualmente ni enviar en un informe enviado. Este límite existe solo en archivos de Excel, no en los demás formatos admitidos. 

Si intenta exportar datos más allá del límite, es posible que no reciba todos los datos esperados en la exportación. Por el contrario, se produce un informe modificado dentro del límite. 

Además, se detendrán los informes que tarden más de 60 minutos en ejecutarse.

Si tiene dudas o problemas con respecto a su límite, póngase en contacto con el servicio de asistencia técnica de Workfront.

## Explicación de las marcas de hora en los informes entregados

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Note about if this is delivered at a time based on the user's time zone settings?)</p>
-->

Al recibir un informe en un mensaje de correo electrónico, es posible que la marca de tiempo y el formato de hora del informe no coincidan con los de Workfront si desea ver el informe en Workfront al mismo tiempo que se entregó. 

Tenga en cuenta lo siguiente: 

* Al ver un informe en el explorador, la marca de tiempo y el formato del informe coinciden con la configuración regional y la zona horaria del explorador, tal como se define en la configuración del explorador.
* Cuando el informe se envía por correo electrónico, el informe lleva la marca de tiempo y el formato que coincidan con la configuración regional y la zona horaria del usuario tal como se especifican en el perfil de Workfront.\
   Para obtener más información sobre la configuración regional y la zona horaria del usuario en Workfront, consulte el artículo [Edición del perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

## Informes con una vista especial {#reports-with-a-special-view}

Cuando se aplica una vista especial a un informe, la vista especial aparece en la ficha Detalles del informe en Workfront.

Cuando se programa la entrega de un informe que tiene una vista especial, la pestaña Detalles predeterminada se envía en el adjunto del correo electrónico enviado, en lugar de en la vista especial.

Se consideran opiniones especiales las siguientes:

* Vista Milestone en un informe de proyecto
* Vista Gantt en un informe de proyecto o tarea
* Informes con un gráfico como ficha predeterminada

>[!NOTE]
Si también hay una ficha Matriz en el informe además de la ficha predeterminada con una vista especial, el informe se envía tal como aparece en la ficha Matriz.

Para obtener más información sobre cómo aplicar una vista especial a un informe, consulte el artículo [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## Usar el archivo entregado

 Cuando se envía un informe desde Workfront, el usuario recibe un mensaje de correo electrónico con el informe en un archivo adjunto independiente. 

* [Línea de asunto, nombre de archivo adjunto y título del informe](#subject-line-attachment-name-and-report-title)
* [Marcas de hora](#timestamps)
* [Personalización de marca](#branding)
* [Formato](#formatting)
* [Vínculos](#links)

### Línea de asunto, nombre de archivo adjunto y título del informe {#subject-line-attachment-name-and-report-title}

Para obtener más información sobre la línea de asunto del correo electrónico del informe enviado, consulte [Programar un envío automático de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).

El nombre del informe adjunto es: *The_Name_Of_The_Report* seguido del formato de archivo exportado. 

Si programó el informe enviado para que tenga formato de PDF o de HTML, el título del informe será:

*Nombre del informe.*

Los informes programados para enviarse en formato Excel, Excel (.xlsx) o TSV no tienen título.

>[!NOTE]
Si el informe tiene una descripción, se incluirá en el archivo exportado si el archivo tiene el formato de PDF o de HTML.

### Marcas de hora {#timestamps}

La marca de tiempo se muestra en el archivo adjunto solo si el formato del archivo es .pdf. La marca de tiempo se encuentra en el pie de página del archivo adjunto.

La marca de tiempo incluye:

* Fecha
* Hora
* Zona horaria en la que se envió el informe

### Personalización de marca {#branding}

Si el administrador de Workfront ha añadido marcas personalizadas a la instancia de Workfront, los informes enviados en formato .pdf también incluyen el logotipo personalizado.

Los informes enviados en todos los demás formatos no se pueden personalizar con su logotipo.

Para obtener más información sobre la marca de la instancia de Workfront, consulte el artículo [Marca la instancia de Adobe Workfront](../../../administration-and-setup/customize-workfront/brand-workfront/brand-your-workfront-instance.md).

### Formato {#formatting}

Siempre recibe la pestaña predeterminada de un informe cuando se envía o se programa un informe para una entrega, a menos que el informe tenga una vista especial.

Si el informe tiene un formato especial en la aplicación web, el informe debe entregarse con el formato especial cuando las pestañas Details y Matrix se envíen solo para archivos .pdf y Excel.

El filtro, la vista o la agrupación del informe no se incluyen en el archivo enviado. La descripción del informe se incluye únicamente cuando se envía el informe como archivo de PDF.

Para obtener más información sobre la recepción de informes con una vista especial, consulte el artículo [Informes con una vista especial](#reports-with-a-special-view).\
Para obtener más información sobre la selección de la ficha predeterminada de un informe y sobre el formato especial, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

### Vínculos {#links}

Cuando se envía un informe desde Workfront al formato de PDF o Excel, los vínculos de trabajo que existan en el documento original permanecerán activos en el archivo enviado. Los vínculos pueden apuntar a cualquier objeto de Workfront que admita la vinculación.

El nombre del informe en el mensaje de correo electrónico también es un vínculo.

## Informar sobre informes programados

Puede ver si un informe se ha configurado para enviarse creando lo siguiente:

* **Una vista** para el objeto Informe de una lista o un informe para informes: Cree una vista en una lista de informes o en un informe para informes, y agregue la siguiente columna a la vista:\
   *Nombre del informe programado.\
   *Los nombres de todos los envíos programados para ese informe se enumeran en la columna de una lista con viñetas.\
   ![scheduled_reports_info_in_view.png](assets/scheduled-reports-info-in-view-350x294.png)

* **Un filtro** para el objeto Informe : cree un filtro en una lista de informes o en un informe de informes con la siguiente instrucción: *El ID del informe programado no está en blanco*.\
   Esto mostrará únicamente los informes que se han programado en su lista o informe.\
   ![](assets/qs-scheduled-report-filter-350x101.png)\
   Para obtener más información sobre la creación de informes, consulte [Crear un informe personalizado](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md). Para obtener información sobre la creación de informes, consulte [Crear un informe sobre las actividades de informes](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Scheduling a Repeating&nbsp;Report Delivery</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can schedule up to 10 repeating report deliveries for any given report.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can schedule a report to be delivered only if you are the creator of the report. If you need to send a report that you did not create, you can send it on a manual basis.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To schedule&nbsp;a report for automatic delivery or to edit an existing report delivery:&nbsp;​</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report for which you want to schedule delivery.&nbsp;</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The <strong>Send Report</strong> dialog box is displayed.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Select the <strong>Repeating Deliveries</strong>&nbsp;tab.<br><img src="assets/report-delivery-schedule-350x169.png" alt="" style="width: 350;height: 169;"></li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">(Conditional)&nbsp;To modify an existing repeating report delivery, select the report delivery in the <strong>Repeating Deliveries</strong>&nbsp;section.</li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Specify the following information:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Send to:</strong> Begin typing the name of the user, group, team, or role who you want to send&nbsp;the report to, then click the name when it appears in the drop-down list.<br>Or<br>Specify the email address of a person external to the Workfront system who you want to have access to the report.<br> Repeat this process to send the report to multiple users, groups, teams, or roles.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Subject:</strong> Specify a subject for the email notification.<br> By default, the email subject is: <em>Workfront Report: <Name of the report> Date of the Export</em>.<strong></strong></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Message:</strong> Specify a message to include in the email.<br>By default, the email message is:&nbsp;<em>Attached is the <report frequency> report <Name of the report> generated by Workfront on <Date>.</em><br>
   <note type="note">
   For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks.&nbsp;Please go back to the report scheduler&nbsp;to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report.&nbsp;
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Deliver this report with the Access Rights of:</strong>&nbsp;Begin typing the name of a user who has access to the report, then click the name when it appears&nbsp;in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify&nbsp;here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>
   <note type="note">
   This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Format:</strong> Select in which of the following formats you want the report to be delivered:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> HTML</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">PDF</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS&nbsp;Excel</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel (.xlsx)</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">TSV &nbsp;</li>
   </ul></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Include Links:</strong>&nbsp;This option is available&nbsp;only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document. <br>Documents that contain more than 65,530 links cannot be opened. If the exported document will contain more than 65,530 links, deselect this option.<br>This option is enabled by default.&nbsp;</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Summary:</strong> Displays a summary of when the delivery repeats.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats:</strong> Select whether the report should be delivered daily, weekly, monthly, or yearly.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats Every:</strong> Select the frequency with which you want&nbsp;the delivery to repeat. The value you select for this option is&nbsp;based on the option that is selected in the <strong>Repeats</strong>&nbsp;drop-down list.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Time:</strong> Select the time of day for the delivery to be sent.</li>
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Repeats On:</strong>&nbsp;This option is available when the <strong>Repeats</strong>&nbsp;option is set to either <strong>Weekly</strong>&nbsp;or <strong>Monthly</strong>.</p>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the <strong>Repeats</strong>&nbsp;option is set to <strong>Weekly</strong>: Select the days of the week that the delivery is sent.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">When the <strong>Repeats</strong>&nbsp;option is set to <strong>Monthly</strong>: Select whether the delivery is sent on the day of the month, day of the week, or last day of the month (these options leverage the date that you select in the <strong>Starts On</strong>&nbsp;field).</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Starts On:</strong> Select the date for the scheduled delivery to begin.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Ends On:</strong> Select a date for the scheduled delivery to end. <br>Or</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Select <strong>Never</strong>&nbsp;if you want the scheduled delivery to last indefinitely.</li>
   -->

<!--
   <li value="6" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Save</strong>&nbsp;to save the report delivery.<br> The report is saved in the <strong>Repeating Deliveries</strong>&nbsp;section&nbsp;(in the <strong>Send Report</strong> dialog box).<br> The report will be sent at the schedule time<br>Or<br>To manually send the report, click <strong>Send Now</strong>.<br>For more information about sending the report instantly or manually, see&nbsp;.</li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Deleting a Scheduled Report Delivery</h2>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Go to the report with the delivery you want to delete.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then <strong>Send Report</strong>.&nbsp;</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Repeating Deliveries</strong>.&nbsp;</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the name of the scheduled delivery you want to delete, then click <strong>Delete</strong>. The report is no longer set up for the scheduled delivery.&nbsp;</li>
   -->

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Sending a Report Manually, on a One-Time Basis</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can manually send a report&nbsp;that has been previously scheduled, or you can create a single-use report delivery.​</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a title="Setting Up Report Deliveries" href="#sending-a-scheduled-report-now" class="MCXref xref">Sending a Scheduled Report Now</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a title="Setting Up Report Deliveries" href="#sending-a-report-one-time-only" class="MCXref xref">Sending a Report (One Time Only)</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="sending-a-scheduled-report-now">Sending a Scheduled Report Now</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">After a scheduled report has been set up, you can manually send the report rather than&nbsp;waiting until the scheduled time.</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report that you want to send now.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The Send Report dialog box is displayed.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click the <strong>Repeating Deliveries</strong> tab.</li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Repeating Deliveries</strong>&nbsp;section, select the report delivery that was previously created.<br><img src="assets/report-delivery-schedule-send-350x160.png" alt="" style="width: 350;height: 160;"></li>
   -->

<!--
   <li value="5" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Send Now</strong>.<br> The report is sent to all users identified in the scheduled delivery.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="sending-a-report-one-time-only">Sending a Report (One Time Only)</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can manually send a report at any time. When you send a report in this way, delivery information (such as&nbsp;the users you are sending to and&nbsp;the email subject) are not saved. If you want to create a report delivery that you can save for later use, create a repeating scheduled report.&nbsp;</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">To send a report to users (one time only):</p>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">Navigate to and click the name of the report that you want to send now.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Report Actions</strong>, then&nbsp;<strong>Send Report</strong>.<br> The <strong>Send Report</strong> dialog box is displayed.<br><img src="assets/report-delivery-sendnow-350x351.png" alt="" style="width: 350;height: 351;"></li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">On the <strong>Send Now</strong>&nbsp;tab, specify the following information:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Send to:</strong> Begin typing the name of the user, group, team, or role who you want to send&nbsp;the report to, then click the name when it appears in the drop-down list.&nbsp;Or, specify the email address of a person external to the Workfront system who you want to have access to the report.<br> Repeat this process to send the report to multiple users, groups, teams, or roles.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Subject:</strong> Specify a subject for the email notification.<br> By default, the email subject is: <em>Workfront Report: <Name of the report> Date of the Export</em>.</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Email Message:</strong> Specify a message to include in the email.<br>By default, the email message is:&nbsp;<em>Attached is the <report frequency> report <Name of the report> generated by Workfront on <Date>.</em><br>
   <note type="note">
   For reports delivered as an Excel file only, the following message is also added to the email: "Please be aware that with MS Excel (XLS) file types, there is a limit (65,530) on the number of hyperlinks these file types support. If you exceed those limits, your file will not open and it is recommended to resend without the hyperlinks.&nbsp;Please go back to the report scheduler&nbsp;to remove hyperlinks and resend the report." The "please go back to the report scheduler" phrase is a link back to the report.&nbsp;
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Deliver this report with the Access Rights of:</strong>&nbsp;Begin typing the name of a user who has access to the report, then click the name when it appears&nbsp;in the drop-down list. Users who receive the report will be granted the same level of access to the report as the user that you specify&nbsp;here.<br> For more information, see <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Run and deliver a report with the access rights of another user</a>.
   <note type="note">
   This field does not support wildcards. For example, using the wildcard $$User.ID does not run the report with the access rights of the user who is receiving the report.
   </note>
   </li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Format:</strong> Select in which of the following formats you want the report to be delivered:
   <ul>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> HTML</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">PDF</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS Excel</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">MS&nbsp;Excel (.xlsx)</li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode">TSV</li>
   </ul></li>
   <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Include Links:</strong>&nbsp;This option is available&nbsp;only when <strong>MS Excel</strong> is selected in the <strong>Format</strong> drop-down menu. When this option is enabled, any hyperlinks are included in the exported Excel document. <br>Documents that contain more than 65,000 links cannot be opened. If the exported document will contain more than 65,000 links, deselect this option.<br>This option is enabled by default.</li>
   </ul></li>
   -->

<!--
   <li value="4" data-mc-conditions="QuicksilverOrClassic.Draft mode">Click <strong>Send Now</strong>.<br> The report is sent to all users that you identified.<br> Or<br> Click <strong>Make Repeating Delivery</strong>&nbsp;if you want to set up&nbsp;a scheduled delivery with this same information, then complete the additional information regarding the frequency of when the report is sent.</li>
   -->
