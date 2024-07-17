---
title: Módulos CloudConvert
description: Módulos CloudConvert
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: e21ef8a0-bec0-43fc-a495-c00b4023a273
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '3008'
ht-degree: 0%

---

# [!DNL CloudConvert] módulos

En un escenario de Adobe Workfront Fusion, puede automatizar los flujos de trabajo que utilizan CloudConvert, así como conectarlo a varias aplicaciones y servicios de terceros. Los módulos [!DNL CloudConvert] le permiten supervisar y administrar trabajos, tareas e importar y exportar archivos en su cuenta de [!DNL CloudConvert].

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] o superior</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Trabajo]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licencia**</td> 
   <td>
   <p>Requisito de licencia actual: no se requiere licencia de [!DNL Workfront Fusion].</p>
   <p>O</p>
   <p>Requisito de licencia heredado: [!UICONTROL [!DNL Workfront Fusion] para automatización e integración de trabajo] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Product</td> 
   <td>
   <p>Requisito de producto actual: si tiene el plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Adobe Workfront], su organización debe adquirir [!DNL Adobe Workfront Fusion] así como [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo. [!DNL Workfront Fusion] está incluido en el plan [!DNL Workfront] de [!UICONTROL Ultimate].</p>
   <p>O</p>
   <p>Requisito de productos heredados: su organización debe comprar [!DNL Adobe Workfront Fusion] y [!DNL Adobe Workfront] para utilizar la funcionalidad descrita en este artículo.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

## Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion] {#connect-cloudconvert-to-workfront-fusion}

Para conectar tu cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], debes obtener la clave de API de tu cuenta de [!DNL CloudConvert].

