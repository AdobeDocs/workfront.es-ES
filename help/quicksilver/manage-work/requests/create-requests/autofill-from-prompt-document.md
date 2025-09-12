---
title: Utilizar el relleno de formulario AI para rellenar una solicitud utilizando indicaciones o documentos
content-type: reference
description: Puede utilizar IA para rellenar automáticamente los campos de solicitud introduciendo una solicitud o suministrando un documento.
author: Becky
feature: Get Started with Workfront
exl-id: 4a22f9ea-c9ee-4947-8683-9989c54903b1
source-git-commit: 2c46145ef24c6870239edc1e5fa96f88f4cb2fd7
workflow-type: tm+mt
source-wordcount: '1368'
ht-degree: 9%

---

# Utilizar el relleno de formulario AI para rellenar una solicitud utilizando indicaciones o documentos

>[!NOTE]
>
>* Esta funcionalidad estará disponible como una versión beta abierta en la siguiente programación:
>
>   * Versión mensual: 11 de septiembre de 2025
>   * Versión trimestral: 16 de octubre de 2025
>
>* Para utilizar esta funcionalidad, su organización debe cumplir los requisitos para utilizar Workfront AI Assistant. Para obtener más información, consulte [Requisitos previos para el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

Rellenar formularios de IA puede ayudarle a rellenar automáticamente los campos de solicitud en función de una solicitud que haya introducido. También puede rellenar campos basados en texto como correos electrónicos o documentos cargados. Puede aprobar o rechazar estas sugerencias antes de enviar la solicitud.

El relleno de formulario de IA no sobrescribe los campos que ya haya rellenado.

Los usuarios no reciben sugerencias de datos a los que no tienen acceso de otro modo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p>Nuevo: colaborador o superior</p>
   O
   <p>Actual: solicitud o superior</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Problemas</p>  </td> 
  </tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td><p>Acceso para añadir solicitudes a una cola de solicitudes</p> <p>Ver permisos superiores en la solicitud existente</p> <p>Para obtener información sobre cómo configurar una cola de solicitudes, consulte <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Crear una cola de solicitudes</a>. </p> </td> 
  <tr>
  </tr>
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Requisitos previos

Para usar el Relleno de formulario AI para rellenar solicitudes con un aviso o documento, se deben aplicar **todas** las siguientes condiciones:

* Su organización debe haber migrado a Adobe IMS (sistema Identity Management)
* La experiencia unificada de Adobe debe estar habilitada
* Su organización debe tener un plan Select, Prime o Ultimate Workfront
* Adobe debe tener registrado un acuerdo de Adobe Gen AI

  Para obtener más información sobre la firma del acuerdo, consulte [Firmar el acuerdo de IA de Adobe Gen](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#sign-the-adobe-gen-ai-agreement) en el artículo Información general del Asistente de IA.
* El asistente de IA debe estar habilitado en la configuración del sistema de su organización. Esto lo administra el administrador de Workfront.

  Para obtener más información sobre cómo habilitar el Asistente de IA en la configuración del sistema, consulte [Habilitar o deshabilitar el Asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/enable-or-disable-assistant.md).

## Obtener sugerencias de un mensaje de texto

El relleno de formulario AI puede sugerir valores de campo basados en texto como correos electrónicos. Se pega en un bloque de texto y Workfront procesa el texto para sugerir valores de campo basados en el texto.

Por ejemplo, si el correo electrónico incluye &quot;Vence el 1 de junio&quot; y el formulario de solicitud tiene un campo para la fecha de vencimiento, el rellenado del formulario de IA sugeriría el 1 de junio para ese valor de campo.

Al rellenar un formulario, Workfront también comprueba las solicitudes anteriores de contextos similares. Por ejemplo, si el mensaje indica que la solicitud es para un cliente determinado, Workfront puede localizar e introducir la dirección de facturación de ese cliente automáticamente, en función de solicitudes anteriores.

Puede pegar el texto para aplicarlo a todo el formulario o a una sola sección del formulario.

Para utilizar sugerencias basadas en un mensaje de texto pegado:

1. Comience a crear una solicitud.

   Para obtener instrucciones, consulte [Crear y enviar solicitudes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Para aplicar el mensaje de texto a todo el formulario, haga clic en el icono de IA ![Icono de IA](assets/request-prompt-icon.png) bajo el nombre del formulario.

   O

   Para aplicar el mensaje de texto para una sola sección, haga clic en el icono de IA ![Icono de IA](assets/request-prompt-icon.png) junto al nombre de la sección.

1. Pegue el texto en el cuadro de mensaje.
1. Haga clic en **Rellenar el formulario**.

   Workfront genera sugerencias para el formulario.
1. Para cada sugerencia de campo, seleccione **Aceptar** o **Rechazar** para ese campo.

   ![Aceptar o rechazar sugerencia](assets/accept-reject-suggestion.png)

   O

   Seleccione **Aceptar todo** o **Rechazar todo** en la parte superior de la página para aceptar o rechazar todas las sugerencias.

   >[!NOTE]
   >
   >Las sugerencias que no se hayan revisado se aceptarán automáticamente cuando envíe la solicitud.

### Ejemplos de mensajes de texto

Estos ejemplos muestran solicitudes de varias formas en las que la IA puede hacer referencia a otros proyectos.

#### Referencia a una campaña de clientes anterior

>[!BEGINSHADEBOX]

Cree una solicitud de campaña similar a la que hicimos para el lanzamiento del segundo trimestre de (empresa del cliente), pero esta vez para su división de Automoción. Mantenga el mismo conjunto de entregables y perfil de audiencia.

>[!ENDSHADEBOX]

#### Creación de un proyecto existente

>[!BEGINSHADEBOX]

Utilice la misma configuración que tuvimos en el inicio del proyecto (nombre del proyecto) la primavera pasada. Quiero ejecutar una campaña de publicidad digital dirigida a la misma audiencia ejecutiva, pero con fechas actualizadas para este trimestre.

>[!ENDSHADEBOX]

#### Reutilización de un estilo de un resultado anterior

>[!BEGINSHADEBOX]

Prepare una solicitud similar a la campaña de promoción de verano (de la compañía del cliente) que ejecutamos el año pasado. Céntrese en los activos de las redes sociales, mantenga el español como idioma principal y ajuste el presupuesto a $75,000.

>[!ENDSHADEBOX]

#### Ampliación de un tipo de campaña anterior

>[!BEGINSHADEBOX]

Tome como referencia la campaña de la serie de seminarios web (nombre de la campaña) del primer trimestre. Quiero el mismo flujo de trabajo de registro y activos, pero esta vez el tema es &quot;IA en la planificación financiera&quot; y la audiencia son profesionales jóvenes.

>[!ENDSHADEBOX]

#### Repetición de una solicitud para un producto diferente

>[!BEGINSHADEBOX]

Configure una solicitud de campaña como el proyecto de cambio de marca (de la empresa del cliente) que gestionamos, pero reemplace por (nueva empresa del cliente) como cliente. Mantenga todos los entregables alineados con la marca corporativa.

>[!ENDSHADEBOX]

#### Estilo narrativo con referencias implícitas

>[!BEGINSHADEBOX]

Estamos planeando una campaña similar a los anuncios sociales de las fiestas que publicamos el año pasado. El presupuesto debe ser de unos 50 000, el objetivo es la generación de posibles clientes y las entregas deben incluir recursos de Instagram y TikTok.

>[!ENDSHADEBOX]


## Obtener sugerencias basadas en un documento que cargue

El relleno automático puede sugerir valores de campo basándose en un documento que cargue.

Este tipo de sugerencia también comprueba las solicitudes anteriores para contextos similares. Por ejemplo, si el mensaje indica que la solicitud es para un cliente determinado, Workfront puede localizar e introducir la dirección de facturación de ese cliente automáticamente, en función de solicitudes anteriores.

### Protecciones de carga de documentos

#### Tipos de archivos compatibles

Se admiten los siguientes tipos de archivo:

<table>
<tr style="border: 0;">
<td>
<ul>
<li>BMP</li>
<li>CSV</li>
<li>DOC</li>
<li>DOCX</li>
<li>GIF</li>
<li>JPEG</li>
</ul>
</td>
<td>
<ul>
<li>ODP</li>
<li>ODS</li>
<li>ODT</li>
<li>PDF</li>
<li>PNG</li>
<li>PPT</li>
</ul>
</td>
<td>
<ul>
<li>PPTX</li>
<li>RTF</li>
<li>TIFF</li>
<li>TXT</li>
<li>XLS</li>
<li>XLSX</li>
</ul>
</td>
</tr>
</table>

#### Tamaño de archivo compatible

Cada archivo puede tener un tamaño de hasta 100 MB

#### Número de archivos

Puede cargar hasta 50 archivos (páginas, diapositivas u hojas).

>[!IMPORTANT]
>
>Los documentos se convierten en una serie de imágenes, cada una de las cuales se considera un archivo independiente.
>
>Por ejemplo, puede cargar un archivo de PowerPoint con 50 diapositivas o 5 documentos de Word con 10 páginas cada uno.

#### Tipos de campo admitidos

Los tipos de campo de Workfront afectan a si un campo determinado se puede rellenar automáticamente.

<table>
<tr>
<td><b>El relleno automático de </b><br> compatible puede rellenar</td>
<td><b>No compatible</b> <br>El relleno automático no se rellena</td>
</tr>
<tr>
<td>
<ul>
<li>Texto de línea única</li>
<li>Área de texto o párrafo</li>
<li>Campo de fecha</li>
<li>Casilla de verificación</li>
<li>Botones de radio</li>
<li>desplegables de selección única y múltiple</li>
</ul>
</td>
<td><li>Escritura anticipada</li>
<li>Búsqueda externa</li>
<li>Búsqueda interna</li>
<li>Referencia</li>
<li>Campos incrustados de WF Planning</li>
</ul>
</td>
</tr>
</table>

#### Otras prácticas recomendadas

Tenga en cuenta lo siguiente al cargar un documento en un relleno de formulario AI:

* El relleno de formulario AI está optimizado actualmente para el alfabeto latino.
* Se recomienda utilizar un tamaño de texto de 8 puntos o superior.
* El relleno de formulario de IA puede tener dificultades con las imágenes del documento, como imágenes rotadas o distorsionadas, gráficos y recuentos o usos de motivos espaciales en los objetos de las imágenes.
* Como siempre, recomendamos comprobar la precisión de los resultados antes de enviar la solicitud.

### Cargar un documento para rellenar automáticamente una solicitud

Puede cargar un documento para aplicarlo a todo el formulario o a una sola sección del formulario.

1. Comience a crear una solicitud.

   Para obtener instrucciones, consulte [Crear y enviar solicitudes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Para aplicar el documento a todo el formulario, haga clic en el icono de IA ![Icono de IA](assets/request-prompt-icon.png) bajo el nombre del formulario.

   O

   Para aplicar el documento a una sola sección, haga clic en el icono de IA ![Icono de IA](assets/request-prompt-icon.png) junto al nombre de la sección.

1. Haga clic en **Cargar archivos** y, a continuación, seleccione el archivo en el administrador de archivos.

   O

   Arrastre el documento desde el administrador de archivos hasta el cuadro **Cargar archivos para rellenar automáticamente el formulario de solicitud**.
1. Haga clic en **Rellenar el formulario** de **Rellenar la sección**.

   Workfront genera sugerencias para el formulario.
1. Para cada sugerencia de campo, seleccione **Aceptar** o **Rechazar** para ese campo.

   ![Aceptar o rechazar sugerencia](assets/accept-reject-suggestion.png)

   O

   Seleccione **Aceptar todo** o **Rechazar todo** en la parte superior de la página para aceptar o rechazar todas las sugerencias.

   >[!NOTE]
   >
   >Las sugerencias que no se hayan revisado se aceptarán automáticamente cuando envíe la solicitud.

## Resolución de problemas

Si no recibe las sugerencias esperadas, puede deberse a una de las siguientes causas:

* Debe tener al menos un mes de datos de solicitud en el sistema para poder sugerir valores de campo de solicitudes anteriores.
* Es posible que no haya seguido las protecciones de carga de documentos al cargar un documento desde el que extraer sugerencias. Para obtener más información, consulte [Protecciones de carga de documentos](#document-upload-guardrails) en este artículo.
