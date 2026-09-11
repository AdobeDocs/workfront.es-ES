---
title: Crear registros de planificación a partir de breves de espacio de ideas
description: Con el Espacio de ideas, una nueva funcionalidad de Adobe Workfront Planning, puede convertir informes en registros de Planning. Los informes exportados crean registros nuevos o actualizan los existentes. Este artículo describe cómo se pueden crear o editar registros existentes de Planning mediante el espacio de ideación.
role: User, Admin
author: Alina
source-git-commit: 02ea2cad43b1064e30a7356feaa194f98d448092
workflow-type: tm+mt
source-wordcount: '1210'
ht-degree: 2%

---


# Creación de registros de Planning a partir de informes del espacio de ideación

<!--
Will this release JUST to preview? If not - hide the preview portion below
-->

<!--
I started with this under Records first but what if Ideation will be added to other products and it will generate record types in those products? keep it here so it can be moved, if needed, to a standalone product one day?
-->

<!--
*********************** IMPORTANT ***************
THIS ARTICLE HAS 2 DRAFTS IN 2 SEPARATE AREAS FROM CLAUDE - THEY WERE CREATED AT DIFFERENT TIMES - WHICH ONE WOULD YOU KEEP OR MERGE THEM INTO ONE ARTICLE
-->

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible como parte del programa **Beta** del espacio de ideación. </span>

<span class="preview">Para obtener más información, consulte [Introducción al espacio de ideación para Adobe Workfront Planning](/help/quicksilver/planning/ideation/get-started-with-planning-ideation.md).</span>

{{planning-important-intro}}

Con el Espacio de ideas, una nueva funcionalidad de Adobe Workfront Planning, puede convertir informes en registros de Planning. Los informes exportados crean registros nuevos o actualizan los existentes.

Este artículo describe cómo se pueden crear o editar registros existentes de Planning mediante el espacio de ideación.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

<!--
are there additional license restrictions or packages to be purchased to have access to Ideation space?? If yes, update the table below
-->

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Cualquier Workfront o flujo de trabajo con un paquete de Planning</p></li>
O
<li><p>Cualquier paquete de Planning cuando se adquiere como producto independiente</p></li></ul>
   </td>

<tr> 
   <td role="rowheader"><p>Productos adicionales</p></td> 
   <td><ul>
   <li><p>Adobe GenStudio for Performance Marketing</p></li>
   <!--
   <li><p>Adobe Customer Journey Analytics</p></li>
   -->
   </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workflow</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licencia de planificación de Adobe</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> 
   <ul>
   <li><p>Debe agregar un tipo de licencia de flujo de trabajo y de Planning al nivel de acceso cuando tenga un flujo de trabajo y un paquete de Planning a la vez</p>   </li>
   <li><p>La configuración Deshabilitar espacio de ideación en su nivel de acceso debe estar deseleccionada</p></li>
</td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td> <p>Permisos de contribución o superiores al espacio de trabajo y tipo de registro donde desee agregar registros </p>
      <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
      <p>Ver permisos de objetos de Workfront para agregarlos a informes <!--not sure if this is available--></p>
      <p>Permisos de editor en el espacio de ideación para crear informes</p>
   </td> 
  </tr>  
   <tr> 
   <td role="rowheader"><p>Funciones de usuario de Adobe GenStudio for Performance Marketing</p></td> 
   <td><p><ul><li>Cualquier función de usuario de GenStudio para acceder a campañas, productos y personas</li>
   <li>GenStudio System Manager para acceder a las activaciones <!--and Events--></li></ul>
   Para obtener más información, consulte <a href="https://experienceleague.adobe.com/en/docs/genstudio-for-performance-marketing/user-guide/intro/user-roles">Funciones de usuario y permisos</a>. 
   </p>
  </td> 
  </tr> 
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++  

## Consideraciones sobre el uso del espacio de ideación para crear registros