1. Inicie sesión en su cuenta de [!DNL CloudConvert] y abra su [!UICONTROL panel].
1. Abra la sección **[!UICONTROL Autorización] > [!UICONTROL Claves de API]**.
1. Haga clic en **[!UICONTROL Crear nueva clave de API]**.
1. Escriba el nombre de la clave de API, habilite los ámbitos que desee usar y, a continuación, haga clic en **[!UICONTROL Crear]**.
1. Copie el token proporcionado y guárdelo en un lugar seguro.
1. En [!DNL Workfront Fusion], empiece a crear un escenario y abra el cuadro de diálogo **[!UICONTROL Crear una conexión]** del módulo [!DNL CloudConvert].

   Para obtener instrucciones, vea [Crear un escenario en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Escriba el token que guardó en el paso 5 y luego haga clic en **[!UICONTROL Continuar]** para establecer la conexión.

## [!DNL CloudConvert] módulos y sus campos {#cloudconvert-modules-and-their-fields}

Al configurar [!DNL CloudConvert] módulos, [!DNL Workfront Fusion] muestra los campos que se indican a continuación. Junto con estos, podrían mostrarse [!DNL CloudConvert] campos adicionales, según factores como el nivel de acceso en la aplicación o el servicio. Un título en negrita en un módulo indica un campo obligatorio.

Si ve el botón Asignar encima de un campo o función, puede utilizarlo para establecer variables y funciones para ese campo. Para obtener más información, vea [Asignar información de un módulo a otro en [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Tareas comunes](#common-tasks)
* [Trabajos](#jobs)
* [Tareas](#tasks)
* [Otro](#other)

### Tareas comunes

* [Capturar un sitio web](#capture-a-website)
* [[!UICONTROL Convertir un archivo]](#convert-a-file)
* [Crear un archivo](#create-an-archive)
* [Combinar archivos](#merge-files)
* [Optimización de un archivo](#optimize-a-file)

#### [!UICONTROL Capturar un sitio web]

Este módulo de acción captura un sitio web especificado y lo guarda en formato PDF, JPG de la o PNG.

Usted especifica la dirección URL del sitio web y otra información, como dónde desea almacenar la información.

El módulo devuelve el ID del archivo y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Introduzca la dirección URL del sitio web que desea capturar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de salida] </td> 
   <td>Seleccione si desea guardar el sitio web capturado en formato PNG, JPG o PDF. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de archivo] </td> 
   <td>Introduzca un nombre de archivo (incluida la extensión) para el archivo de salida de destino.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados] </td> 
   <td> <p>(Opcional) Defina encabezados de solicitud. </p> <p>Esto resulta útil, por ejemplo, cuando la dirección URL especificada requiere autorización. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Conversión y opciones específicas del motor] </p> </td> 
   <td>Especifique las opciones específicas del motor y la conversión. Para ver las opciones disponibles, consulte la documentación de la API <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] </a> para <code>input_format</code> y <code>output_format</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descargar un archivo] </td> 
   <td> <p>Active esta opción si también desea incluir datos de archivo en la salida del módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Convertir un archivo]

Convierte un archivo en un formato de salida seleccionado.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de entrada]</td> 
   <td>Seleccione si desea cargar un archivo mediante [!DNL Workfront Fusion] o proporcione la dirección URL desde la cual se cargará el archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cargar un archivo]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importar un archivo desde URL]</td> 
   <td> 
    <ul> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>Introduzca la dirección URL del archivo que desea convertir.</p> </li> 
     <li> <p><strong>[!UICONTROL Encabezados]</strong></p> <p>Defina los encabezados de solicitud (opcional). Esto resulta útil, por ejemplo, cuando la dirección URL especificada requiere la autorización.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato]</td> 
   <td>Seleccione si desea especificar el formato de entrada del archivo que desea convertir. Si no se especifica, se utiliza la extensión del archivo de entrada como formato de entrada.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Input Format]</td> 
   <td>Seleccione el formato actual del archivo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Formato de salida]</td> 
   <td>Seleccione el formato de archivo de destino al que desea convertir el archivo.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Nombre de archivo]</td> 
   <td>Elija un nombre de archivo (incluida la extensión) para el archivo de salida de destino.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>[!UICONTROL Conversión y opciones específicas del motor] </p> </td> 
   <td>Especifique las opciones específicas del motor y la conversión. Para ver las opciones disponibles, consulte la documentación de la API <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] </a> para <code>input_format</code> y <code>output_format</code>.</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL Descargar un archivo] </td> 
   <td> <p>Active esta opción si también desea incluir datos de archivo en la salida del módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Crear un archivo]

Permite añadir uno o varios archivos al archivo ZIP, RAR, 7Z, TAR, TAR.GZ o TAR.BZ2.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Archivos de entrada]</p> </td> 
   <td> <p>Especifique los archivos que desea agregar al archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cargar un archivo]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Importar un archivo desde URL]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>Introduzca la dirección URL del archivo que desea archivar.</p> <p><strong>[!UICONTROL Encabezados]</strong> </p> <p>Defina los encabezados de solicitud (opcional). Esto resulta útil, por ejemplo, cuando la dirección URL especificada requiere la autorización.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de salida]</td> 
   <td> <p> Seleccione el formato de destino del archivo archivado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de archivo]</td> 
   <td> <p> Introduzca el nombre del archivo (incluida la extensión) para el archivo de salida de destino.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conversión y opciones específicas del motor] </td> 
   <td> <p>Especifique las opciones específicas del motor y la conversión. Para ver las opciones disponibles, consulte la documentación de la API <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] </a> para <code>input_format</code> y <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descargar un archivo]</td> 
   <td> <p>Active esta opción si también desea incluir datos de archivo en la salida del módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Combinar archivos]

