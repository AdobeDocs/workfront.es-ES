---
user-type: administrator
product-area: system-administration;setup
title: Importación de tarjetas de tasa desde una plantilla
description: Puede utilizar un archivo de plantilla para crear las tarjetas de tarifa en Excel e importarlas en Adobe Workfront.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: debe90e7-08c2-4385-96fb-8d349dec6741
source-git-commit: aa774419e65e9e4a5785382d3cb2b22bdb0389c9
workflow-type: tm+mt
source-wordcount: '1812'
ht-degree: 3%

---

# Importar tarjetas de tarifas desde una plantilla

Puede utilizar un archivo de plantilla para crear las tarjetas de tarifas en Excel e importarlas en Adobe Workfront, en lugar de agregar todos los roles y tarifas manualmente.

Para ver las tarjetas de tasa de ejemplo descritas en este artículo, descargue el [archivo de muestra](assets/rate-cards-sample.zip).

Para obtener más información sobre las tarjetas de tarifas, consulte [Administrar tarjetas de tarifas](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md).

## Reglas importantes para trabajar con el archivo de plantilla

* Introduzca el rol o la categoría de recurso no laboral, pero no ambos.
* La secuencia de tarjetas de tasa de la ficha RATE_RTCRD debe coincidir con el orden de las tarjetas de la ficha RTCRD (1 para la primera, 2 para la segunda, etc.).
* La fecha de inicio y la fecha de finalización deben seguir los formatos permitidos.
* Las tarjetas de tarifas se pueden importar sin tarifas y actualizar más tarde.
* Atributos personalizados (Agencia, Centro de coste, etc.) puede variar. Consulte con el administrador del sistema los requisitos exactos.
* Las filas eliminadas en la plantilla no eliminarán los registros existentes en el sistema.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Standard]</td> 
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Editar acceso a [!UICONTROL Rate Cards]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Rellene el archivo de plantilla

{{step-1-to-setup}}

1. El panel de navegación izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifas**].
1. Haga clic en **Nueva tarjeta de tarifa** y luego haga clic en **Descargar plantilla de Excel**.
1. Siga las indicaciones del explorador para guardar el archivo de plantilla en el equipo.
1. Abra el archivo de plantilla en Excel.

   >[!TIP]
   >
   > Guarde el archivo con un nombre nuevo si desea mantener el archivo de plantilla vacío y utilizarlo de nuevo más tarde.

   La plantilla tiene dos pestañas. Ambas pestañas deben tener la información correcta para importar correctamente las tarjetas de tasa.

   * RTCRD: Definir las tarjetas de tasas (información básica)
   * RATE_RTCRD: Definir las tasas detalladas asociadas con cada tarjeta de tasas

### Fill out the RTCRD (Rate Card Setup) tab

Create and list all of rate cards on this tab. Each row represents one rate card.

![RTCRD tab on rate card import template file](assets/rate-card-import-template-tab1.png)

1. Enter the information for a rate card on each row:

   * **Name** (required): The name of the rate card, such as &quot;Global Billing 2025.&quot;

     This name is the main identifier for the rate card. Each rate card must have a unique name.

   * **Description** (optional): A free-form text description of the rate card. Use this to describe purpose, scope, or validity, for example, &quot;Applies to North American projects.&quot;
   * **Company** (optional): This can be either the company name or the company ID. The import will recognize both.

     Example: Coffesta, or _68c0234e00000541dd8c0757723daa68_

   * **Group** (optional): This can be either the group name or the group ID. The import will recognize both.

     Example: Marketing, or _68c0234e00000541dd8c0757723daa68_

   * **Custom fields** (optional): You can add additional columns with custom field names if your environment has specific requirements.

   >[!NOTE]
   >
   >* At minimum, you must enter the Name for each rate card.
   >* Each rate card is automatically given a sequence number based on its row position. For example, the first rate card you define (in row 2) is sequence 1, the next is 2, and so on. These sequence numbers are used in the RATE_RTCRD tab to attach rates.

### Fill out the RATE_RTCRD (Rates Setup) tab

