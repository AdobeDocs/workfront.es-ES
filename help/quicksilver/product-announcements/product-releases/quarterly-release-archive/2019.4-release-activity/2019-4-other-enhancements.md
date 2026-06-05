---
content-type: release-notes
navigation-topic: 2019-4-release-activity
title: Otras mejoras de la versión 2019.4
description: Esta página describe varias mejoras realizadas con la versión 2019.4. Estará disponible en el entorno de producción la semana del 11 de noviembre de 2019.
author: Luke
feature: Product Announcements
recommendations: noDisplay, noCatalog
exl-id: ed7488f1-2076-4160-97f3-a3da25cccd0f
TQID: https://experienceleague.adobe.com/YIrC0bPIlY8yLTVQ5VlsYctwXFu-fV5syuqmmh7i5ek
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
  - id: f48b5020-b9cd-4d99-bc6e-42c35e90c1f8
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 566
ht-degree: 51%

---

# Otras mejoras de la versión 2019.4

Esta página describe varias mejoras realizadas con la versión 2019.4. Estará disponible en el entorno de producción la semana del 11 de noviembre de 2019.

Para obtener una lista de todos los cambios realizados en 2019.4, consulte [Información general de la versión 2019.4](../../../../product-announcements/product-releases/quarterly-release-archive/2019.4-release-activity/2019-4-release-activity-overview.md).

<table style="table-layout:auto"> 
 <col> 
 <tbody> 
  <tr> 
   <td> <strong>Iniciar un flujo de trabajo de revisión automatizado desde un documento de Adobe CC</strong> <p>Sin salir de Adobe CC, puede iniciar un flujo de trabajo de revisión automatizado para un documento de Adobe CC que haya creado. Para obtener más información, consulte la sección <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md#generate" class="MCXref xref" xrefformat="{para}">Generar una prueba desde Illustrator o InDesign</a> en el artículo <a href="../../../../documents/workfront-for-adobe-creative-cloud/use-wf-adobe-cc.md" class="MCXref xref" xrefformat="{para}">Usar la extensión de Workfront para Illustrator y InDesign</a>.</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td><strong>Workfront G Suite add-on</strong> <p>Now you can manage Workfront objects directly from Gmail, Google Calendar, and Google Drive.</p> <p>When you open a Workfront notification email, instantly view all information about the associated object and take actions, such as reviewing content or updating a status, without leaving your Inbox.</p> <p>When you open a non-Workfront email:</p> 
     <ul> 
      <li>Convert it into a task or issue.</li> 
      <li>Associate it with a project.</li> 
      <li>Assign it as a work item.</li> 
      <li>Add it to a work item as an update.</li> 
      <li>Upload its attachments to Workfront.</li> 
     </ul> <p>Manage Workfront objects without leaving G Suite:</p> 
     <ul> 
      <li>Post updates and replies to comments.</li> 
      <li>View and manage documents associated with a task or issue.</li> 
     </ul> <p>Access and work with object details:</p> 
     <ul> 
      <li>Read the description</li> 
      <li>View the parent object</li> 
      <li>Change the status</li> 
      <li>Access custom data</li> 
      <li>Mark it as complete.</li> 
     </ul> <p>And access your Workfront Home content, including tasks, issues, approvals, and access requests, without leaving G Suite.</p> <p>For more information, see <a href="../../../../workfront-integrations-and-apps/workfront-for-g-suite/workfront-for-gsuite.md" class="MCXref xref" xrefformat="{para}">Adobe Workfront for G Suite</a>.</p> </td> 
   </tr>
  --> 
  <tr> 
   <td> <strong>Impedir direcciones de correo electrónico duplicadas</strong> <p>Ya no puede utilizar la misma dirección de correo electrónico al crear varios usuarios en Workfront, aunque esas direcciones de correo electrónico varíen según el caso. Por ejemplo, no se puede crear un usuario con la dirección de correo electrónico de JohnDoe@example.com y otro usuario con la dirección de correo electrónico de johndoe@example.com. </p> <p>Antes de este cambio, se admitía la creación de usuarios con direcciones de correo electrónico coincidentes que solo diferían según el caso. </p> <p>Nota: Los usuarios existentes con direcciones de correo electrónico coincidentes que solo difieran en función del caso deberán actualizarse en una fecha futura. Si tiene usuarios en una instancia de Workfront con direcciones de correo electrónico coincidentes que solo difieren según el caso, Workfront se pondrá en contacto con usted para proporcionarle información adicional y una cronología cuando sea necesario actualizarlas.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Tipos de objeto adicionales disponibles para los campos de escritura anticipada en un formulario personalizado</strong> 
     <p>Ahora, al crear un campo personalizado de escritura anticipada, puede asociar los siguientes tipos de objetos al campo: Usuario, Empresa, Grupo, Función de trabajo, Portfolio, Programa, Proyecto y Plantilla.</p> 
     <p>Anteriormente, solo se podía asociar el tipo de objeto Usuario con un campo personalizado de escritura anticipada.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> <strong>Se muestra el nombre de archivo de la última versión de un documento</strong> <p>Ahora, cuando se carga una versión de documento con un nombre de archivo diferente al de la versión existente, el nuevo nombre de archivo se muestra en Workfront.</p> <p>Anteriormente, cuando se agregaba una nueva versión con un nombre de archivo diferente, el nombre de archivo de la versión anterior seguía apareciendo en Workfront.</p> <p>Para obtener más información, consulte <a href="../../../../documents/managing-documents/upload-new-document-version.md" class="MCXref xref" xrefformat="{para}">Cargar una nueva versión de un documento</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <strong>Añadir un filtro a un campo Typeahead en un formulario personalizado</strong> <p>Ahora, cuando añada un campo Typeahead a un formulario personalizado, puede añadir un filtro para limitar los objetos disponibles cuando alguien utiliza el campo. Por ejemplo, puede limitar el campo para que el usuario pueda seleccionar solo miembros de los equipos de marketing y ventas de su organización.</p> <p>Para obtener más información, consulte la sección Crear y añadir un nuevo campo en el artículo Creación de formularios personalizados.</p> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Cambiar el tipo de visualización de un campo en un formulario personalizado</strong> 
     <p>Ahora puede cambiar el tipo de visualización de un campo en un formulario personalizado.</p> 
     <p>Por ejemplo, si ha creado un campo Casillas de verificación, puede cambiarlo por un campo Desplegable o por un campo Botones de opción. Estos tres tipos de visualización de campo son intercambiables.</p> 
     <p>O bien, si ha creado un campo de texto de una única línea, puede cambiarlo por un campo de texto de párrafo. Estos dos tipos de visualización de campo son intercambiables.</p> 
     <p>Anteriormente, para cambiar el tipo de visualización de un campo personalizado, se tenía que crear un nuevo campo y eliminar el antiguo. Esto requería transferir datos, lo que a menudo llevaba mucho tiempo.</p> 
    </div> </td> 
  </tr> 
  <tr> 
   <td> 
    <div> 
     <strong>Creación de calendarios e informes de días libres</strong> 
     <p>Ahora puede ver el tiempo libre del usuario para una mejor planificación y ejecución. También puede añadir nuevos informes y calendarios de días libres a sus paneles de control para obtener una vista en tiempo real de la disponibilidad del usuario.</p> 
    </div> </td> 
  </tr> 
 </tbody> 
</table>