Combina al menos dos archivos en un PDF. Si los archivos de entrada no son PDF, se convierten automáticamente en PDF.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Archivos de entrada]</p> </td> 
   <td> <p>Especifique los archivos que desea combinar.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cargar un archivo]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Importar un archivo desde URL]</p> </td> 
   <td> <p><strong>[!UICONTROL URL]</strong> </p> <p>Introduzca la dirección URL del archivo que desea archivar.</p> <p><strong>[!UICONTROL Encabezados]</strong> </p> <p>Defina los encabezados de solicitud (opcional). Esto resulta útil, por ejemplo, cuando la dirección URL especificada requiere la autorización.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de salida]</td> 
   <td> <p> Seleccione el formato de destino del archivo combinado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de archivo]</td> 
   <td> <p> Introduzca el nombre del archivo (incluida la extensión) para el archivo de salida de destino.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conversión y opciones específicas del motor] </td> 
   <td> <p>Especifique las opciones específicas del motor y la conversión. Para ver las opciones disponibles, consulte la documentación de la API <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] </a> para <code>input_format</code> y <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descargar un archivo]</td> 
   <td> <p>Active esta opción si también desea incluir datos de archivo en la salida del módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Optimizar un archivo]

Este módulo de acción optimiza y comprime un archivo en formato PDF, PNG o formato de JPG.

Especifique el archivo y los parámetros para optimizarlo y almacenarlo.

El módulo devuelve el ID del archivo y cualquier campo asociado, junto con cualquier campo personalizado y valor al que acceda la conexión. Puede asignar esta información en módulos subsiguientes en el escenario.

Al configurar este módulo, se muestran los campos siguientes.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivo de entrada]</td> 
   <td>Seleccione si desea cargar un archivo mediante Workfront Fusion o proporcione la dirección URL desde la que se cargará el archivo.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Cargar un archivo]</p> </td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Importar un archivo desde URL] </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong>: escriba la dirección URL del archivo que desea convertir.</li> 
     <li><strong>[!UICONTROL Encabezados]</strong>: (Opcional) Defina encabezados de solicitud. Esto resulta útil, por ejemplo, cuando la dirección URL especificada requiere autorización.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Optimization for] </td> 
   <td> <p>Seleccione el perfil de optimización para las necesidades específicas del público objetivo.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Web]</strong>: optimización para la web (predeterminado)</p> 
      <ul> 
       <li>Eliminación de datos redundantes e innecesarios para la web</li> 
       <li>Reducir resolución, recortar y comprimir imágenes de forma inteligente</li> 
       <li>Fuentes de combinación y subconjunto</li> 
       <li>Convertir colores en RGB</li> 
      </ul> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Imprimir]</strong>: Optimización para impresión</p> 
      <ul> 
       <li> <p>Eliminar datos redundantes e innecesarios para imprimir</p> </li> 
       <li> <p>Reducir resolución, recortar y comprimir imágenes de forma inteligente</p> </li> 
       <li> <p>Fuentes de combinación y subconjunto</p> </li> 
       <li> <p>Convertir colores a CMYK</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Archivo]</strong>: Optimización para fines de archivo</p> 
      <ul> 
       <li> <p>Eliminación de datos redundantes e innecesarios para el archivado</p> </li> 
       <li> <p>Comprimir imágenes de forma inteligente</p> </li> 
       <li> <p>Fuentes de combinación y subconjunto</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Imágenes digitalizadas]</strong>: Optimización para imágenes digitalizadas</p> 
      <ul> 
       <li> <p>Perfil optimizado para PDF que principalmente constan de imágenes rasterizadas</p> </li> 
       <li> <p>Comprimir las imágenes sin reducir significativamente la calidad visual</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL reducción de tamaño máximo]</strong>: optimización para reducción de tamaño máximo</p> 
      <ul> 
       <li> <p>Utilice la máxima compresión posible</p> </li> 
       <li> <p>Podría reducir la calidad visual</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de entrada] </td> 
   <td>Seleccione el formato del archivo de entrada que desea optimizar. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de archivo]</td> 
   <td> <p>Introduzca un nombre de archivo (incluida la extensión) para el archivo de salida de destino.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conversión y opciones específicas del motor]</td> 
   <td> <p>Especifique las opciones específicas del motor y la conversión. Para ver las opciones disponibles, consulte la documentación de la API <a href="https://cloudconvert.com/api/v2/convert#convert-tasks">[!DNL CloudConvert] </a> para <code>input_format</code> y <code>output_format</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Descargar un archivo]</td> 
   <td> <p>Active esta opción si también desea incluir datos de archivo en la salida del módulo.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Trabajos