Define all the rates that belong to the rate cards on this tab.

Every row on the tab defines one specific rate. You can create multiple rates under the same rate card by repeating the rate card sequence.

Asegúrese de que las fechas no se superponen a menos que sea el propósito.

![Ficha RATE_RTCRD en el archivo de plantilla de importación de tarjeta de tarifas](assets/rate-card-import-template-tab2.png)

1. Introduzca la información de una tasa en cada fila:

   * **Nombre** (obligatorio): Una etiqueta para la fila de tarifa.

     La práctica recomendada es reutilizar el nombre de la tarjeta de tarifa para una mayor claridad, como &quot;Facturación global 2025: tarifa de desarrollador&quot;.

   * **Referencia de tarjeta de tarifa** (obligatorio): El número de secuencia de la tarjeta de tarifa a la que pertenece esta tarifa.

     Si la tarjeta de tarifa fue la primera que enumeró en la ficha RTCRD (fila 2), escriba 1. Si era el segundo, escriba 2, y así sucesivamente.

   * **Rol** (necesario si no se usa la categoría de recursos no laborales): El rol al que se aplica la tarifa. Puede ser el nombre de la función o el ID de la función. La importación reconocerá ambos.

     Ejemplo: Designer o _68c0234e00000541dd8c0757723daa68_

   * **Categoría de recurso no laboral** (obligatorio si no se usa el rol): La categoría de recurso no laboral a la que se aplica la tasa. Puede ser el nombre o el ID de la categoría. La importación reconocerá ambos.

     Ejemplo: cámara o _68c0234e00000541dd8c0757723daa68_

     >[!IMPORTANT]
     >
     >No puede escribir datos en las columnas **Rol** y **Categoría de recursos no laborales**. Se requiere una.

   * **Fecha de inicio** (opcional): La fecha en que la tarifa entra en vigencia.

     La fecha debe seguir uno de los formatos admitidos (según su ubicación): dd/MM/aaaa, dd/MM/aaaa, DD/MM/AAAA, DD/MM/AAAA, dd/MM/aa, dd/MM/aa, dd/MM/yyyy, dd/MM/yyyy, yyyy-MM-dd, yyyy-dd-MM

     Ejemplo: 01/01/2025

     Para obtener más información, consulte [Requisitos de formato de fecha](#date-formatting-requirements), más adelante.

   * **Fecha de finalización** (opcional): La fecha en que la tarifa deja de ser efectiva.

     Esta fecha debe seguir los mismos formatos admitidos que la fecha de inicio.

     Para obtener más información, consulte [Requisitos de formato de fecha](#date-formatting-requirements), más adelante.

   * **Value** (optional): The numeric rate value, for example 150. El valor predeterminado es 0.
   * **Currency** (optional): The currency for the rate, for example USD, EUR, GBP. The default is the system currency.
   * **Locked** (optional): Indicates if the rate is locked. Valid values are True or False.
   * **Attributes** (optional / custom): The last columns (Agency, Location, Cost Center, etc.) are Rate Attributes that differ by customer configuration. These are customizable fields and may vary per customer environment.

     Example: Agency = &quot;1: Agency,&quot; Location = &quot;Chicago,&quot; Cost Center = &quot;22: Cost Center&quot;

### Fill out the RSALS (Rate Card Alias) tab

Create and list all of the aliases on this tab. Each row represents one alias.

When the rate card is attached to a project, the alias appears on information such as placeholder assignments, expenses, and reports, instead of the internal job role name. Only one alias can exist for each job role and attribute combination within a single rate card.

An alias is added to the system, but it is not connected to a job role based on the information on this tab.

![RSALS tab on rate card import template file](assets/rsals-tab-rate-card-import.png)

1. Enter the name of an alias on each row.

   Only enter one alias name per row: a job role alias, a non-labor resource category alias, or an expense type alias.

### Fill out the RCRMET_RTCRD_RSALS (Rate Card Metadata) tab

On this tab you can define the connections between resources and aliases for a specific rate card.

![RCRMET_RTCRD_RSALS tab on rate card import template file](assets/rcrmet-tab-rate-card-import.png)

1. Enter the information on each row:

   * **Rate Card** (required): The name or the sequence number of the rate card that the resource and alias belong to. The rate card must be listed on the RTCRD tab.

     For a sequence number: If the rate card was the first one you listed on the RTCRD tab (row 2), enter 1. Si era el segundo, escriba 2, y así sucesivamente.

   * **Rol** (necesario si no se usan el tipo de gasto y la categoría de recursos no laborales): El rol al que está conectado el alias. Puede ser el nombre de la función o el ID de la función. La importación reconocerá ambos.

     Ejemplo: Designer o _68c0234e00000541dd8c0757723daa68_

   * **Tipo de gasto** (necesario si no se usan el Rol de trabajo y la Categoría de recursos no laborales): El tipo de gasto al que está conectado el alias. Puede ser el nombre del tipo de gasto o el ID del tipo de gasto. La importación reconocerá ambos.

     Ejemplo: Viaje o _68c0234e00000541dd8c0757723daa68_

   * **Categoría de recurso no laboral** (necesario si no se usan el rol y el tipo de gasto): La categoría de recurso no laboral a la que está conectado el alias. Puede ser el nombre o el ID de la categoría. La importación reconocerá ambos.

     Ejemplo: cámara o _68c0234e00000541dd8c0757723daa68_

     >[!IMPORTANT]
     >
     >No puede ingresar las tres columnas **Rol**, **Tipo de gasto** y **Categoría de recursos no laborales**. Se requiere una.

   * **Alias de recurso**: El alias introducido en la ficha RSALS.

### Requisitos de formato de fecha

Al preparar los datos de la tarjeta de tarifas para la importación, debe asegurarse de que las columnas de fecha tengan el formato **General**, no **Fecha**.

Si las columnas están configuradas en Formato de fecha, el sistema puede malinterpretar los valores durante el proceso de importación, lo que provoca errores o errores en las cargas. El uso del formato General conserva la representación numérica o textual sin procesar de la fecha, lo que permite al sistema validar y aplicar correctamente los valores.

Seguir estos pasos evitará problemas innecesarios y garantizará una importación fluida y precisa de los datos de tarifas.

1. Antes de guardar o cargar el archivo, seleccione las columnas de fecha en la hoja de cálculo.
1. Cambie el formato de columna a **General**.
1. Compruebe que los valores siguen mostrándose correctamente (por ejemplo, 01/01/2025 o 2025-01-01).

## Importar el archivo de plantilla

{{step-1-to-setup}}

1. El panel de navegación izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifas**].
1. Click **New rate card**, then click **Import new rate cards**.
1. Drag and drop your file into the dialog, or click **Select an Excel file** to browse to the file on your computer.
1. Click **Start importing**.

   If there are no issues with the file, then a confirmation message appears and the new rate cards appear in the list.

1. If the file contains issues, an error message appears. Click **See issues** to view the issues on a separate screen.

   You must correct the issues in the Excel file and import it again before the rate cards will exist in Workfront.

## Update existing rate cards

You can update the rates in your existing rate cards using the same Excel template and upload those changes to Workfront.

Only the RATE_RTCRD (Rates Setup) tab is required for updating existing rates.

>[!NOTE]
>
>Uploading rates for an existing rate card overwrites all of the current job roles and rates on the rate card.
>
>For example, if you have 5 job roles with rates on the existing rate card and the Excel file has 1 job role, then the rate card will have 1 job role after you upload. To keep the other 5 job roles and their rates on the rate card, you must include them in the Excel file.

To update existing rate cards:

{{step-1-to-setup}}

1. El panel de navegación izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifas**].
1. Click **New rate card**, then click **Import rate card updates**.
1. Drag and drop your file into the dialog, or click **Select an Excel file** to browse to the file on your computer.
1. Click **Start importing**.

   If there are no issues with the file, then a confirmation message appears and the new rate cards appear in the list.

1. If the file contains issues, an error message appears. Click **See issues** to view the issues on a separate screen.

   You must correct the issues in the Excel file and import it again before the rate card updates will exist in Workfront.