* Solo puede iniciar el espacio de ideación desde Workfront Planning, a medida que crea o edita registros. El espacio de ideación no existe fuera de Workfront Planning.
* Para acceder al espacio de ideación, debe tener un espacio de trabajo y un tipo de registro en Workfront Planning.
* Los registros nuevos siempre comienzan con contenido de marcador de posición, independientemente de cómo los cree.
* Cuando se elimina un registro de Planning vinculado a un informe de ideación, el informe permanece en el espacio de ideación y su lienzo asociado en el espacio de ideación no se elimina.
* La sincronización de información solo se produce desde el Espacio de ideación a Workfront Planning. No hay sincronización inversa o automática de un registro de Planning al informe de espacio de ideación.
* Cuando se crean, editan o eliminan campos en Workfront Planning, se dan los siguientes escenarios:

  * Los nuevos campos creados en los registros vinculados a los informes de ideación se añaden diariamente a la información. Los nuevos campos aparecen vacíos en el resumen de ideación.
  * Los campos eliminados permanecen en la descripción y conservan sus valores anteriores.
  * Los campos con nombres cambiados actualizan sus nombres en la descripción.
* Puede agregar documentos como tarjetas en el espacio de ideación. Esto también incluye imágenes.

  Se admiten los siguientes tipos de archivo: PDF, Excel, CSV, PNG (y otros formatos de imagen), Word y PowerPoint. No se admiten vídeos.

  Todos los documentos cargados se convierten a PDF en el servidor para su procesamiento.
* Puede arrastrar y soltar registros directamente desde Workfront Planning en el espacio y aparecerán del mismo modo que los archivos cargados manualmente.

## Creación de registros con el espacio de ideación

1. En la página de aterrizaje de Workfront Planning, haga clic en la tarjeta de un espacio de trabajo que pueda administrar.
1. Haga clic en la tarjeta de un tipo de registro al que pueda agregar registros.
1. Realice una de las siguientes acciones para crear un registro:

   * Desde cualquier vista de la página de tipo de registro, haz clic en **Nuevo registro** en la esquina superior derecha de la página y en el cuadro **Elige una forma de agregar tus registros**, haz clic en **Abrir el espacio de ideación** y, a continuación, haz clic en **Continuar**.
   * Desplácese hasta la parte inferior de la tabla de registro y haga clic en **Nueva fila**; a continuación, haga clic en **Abrir el espacio de ideación**.

     >[!TIP]
     >
     >Si se selecciona **No mostrar**, se descartará permanentemente la solicitud futura. Al hacer clic en el icono Cerrar **X**, se cerrará este cuadro, pero volverá a aparecer la próxima vez que agregue un registro en línea.

   ![Nuevo cuadro de registros con el botón Abrir espacio de ideación](assets/new-record-creation-picker-with-ideation.png)

   El espacio de ideación se abre en una nueva pestaña con un mensaje vacío.

   El registro se crea inmediatamente con texto de marcador de posición.

1. (Opcional) Haga clic en **Usar informe existente** en el cuadro de mensaje para examinar y agregar un documento existente que el espacio de ideación utilizará para crear el informe y el registro futuro.

   ![Mensaje de información de ideación vacío](assets/empty-ideation-prompt.png)

1. (Opcional) Haga clic en el icono **Abrir lienzos anteriores** <!--accurate??--> ![Abrir el icono de los informes existentes](assets/open-existing-briefs-icon.png) en la esquina superior derecha del cuadro de mensaje para abrir los informes existentes

1. En **¿En qué está trabajando?** , describa el tipo de registro que desea crear.

   Cuantos más detalles comparta, más útil será la información proporcionada por el espacio de ideación. Por ejemplo, escriba una descripción de la campaña que está planeando: &quot;campaña de vuelta al colegio para una agencia de marketing&quot;.

1. Haga clic en **Comenzar a idear**.

   El espacio de ideación funciona siguiendo los pasos siguientes mientras crea su idea: <!--check some of these in the UI - there might have been UI text changes-->

   1. Comprenda su objetivo y contexto
   2. Revisar el espacio y los materiales seleccionados
   3. Recopilar pruebas de documentos, sitios web y datos
   4. Sintetizar los resultados en un resumen de investigación
   5. Crear y refinar tarjetas con citas

   Durante este proceso, verá el espacio de ideación buscando activamente los datos de Workfront Planning conectados o la información disponible en la web.

   Por ejemplo, podría buscar programas, productos, personalidades o regiones existentes, así como conceptos similares disponibles en línea. <!--check on this with Et-->

   Cuando la ideación termina, se añaden las siguientes cosas al espacio de ideación:

   * Un resumen de los hallazgos de IA que está vinculado a varias tarjetas con información detallada sobre los aspectos a considerar. Las tarjetas de detalles se muestran en una nueva sección. Un conector indica qué sección de la tarjeta pertenece a qué resumen.

   * Un archivo **Brief** en la esquina inferior izquierda del espacio de ideación. El informe es un borrador del registro futuro y se muestra como la página Detalles de un registro.

   ![Tarjeta de ideas con ramas](assets/ideation-card-with-branched-off-additional-cards.png)

