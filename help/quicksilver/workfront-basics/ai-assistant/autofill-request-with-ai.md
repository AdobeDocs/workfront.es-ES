---
title: Rellenar automáticamente una solicitud mediante IA
content-type: reference
description: Puede utilizar IA para rellenar automáticamente los campos de solicitud.
author: Becky
feature: Get Started with Workfront
exl-id: d053e604-5a28-4fd3-8f89-4467b6e46f02
source-git-commit: 977817157e016b7cbe591d8627031208d7bf3bb3
workflow-type: tm+mt
source-wordcount: '856'
ht-degree: 3%

---

# Rellenar automáticamente una solicitud mediante IA

>[!NOTE]
>
>Actualmente, esta funcionalidad forma parte de una versión beta cerrada. Para activar esta funcionalidad, póngase en contacto con sargism@adobe.com.
>
>Para poder acceder a la versión beta cerrada, su organización debe cumplir los requisitos para utilizar el asistente de IA de Workfront. Para obtener más información, consulte [Requisitos previos para el asistente de IA](/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md#prerequisites-to-ai-assistant).

AI puede ayudarle a rellenar automáticamente los campos de solicitud. Puede sugerir valores de campo basados en solicitudes anteriores o analizarlos a partir de texto como correos electrónicos o documentos cargados.

Puede aprobar o rechazar estas sugerencias antes de enviar la solicitud.

El relleno automático no sobrescribe los campos que ya haya rellenado.

## Obtener sugerencias al rellenar el formulario

El relleno automático puede sugerir valores de campo mientras rellena el formulario. A medida que introduce valores en los campos de solicitud, Workfront compara esos valores con las solicitudes anteriores. Si el valor introducido se correlaciona estrechamente con otros valores de campo en contextos similares en solicitudes anteriores, Workfront sugiere esos valores.

Por ejemplo, si una clínica siempre utiliza el mismo código de facturación, Workfront sugeriría ese código de facturación en el campo apropiado cuando se introduzca el nombre de la clínica.

Para utilizar sugerencias basadas en solicitudes anteriores:

1. Comience a crear una solicitud.

   Para obtener instrucciones, consulte [Crear y enviar solicitudes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Empiece a rellenar los campos.

   A medida que rellena los campos, otros campos pueden mostrar sugerencias.

1. Para cada sugerencia de campo, seleccione **Aceptar** o **Rechazar** debajo de ese campo.

   O

   Seleccione **Aceptar todo** o **Rechazar todo** en la parte superior de la página para aceptar o rechazar todas las sugerencias.

## Obtener sugerencias de un mensaje de texto

El relleno automático puede sugerir valores de campo basados en texto como correos electrónicos. Se pega en un bloque de texto y Workfront procesa el texto para sugerir valores de campo basados en el texto.

Por ejemplo, si el correo electrónico incluye &quot;Vence el 1 de junio&quot; y el formulario de solicitud tiene un campo para la fecha de vencimiento, Workfront sugeriría el 1 de junio para ese valor de campo.

Este tipo de sugerencia también comprueba las solicitudes anteriores para contextos similares. Por ejemplo, si el mensaje indica que la solicitud es para un cliente determinado, Workfront puede localizar e introducir la dirección de facturación de ese cliente automáticamente, en función de solicitudes anteriores.

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
1. Para cada sugerencia de campo, seleccione **Aceptar** o **Rechazar** debajo de ese campo.

   O

   Seleccione **Aceptar todo** o **Rechazar todo** en la parte superior de la página para aceptar o rechazar todas las sugerencias.

## Obtener sugerencias basadas en un documento que cargue

El relleno automático puede sugerir valores de campo basándose en un documento que cargue.

Este tipo de sugerencia también comprueba las solicitudes anteriores para contextos similares. Por ejemplo, si el mensaje indica que la solicitud es para un cliente determinado, Workfront puede localizar e introducir la dirección de facturación de ese cliente automáticamente, en función de solicitudes anteriores.

### Protecciones de carga de documentos

#### Tipos de archivos compatibles

Se admiten los siguientes tipos de archivo:

* BMP
* CSV
* DOC
* DOCX
* GIF
* JPEG
* JPG
* ODP
* ODS
* ODT
* PDF
* PNG
* PPT
* PPTX
* RTF
* TIFF
* TXT
* XLS
* XLSX

#### Tamaño de archivo compatible

Cada archivo puede tener un tamaño de hasta 100 MB

#### Número de archivos

Puede cargar hasta 50 archivos (páginas, diapositivas u hojas).

>[!IMPORTANT]
>
>Los documentos se convierten en una serie de imágenes, cada una de las cuales se considera un archivo independiente.
>
>Por ejemplo, puede cargar un archivo de PowerPoint con 50 diapositivas o 5 documentos de Word con 10 páginas cada uno.

#### Otras prácticas recomendadas

Tenga en cuenta lo siguiente al cargar un documento para el relleno automático de la solicitud:

* El relleno automático está optimizado actualmente para el alfabeto latino.
* Se recomienda utilizar un tamaño de texto de 8 puntos o superior.
* El relleno automático puede tener dificultades con las imágenes del documento, como imágenes rotadas o distorsionadas, gráficos y recuentos o usos de motivos espaciales en los objetos de las imágenes.
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
1. Para cada sugerencia de campo, seleccione **Aceptar** o **Rechazar** debajo de ese campo.

   O

   Seleccione **Aceptar todo** o **Rechazar todo** en la parte superior de la página para aceptar o rechazar todas las sugerencias.