* [[!UICONTROL Crear un trabajo (avanzado)]](#create-a-job-advanced)
* [[!UICONTROL Nuevo evento de trabajo]](#new-job-event)
* [[!UICONTROL Trabajos de lista]](#list-jobs)
* [[!UICONTROL Obtener un trabajo]](#get-a-job)
* [[!UICONTROL Eliminar un trabajo]](#delete-a-job)

#### [!UICONTROL Crear un trabajo (avanzado)]

Este módulo crea un trabajo. Un trabajo puede ser una o varias tareas identificadas en el campo [!UICONTROL Nombre] y vinculadas entre sí mediante el campo [!UICONTROL Entrada].

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archivos de entrada]</td> 
   <td> <p>Seleccione si desea cargar un archivo mediante [!DNL Workfront Fusion] o proporcione la dirección URL desde la cual se cargará el archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cargar un archivo]</td> 
   <td> <p>Seleccione un archivo de origen de un módulo anterior o asigne el nombre y los datos del archivo de origen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Importar un archivo desde URL]</p> </td> 
   <td> 
    <ul> 
     <li><strong>[!UICONTROL URL]</strong>: escriba la dirección URL del archivo que desea procesar.</li> 
     <li><strong>[!UICONTROL Encabezados]</strong>: (Opcional) Defina encabezados de solicitud. Esto resulta útil, por ejemplo, cuando la dirección URL especificada requiere autorización.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Tareas]</p> </td> 
   <td> <p>Agregar tareas que se realizarán dentro del trabajo.</p> <p>Consulte las descripciones de los campos de las operaciones en la sección correspondiente.</p> 
    <ul> 
     <li><a href="#convert-a-file" class="MCXref xref">[!UICONTROL Convertir un archivo]</a> </li> 
     <li><a href="#capture-a-website" class="MCXref xref">[!UICONTROL Capturar un sitio web]e</a> </li> 
     <li><a href="#optimize-a-file" class="MCXref xref">[!UICONTROL Optimizar un archivo]</a> </li> 
     <li><a href="#create-an-archive" class="MCXref xref">[!UICONTROL Crear un archivo]</a> </li> 
     <li><a href="#merge-files" class="MCXref xref">[!UICONTROL Archivos de combinación]</a> </li> 
    </ul> 
    <ul> 
     <li> <p><strong>[!UICONTROL Ejecutar un comando]</strong> </p> <p>Para obtener más información acerca de cómo ejecutar un comando, consulte la <a href="https://cloudconvert.com/api/v2/command#command-tasks">[!DNL CloudConvert] documentación de la API </a>.</p> </li> 
     <li> <p><strong>[!UICONTROL Exportar un archivo a la dirección URL temporal]</strong> </p> <p> Especifique el nombre de la tarea y el nombre de la tarea de entrada (por ejemplo, Conversión).</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Etiqueta] </td> 
   <td> <p>Introduzca una etiqueta. Las etiquetas son cadenas arbitrarias para identificar el trabajo. No tienen ningún efecto y se pueden utilizar para asociar el trabajo con un ID.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar un trabajo]

Este módulo elimina un trabajo, incluidas todas las tareas y datos.

>[!NOTE]
>
>Los trabajos se eliminan automáticamente 24 horas después de finalizar.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de trabajo]</td> 
   <td> <p>Introduzca o asigne el ID del trabajo que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener un trabajo]

