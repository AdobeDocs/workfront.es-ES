---
title: Habilitar un Workspace de Workfront Planning en GenStudio for Performance Marketing
description: Si ya tiene un espacio de trabajo en Adobe Workfront Planning, puede habilitarlo para GenStudio for Performance Marketing en lugar de volver a crear los datos.
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 0747fb80-496f-41c0-b469-1203e1605f05
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/wHSc0Neshdl-Owh1siw72wdO-H1hnEPy-dAk91tDOrI
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
source-git-commit: 0bcb6ef2abbf3789339af27119422ef413cd6eef
workflow-type: tm+mt
source-wordcount: '513'
ht-degree: 2%
---
# Habilitar un espacio de trabajo de Workfront Planning en GenStudio for Performance Marketing

{{planning-important-intro}}

<!-- THIS IS HIDDEN FROM TOC-->

<!--
Better metadata, at publishing:
---
title: Promote a Workfront Planning workspace to GenStudio
description: The GenStudio for Performance Marketing workspace is available in Adobe Workfront Planning when your company has purchased both products and your instance of Workfront is integrated with your company's instance of GenStudio. You can promote a Workfront Planning workspace to GenStudio and have its information visible and updated from both systems.
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
---
-->
Además de Workfront Planning, si su empresa también compró Adobe GenStudio for Performance Marketing, el espacio de trabajo de GenStudio está disponible en Adobe Workfront Planning cuando la instancia de Workfront está integrada con la instancia de GenStudio de su empresa.

Si ya tiene un espacio de trabajo en Workfront Planning, puede habilitarlo para GenStudio en lugar de volver a crear los datos.

Al habilitar un espacio de trabajo, se vincula a un proyecto de almacenamiento de Adobe y se asignan sus tipos de registros y campos al esquema de espacio de trabajo de GenStudio. Una vez completada la configuración, puede abrir los registros del espacio de trabajo en GenStudio.

Tenga en cuenta lo siguiente:

* Debe tener acceso a Workfront Planning y a GenStudio for Performance Marketing.
* Debe tener un proyecto de almacenamiento en la nube de Adobe para vincularlo al espacio de trabajo. Un administrador de organización puede crear uno en Adobe Admin Console.

  Para obtener más información, consulte [Administrar almacenamiento de Adobe](https://helpx.adobe.com/business/enterprise/manage-storage-assets/manage-storage/manage-adobe-storage.html). <!--ensure this site still works-->


## Habilitar un espacio de trabajo de Workfront Planning en GenStudio

1. En Workfront Planning, abra el espacio de trabajo que desee habilitar.
1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del área de trabajo y, a continuación, haga clic en **Habilitar GenStudio**.

   El cuadro **Hacer que el espacio de trabajo GenStudio** esté habilitado se abre con los siguientes pasos:

   1. **Proyecto ACPC**: Seleccione el **Proyecto ACPC** (proyecto de almacenamiento en la nube de Adobe) que desea sincronizar con este espacio de trabajo y, a continuación, haga clic en **Siguiente**. Los usuarios acceden al espacio de trabajo en GenStudio a través de este proyecto.

      ![Habilitar GenStudio en el espacio de trabajo - Paso del proyecto ACPC](assets/make-workspace-genstudio-enabled-box-acpc-step.png)

   1. **Tipos de registros**: asigne los tipos de registros del área de trabajo a los seis tipos de registros que requiere GenStudio:

      * Campañas
      * Productos
      * Personas
      * Canales
      * Regiones
      * Activaciones

      Para cada uno, abra la lista y seleccione el tipo de registro de Planning correspondiente, o bien seleccione **Agregar nuevo** para crearlo y luego haga clic en **Siguiente**.

      ![Habilitar GenStudio en el espacio de trabajo - Paso de tipos de registro](assets/make-workspace-genstudio-enabled-box-record-types-step.png)

   1. **Campos**: Asigne los campos para cada tipo de registro. Utilice las pestañas de la parte superior del cuadro de diálogo para desplazarse entre los tipos de registro. Para cada campo, seleccione el campo Planning correspondiente o seleccione **Agregar nuevo** para crearlo.

      Repita la configuración del campo para todos los tipos de registros.

      ![Habilitar GenStudio en el espacio de trabajo - Paso Campos](assets/make-workspace-genstudio-enabled-box-fields-step.png)

   1. Revise y corrija cualquier advertencia.

      Por ejemplo, un nuevo campo puede convertirse en el campo principal del tipo de registro o se cambia el nombre de un alias de campo que ya está en uso (si ya tiene un campo denominado &quot;Regiones&quot;, el importado puede convertirse en &quot;Regiones 2&quot;).

      Al asignar un campo **Status** se agregan las opciones necesarias.

   1. Haga clic en **Publicar**.

      Aparecerá un mensaje de confirmación cuando el espacio de trabajo esté activado. Los tipos de registros asignados se marcan en el espacio de trabajo.

      Los tipos de registro asignados para que sean accesibles desde GenStudio tienen un nuevo icono **Adobe** en sus tarjetas.

      ![Tipo de registro de campañas con icono de Adobe](assets/campaigns-record-type-card-with-adobe-icon.png)

1. Abra GenStudio, seleccione **Campañas** y luego haga clic en el **proyecto ACPC** que configuró originalmente para esta configuración en la esquina inferior izquierda de la pantalla. Revise los campos y tipos de registro importados.

   >[!TIP]
   >
   >Solo verá los registros que permita la pertenencia al proyecto ACPC.
