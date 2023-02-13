---
product-area: projects
navigation-topic: manage-issues
title: Copiar problemas
description: Puede copiar un problema o una solicitud y guardarlos en el mismo proyecto o en otro. También puede copiar un problema de una tarea a otro proyecto.
author: Alina
feature: Work Management
exl-id: a28adc22-825f-401e-9ed2-efddaa297b8d
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '936'
ht-degree: 1%

---

# Copiar problemas

Puede copiar un problema o una solicitud y guardarlos en el mismo proyecto o en otro. También puede copiar un problema de una tarea a otro proyecto.

Puede copiar problemas de los siguientes objetos:

* De un proyecto al mismo proyecto (duplique en el mismo proyecto)
* De una tarea a la misma tarea (duplicado si se encuentra en la misma tarea)
* De un proyecto a otro
* De una tarea a un proyecto

>[!TIP]
>
>Los &quot;problemas&quot; y las &quot;solicitudes&quot; se utilizan de forma intercambiable en Workfront. Puede registrar problemas tanto en proyectos como en tareas para indicar el trabajo imprevisto que debe solucionarse. También puede enviar solicitudes que se registren como problemas en un proyecto designado como cola de solicitud.

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
   <td> <p>Solicitud o superior</p> <p>Revise o una licencia superior para copiar un problema en la sección Problemas de un proyecto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Nivel de acceso*</td> 
   <td> <p>Editar acceso a Problemas</p> <p>Ver o acceder más a Proyectos y tareas</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre el acceso a los problemas en el nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md" class="MCXref xref">Concesión de acceso a problemas</a>. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos para el problema</p> <p>Permisos de Contribute para el elemento en el que está copiando el problema con la capacidad de Agregar problemas.</p> <p> Para obtener información sobre la concesión de permisos a problemas, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-an-issue.md" class="MCXref xref">Compartir un problema </a></p> <p>Para obtener información sobre la solicitud de permisos adicionales, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre problemas asociados con documentos o colas de solicitud

Tenga en cuenta lo siguiente al copiar problemas que contienen documentos o que están asociados a una cola de solicitudes:

* **Cuando un problema está asociado con una cola de solicitudes:** Cuando copia un problema en otro objeto y el problema está asociado con una cola de solicitudes, el problema copiado ya no está asociado con la cola original desde la que se originó el primer problema.
* **Cuando se adjunta un documento al problema:** Cuando copia un problema en otro objeto y el problema tiene un documento adjunto, el documento y sus versiones también pasan al nuevo problema. Las pruebas o aprobaciones asociadas al documento no se mueven.
* **Cuando un problema está vinculado a un documento o a una carpeta:** Cuando copia un problema que tiene documentos o carpetas vinculados a un servicio de terceros como Google Drive, los vínculos a los documentos se transfieren al problema copiado. 

## Copiar problemas en una lista

Puede copiar uno o varios problemas de una lista de problemas o de un informe de problemas.

1. Vaya al proyecto que contenga el problema o los problemas que desee copiar.

   O

   Vaya a un informe de problemas.

1. Si seleccionó ir a un proyecto, haga clic en **Problemas** en el panel izquierdo.
1. Seleccione el problema o los problemas que desea copiar y haga clic en el botón **Más menú** en la parte superior de la lista de problemas, haga clic en **Copiar en**.

   ![](assets/copy-issue-in-list-nwe-350x169.png)

1. Continúe copiando el problema, tal como se describe en la sección [Copiar un solo problema](#copy-a-single-issue) a partir del paso 2.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE:&nbsp;ensure step number stays accurate)
   </MadCap:conditionalText>
   -->

## Copiar un solo problema {#copy-a-single-issue}

Puede copiar un problema al verlo.

1. Vaya a un problema que desee copiar y, a continuación, haga clic en el botón **Más** menú ![](assets/more-icon.png) a la derecha del nombre del problema, **Copiar** a.

   ![](assets/nwe-copy-at-issue-level-highlighted-350x580.png)

   La variable **Copiar problema** se muestra.

   ![](assets/copy-issue-box-nwe-350x285.png)

1. En el **Seleccionar proyecto de destino** , especifique el nombre del proyecto en el que desea copiar los problemas. El nombre del proyecto actual se muestra de forma predeterminada.

   >[!TIP]
   >
   >En la lista solo se muestran 100 proyectos.

1. (Condicional) Haga clic en **acceso de solicitud** si no tiene acceso para copiar problemas en el proyecto.
1. (Condicional) Siga copiando el problema en el proyecto de destino seleccionado sin solicitar acceso si tiene acceso para agregar problemas a una de las tareas del proyecto de destino.

   ![](assets/copy-issue-request-access-from-project-nwe-350x125.png)

   >[!TIP]
   >
   >Se muestran mensajes similares si el proyecto seleccionado está pendiente de aprobación, completado o muerto, cuando el administrador de Workfront evita agregar problemas a estos proyectos. Para obtener más información, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

1. (Opcional) En la **Opciones** , desmarque cualquiera de los elementos enumerados en la tabla siguiente para eliminarlos del nuevo problema. Todas las opciones están seleccionadas de forma predeterminada.

   >[!NOTE]
   Esto afecta únicamente a los problemas copiados, no a los problemas originales.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Asignaciones</td> 
      <td>Elimina los usuarios, las funciones de trabajo o los equipos que están asignados al problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Progreso</td> 
      <td>Elimina el porcentaje completado, si lo hay, del problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Documentos</td> 
      <td><span style="line-height: 1.5;">Quita todo lo que aparece en la ficha documentos, incluidas las versiones de documentos, los documentos vinculados y las carpetas.</span> <br>De forma predeterminada, las pruebas y aprobaciones del documento no se pueden copiar en otro problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Permisos</td> 
      <td>Elimina las entidades con las que se comparte el problema. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actualizaciones</td> 
      <td>Elimina los comentarios de la sección Actualizaciones del problema.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Datos personalizados</td> 
      <td>Quita la información del formulario personalizado sobre el problema, así como la información sobre los formularios personalizados asociados con documentos adjuntos al problema, si también se copian con el problema. Los formularios personalizados permanecerán adjuntos a los problemas y documentos, pero la información sobre los formularios no se transmitirá al nuevo problema. </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) En la **Seleccionar tarea** , seleccione la tarea a la que desea mover el problema.
1. Haga clic en **Copiar problema** o **Copiar problemas** si ha seleccionado varios problemas en una lista.

   Los problemas copiados se añaden al proyecto especificado.

 