Este módulo recupera los detalles del trabajo.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de trabajo]</td> 
   <td> <p>Introduzca o asigne el ID del trabajo sobre el que desea recuperar detalles.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Trabajos de lista]

Este módulo recupera todos los trabajos que se han ejecutado en su cuenta.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado] </td> 
   <td> <p>Seleccione el estado del trabajo para filtrar los trabajos devueltos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Establezca el número de trabajos que Workfront Fusion 2.0 devolverá durante un ciclo de ejecución.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Nuevo evento de trabajo]

Déclencheur cuando se crea, finaliza o falla un trabajo en su cuenta o tarea.

>[!NOTE]
>
>* El trabajo creado por el módulo [!UICONTROL Crear un trabajo (avanzado)] consta de *varias* tareas.
>* El déclencheur [!UICONTROL Nuevo evento de trabajo] también se activa cuando se crea, finaliza o falla una tarea *individual*.
>

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Nombre de webhook]</td> 
   <td>Introduzca el nombre del webhook. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Formato de salida] </td> 
   <td>Seleccione si desea guardar el sitio web capturado en formato PNG, JPG o PDF. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Evento]</td> 
   <td>Seleccione si el módulo se activa cuando se crea, finaliza o falla el trabajo o la tarea.</td> 
  </tr> 
 </tbody> 
</table>

>[!NOTE]
>
>* Si trabaja con el agregador de matrices (por ejemplo, tiene muchos archivos en diferentes formatos para convertir), use la opción **[!UICONTROL No conozco el formato de entrada]** en el cuadro de diálogo [!UICONTROL Agregar una tarea]. De lo contrario, se devuelve el error.
>* Vinculando tareas dentro del trabajo (nombre > entrada, nombre > entrada, etc.):
>
>  ![](assets/linking-name-across-jobs-350x808.png)>

### Tareas

* [[!UICONTROL Obtener una tarea]](#get-a-task)
* [[!UICONTROL Descargar un archivo]](#download-a-file)
* [[!UICONTROL Tareas de lista]](#list-tasks)
* [[!UICONTROL Reintentar una tarea]](#retry-a-task)
* [[!UICONTROL Cancelar una tarea]](#cancel-a-task)
* [[!UICONTROL Eliminar una tarea]](#delete-a-task)

#### [!UICONTROL Cancelar una tarea]

Este módulo cancela una tarea con un estado de espera o procesamiento.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de tarea]</td> 
   <td> <p> Introduzca o asigne el ID de la tarea que desea cancelar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Eliminar una tarea]

Eliminar una tarea, incluidos todos los datos.

>[!NOTE]
>
>Las tareas se eliminan automáticamente 24 horas después de finalizar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de tarea]</td> 
   <td> <p> Introduzca (asigne) el ID de la tarea que desea eliminar.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Descargar un archivo]

Este módulo recupera el nombre de archivo y los datos de archivo de la tarea especificada.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de tarea]</td> 
   <td> <p> Introduzca o asigne el ID de la tarea desde la que desea descargar el archivo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Obtener una tarea]

Este módulo recupera los detalles de la tarea.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de tarea]</td> 
   <td> <p>Introduzca o asigne el ID de la tarea sobre la que desea recuperar detalles.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Tareas de lista]

Este módulo recupera todas las tareas de la cuenta en función de la configuración del filtro.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Estado] </td> 
   <td> <p>Seleccione el estado de la tarea para filtrar las tareas devueltas por.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Id. de trabajo] </td> 
   <td> <p>Introduzca o asigne el ID de trabajo para devolver solo las tareas dentro del trabajo especificado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Operación] </td> 
   <td> <p>Introduzca el tipo de operación para devolver sólo las tareas con la operación especificada. </p> <p>Nota: Utilice el módulo [!UICONTROL List Possible Operations] para recuperar operaciones.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Límite] </td> 
   <td> <p>Introduzca o asigne el número máximo de registros que desea que devuelva el módulo durante cada ciclo de ejecución de escenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Reintentar una tarea]