1. Continúe añadiendo información al espacio de ideación para completar la creación de la descripción.

1. (Condicional) Cuando finalice el informe, haga clic en la imagen de vista previa en la esquina inferior izquierda y, a continuación, haga clic en una de las siguientes opciones:

   * **Exportar a archivo** para crear un archivo
   * **Exportar a Workfront Planning** para crear un registro de Planning

   Para obtener información acerca de cómo agregar elementos al informe y exportarlo, vea [Crear informes en el espacio de ideación](/help/quicksilver/planning/ideation/create-briefs-in-ideation-space.md).

   De este modo, se termina de crear el registro con la información adicional y se agrega al tipo de registro seleccionado originalmente.

## Editar registros existentes en Espacio de ideas

Puede abrir el espacio de ideación desde registros existentes para actualizarlos.

No se pueden editar registros en lote en el espacio de ideación.

1. Vaya a un registro existente en Workfront Planning y abra su página de detalles.

1. Haga clic en **Abrir en el espacio de ideación**. Esto abre el espacio de ideación en una nueva pestaña.

   Si ya existe una ideación para el registro, se abre ese espacio.

   Si no existe ninguna ideación, crea un espacio de ideación y un informe.

   >[!TIP]
   >
   >La edición masiva de registros con el espacio de ideación no está disponible.

   <!-- 
    I don't think these steps are still valid but the environment was not available to test: 
    - If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
    - If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.
    -->