Este módulo crea una nueva tarea en función de la configuración (carga útil) de otra tarea.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Identificador de tarea]</td> 
   <td> <p> Introduzca o asigne el ID de la tarea desde la que desea crear una nueva tarea.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Otro

* [[!UICONTROL Obtener mi información]](#get-my-info)
* [[!UICONTROL Realizar una llamada API]](#make-an-api-call)

#### [!UICONTROL Obtener mi información]

Recupera detalles de cuenta autenticada acerca del usuario actual.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones acerca de cómo conectar su cuenta de [!DNL CloudConvert] a [!DNL Workfront Fusion], vea <a href="#connect-cloudconvert-to-workfront-fusion" class="MCXref xref">Conectar [!DNL CloudConvert] a [!DNL Workfront Fusion]</a> en este artículo.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Realizar una llamada API]

Permite realizar una llamada de API personalizada.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Conexión]</td> 
   <td> <p>Para obtener instrucciones sobre cómo conectar su cuenta de [Fusion App] a Workfront Fusion, consulte <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Crear una conexión a Adobe Workfront Fusion: instrucciones básicas</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td> <p>Escriba una ruta relativa a <code>https://api.cloudconvert.com/</code>. Por ejemplo: <code>/v2/tasks</code></p> <p>Para obtener la lista de extremos disponibles, consulte la Documentación de la API <a href="https://cloudconvert.com/api/v2">[!DNL CloudConvert] v2</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Método]</td> 
   td&gt; <p>Seleccione el método de solicitud HTTP que necesita para configurar la llamada de API. Para obtener más información, vea <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Métodos de solicitud HTTP en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Encabezados]</td> 
   <td> <p>Añada los encabezados de la solicitud en forma de objeto JSON estándar.</p> <p>Por ejemplo, <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion 2.0 agrega los encabezados de autorización por usted.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cadena de consulta]</td> 
   <td> <p>Añada la consulta para la llamada de API en forma de objeto JSON estándar.</p> <p>Por ejemplo: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cuerpo]</td> 
   <td> <p>Agregue el contenido del cuerpo para la llamada de API en forma de objeto JSON estándar. Cuando utilice afirmaciones condicionales como <code>if</code> en su JSON, ponga las comillas fuera de la afirmación condicional.<img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"></p> </td> 
  </tr> 
 </tbody> 
</table>

**Ejemplo:** tareas de lista

La siguiente llamada de API devuelve todas las tareas de su cuenta de CloudFront:

URL: `/v2/tasks`

Método: `GET`

![](assets/cloudconvert-api-example-input.png)

Las coincidencias de la búsqueda se encuentran en la salida del módulo en [!UICONTROL Paquete] > [!UICONTROL Cuerpo] > [!UICONTROL datos].

En nuestro ejemplo, se devolvieron 6 tareas:

![](assets/cloudconvert-api-example-output.png)

## Resolución de problemas {#troubleshooting}

Consulte la siguiente tabla para ver los posibles errores y sus soluciones:

<table style="table-layout:auto">
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p>Error</p> </th> 
   <th>Pasos siguientes</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL El tamaño del archivo de salida supera el límite permitido para su escenario.]</span> </p> </td> 
   <td> <p>Consulte los límites de tamaño de archivo.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL Ha superado el tiempo máximo de conversión.]</span> </p> </td> 
   <td> <p>El plan [!DNL CloudConvert] gratuito ofrece 25 minutos de conversión al día. Si su uso excede el límite del plan gratuito, puede cambiar a un paquete o suscripción (prepagado).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p><span style="font-weight: normal;">[!UICONTROL No se pudo leer el tamaño de fotograma: no se pudo buscar en 1508. �/output/JLIADSA00137P0.mp3: argumento no válido.]</span> </p> </td> 
   <td> <p>Este error se produce, por ejemplo, al convertir archivos de MP3 a WAV. Asegúrese de haber seleccionado la región correcta porque encontrará referencias a archivos, pero no solo al archivo correcto.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL ErrorDeTiempoDeEjecución:] </p> <p><span style="font-weight: normal;">[!UICONTROL Se ha superado el número máximo de repeticiones.]</span> </p> </td> 
   <td> <p>Busque el trabajo [!DNL CloudConvert] correspondiente en la lista de trabajos del panel [!DNL CloudConvert] y compruebe la duración del trabajo:</p> <p> <img src="assets/cloudconvert-duration-350x177.png" style="width: 350;height: 177;"> </p> <p>El tiempo de espera del módulo [!DNL CloudConvert] &gt; [!UICONTROL Convert a File] se establece en 3 minutos. Si la duración del trabajo supera los 3 minutos (posiblemente debido a una sobrecarga temporal del servicio [!DNL CloudConvert]), el módulo genera el error mencionado anteriormente.</p> <p>En este caso, considere una de estas opciones:</p> 
    <ul> 
     <li>Habilite la opción <strong>[!UICONTROL Permitir almacenamiento de ejecuciones incompletas]</strong> en la configuración del escenario para almacenar las ejecuciones incompletas para una resolución manual posterior. Opcionalmente, puede adjuntar una ruta de control de errores al módulo [!DNL CloudConvert] con la directiva [!UICONTROL Break] para resolver automáticamente las ejecuciones incompletas.</li> 
     <li>Deshabilite la opción <strong>[!UICONTROL Descargar un archivo]</strong> en el módulo [!DNL CloudConvert] &gt; [!UICONTROL Convertir un archivo]. En este caso, el módulo no esperará el resultado de la conversión. Para obtener el resultado de la conversión, cree un nuevo escenario y use el déclencheur [!DNL CloudConvert] &gt; [!UICONTROL Nuevo evento de trabajo].</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Ejemplo de flujo de trabajo para el conector [!DNL CloudConvert]

>[!INFO]
>
>**Ejemplo:** Conversión de un vídeo de formato MOV a MP4
>
>1. Visite [https://cloudconvert.com/video-converter](https://>cloudconvert.com/video-converter)
>1. Haga clic en **[!UICONTROL Seleccionar archivo]** y elija el archivo MOV de muestra.
>1. Haga clic en el menú desplegable situado junto a **[!UICONTROL Convertir en]** y elija **[!UICONTROL MP4]**.
>
>1. Haga clic en el icono **[!UICONTROL llave inglesa]**.
>1. Configure los ajustes de compresión de MP4 como lo crea conveniente.
>1. Haga clic en **[!UICONTROL Convertir]**.
>1. Una vez completada la conversión, haz clic en **[!UICONTROL Descargar]**.
>1. Revise el vídeo convertido.
>1. Repita los pasos del 1 al 8 hasta que encuentre la configuración de conversión óptima para el paso 5.
>1. Visite [https://cloudconvert.com/api/v2/convert#convert-tasks](https://cloudconvert.com/api/v2/convert#convert-tasks)
>1. Elija **[!UICONTROL mov]** para el campo **[!UICONTROL input_format]**.
>
>1. Elija **[!UICONTROL mp4]** para el campo **[!UICONTROL output_format]**.
>
>1. Una lista de todos los parámetros posibles como video_codec, crf, etc. aparecerán.
>1. En Workfront Fusion 2.0, inserte el módulo **[!UICONTROL CloudConvert]** > **[!UICONTROL Convertir un archivo]** en su escenario.
>
>1. Abra la configuración del módulo.
>1. Configure el módulo como se muestra a continuación:
>
>   ![](assets/cloudconvert-mp4-example.png)
>
>1. Asegúrese de incluir todos los ajustes en el campo Conversión y opciones específicas del motor: para cada ajuste del paso 5, busque el parámetro correspondiente del paso 13 y su valor correspondiente.