1. Continúe editando el informe como se describe en la sección [Crear registros usando el espacio de ideación](#create-records-using-the-ideation-space) de este artículo.






<!-- this is from Claude, but rephrased and included most of this above: 

## Step 5: Open the Workfront Planning Records panel

To bring real Workfront Planning records into your canvas (rather than just AI-generated ideas), click the **records icon** in the left-hand toolbar (third icon down). This opens the **Workfront Planning Records** panel, listing all **Connected Record types** available in your Planning environment — for example:

- Products
- Regions
- Personas
- Channels
- Activations
- Project
- Test Record
- Experience Manager Assets

## Step 6: Drag real records onto the canvas

Search or browse within a record type (e.g., **Products** or **Personas**), then drag the record you want directly onto the canvas. In the example, an existing **Nike product** record and a **Deep testing** persona record were both dragged in and positioned near the relevant concept cards.

This lets you visually connect your AI-generated ideas to the actual records that already exist in Workfront Planning, grounding the ideation in real data rather than hypothetical entities.


![Dragging a persona record onto the canvas](images/05_drag_persona_record.png)

---

## Step 7: Refine with follow-up prompts

Use the **Ask anything** box in the bottom-right corner at any time to refine the canvas — for example, typing `regenerate` against a specific card to have Catalyze redo that section using updated context. Catalyze will re-run its reasoning steps (searching, synthesizing, citing) and update the affected cards in place.

---

## Step 8: Review the full canvas

Zoom out to see the complete picture: your original campaign goal, all AI-generated concept cards with citations, the real Workfront Planning records you've pulled in (Products, Personas, etc.), and a **Campaign Brief** summary card in the corner pulling it all together.



![Full canvas overview](images/06_full_canvas_overview.png)

---

## Tips

- **Be specific in Step 2** — richer campaign descriptions produce more relevant, better-grounded cards.
- **Check citations** before trusting a generated fact — click **Sources** on any card.
- **Mix AI cards with real records** — dragging in actual Products, Personas, Regions, etc. keeps the canvas tied to your real Planning data, not just AI speculation.
- Responses are AI-generated and may be inaccurate — always verify against the linked sources before finalizing a record.

***************SECOND DRAFT FROM CLAUDE*******************
# Creating and Managing Records with Catalyze Ideation

> This workflow reflects the Closed Beta experience and is expected to evolve before Open Beta and GA. Confirm current behavior before publishing to customers.

This guide explains how to create and ideate on records using Catalyze within Workfront Planning. It covers all entry points, system behavior, data sync rules, and file-upload support.

## Before you start

- You must have access to a record list within Workfront Planning.
- Catalyze always opens in a **new browser tab** — this is consistent across every entry point.
- Any record created through Catalyze starts with **placeholder text** until you begin ideating.

## Option 1: Create a record via the top-level "New Record" button

1. Navigate to your record list in Workfront Planning.
2. Click the **New Record** button at the top of the page.
3. From the dropdown menu, select **Ideate in Catalyze**.
4. A new browser tab opens automatically, launching the Catalyze canvas.
5. A new record is created in Workfront Planning with placeholder text.
6. Begin ideation directly in Catalyze.

**Additional access from the record view:** Open the newly created record and, in its detail modal, click **Ideate in Catalyze**. This opens Catalyze in a new tab (same behavior as above).

## Option 2: Create a record via inline record creation (bottom of table)

1. Scroll to the bottom of the record table.
2. Click **New Record**.
3. The record is created immediately with placeholder text.
4. A pop-up appears with these options:
   - **Open Catalyze** — launches Catalyze in a new browser tab
   - **Don't Show Again** — permanently dismisses the future prompt
   - **X (Close)** — closes the pop-up; it will reappear next time
5. Click **Open Catalyze** to begin ideation.

## Working with existing records

**Contextual actions (bottom selection bar)**
- **Single record selected:** an "Ideate in Canvas" / "Open in Canvas" action appears.
  - If a canvas already exists, it opens that canvas.
  - If no canvas exists, it creates a new one.
- **Multiple records selected:** the Ideate/Open in Canvas action is **not available** — bulk ideation is not supported.

**Record detail panel**
- If no canvas is connected, an **Ideate in Catalyze** button appears in the record header.
- If a record is already linked to a Catalyze canvas, a link appears beneath the record title; clicking it opens the associated canvas.
- If a linked canvas hasn't been exported/pushed back yet, the record shows a placeholder message ("This record has active Canvas...") even if the canvas itself has a real name in Catalyze.

**When can you create a canvas for a record?**
A canvas can be created for a record that is in Workfront Planning and still in **draft** state (not yet marked "ready").

## Record deletion behavior

If a Planning record linked to a Catalyze canvas is deleted:
- The canvas remains intact in Catalyze.
- No data is removed from Catalyze.

## Data synchronization rules

**Sync direction:** One-way only, from Catalyze → Workfront Planning. There is no reverse or automatic sync from Planning back to Catalyze.

**Export process:**
1. In Catalyze, click **Export to Planning**.
2. Data is pushed to the connected Workfront Planning record.
3. The export **overwrites all existing field data** in the record.

**Important notes:**
- Changes made directly in Workfront Planning do **not** sync back to Catalyze.
- Data refresh in Workfront Planning is manual only (Beta behavior) — there is no scheduled/automatic sync.
- Schema updates do sync one direction: once connected, Planning schema changes propagate to Catalyze daily — added fields appear empty, removed fields keep their prior values, and renamed fields update in place.

## Uploading documents into the Catalyze canvas

- Files can be added as a "document card" on the canvas — this works the same whether the file is an image or another document type.
- You can drag and drop files directly from Workfront Planning onto the canvas, and they appear the same way as manually uploaded files.
- All uploaded documents are converted to PDF on the backend for processing.
- Supported file types (as of the Aug 2026 beta): **PDF, Excel, CSV, PNG (and likely other image formats), Word, PowerPoint.**
- **Not supported:** video files.
- You can include images directly in a prompt and Catalyze will recognize their content, though small-format legibility is still being refined.

## Key takeaways

- Use **Ideate in Catalyze** to connect records to the AI-assisted ideation workflow.
- Catalyze always launches in a separate browser tab.
- New records always start with placeholder content, regardless of entry point.
- Data flow between Catalyze and Planning is manual and one-directional (Catalyze → Planning).
- Deleting a Planning record does not delete its associated Catalyze canvas.

-->


<!--
Internal info: 

## The Ideation space and Adobe GenStudio

Adobe GenStudio for Performance Marketing is Adobe's end-to-end content supply chain solution, spanning five stages:

1. Strategy and Ideation
2. Workflow and Planning
3. Asset Management
4. Creation and Production
5. Delivery and Activation

The Ideation space fits in the **Strategy and Ideation** stage — the front door of the content supply chain — and is designed to work natively with the rest of GenStudio, so the briefs and strategic direction it generates flow directly into Workfront Planning for execution.
-->


