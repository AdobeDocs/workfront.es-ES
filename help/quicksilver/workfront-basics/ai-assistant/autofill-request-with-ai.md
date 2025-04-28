---
title: Rellenar automáticamente una solicitud mediante IA
content-type: reference
description: Puede utilizar IA para rellenar automáticamente los campos de solicitud.
author: Becky
feature: Get Started with Workfront
hide: true
hidefromtoc: true
source-git-commit: 9e1a5718092092bb9ca98cf92ddd2a1a07f32f51
workflow-type: tm+mt
source-wordcount: '443'
ht-degree: 0%

---

# Rellenar automáticamente una solicitud mediante IA

AI puede ayudarle a rellenar automáticamente los campos de solicitud. Puede sugerir valores de campo basados en solicitudes anteriores o analizarlos a partir de texto como correos electrónicos.

Puede aprobar o rechazar estos envíos antes de enviar la solicitud.

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

El relleno automático puede sugerir valores de campo basados en texto como correos electrónicos. Pegue un bloque de texto y Workfront procesará el texto para sugerir valores de campo basados en el texto.

Por ejemplo, si el correo electrónico incluye &quot;Vence el 1 de junio&quot; y el formulario de solicitud tiene un campo para la fecha de vencimiento, Workfront sugeriría el 1 de junio para ese valor de campo.

Este tipo de sugerencia también comprueba las solicitudes anteriores para contextos similares. Por ejemplo, si el mensaje indica que la solicitud es para un cliente determinado, Workfront puede localizar e introducir la dirección de facturación de ese cliente automáticamente, en función de solicitudes anteriores.

Puede pegar el texto para aplicarlo a todo el formulario o a una sola sección del formulario.

Para utilizar sugerencias basadas en un mensaje de texto pegado:

1. Comience a crear una solicitud.

   Para obtener instrucciones, consulte [Crear y enviar solicitudes](/help/quicksilver/manage-work/requests/create-requests/create-submit-requests.md).

1. Para aplicar el mensaje de texto a todo el formulario, haga clic en **Rellenar automáticamente con IA** en la esquina superior derecha de la pantalla.

   O

   Para aplicar el mensaje de texto para una sola sección, haga clic en el icono de IA ![Icono de IA](assets/request-prompt-icon.png) junto al nombre de la sección.

1. Pegue el texto en el cuadro de mensaje.
1. Haga clic en **Rellenar el formulario**.

   Workfront genera sugerencias para el formulario.
1. Para cada sugerencia de campo, seleccione **Aceptar** o **Rechazar** debajo de ese campo.

   O

   Seleccione **Aceptar todo** o **Rechazar todo** en la parte superior de la página para aceptar o rechazar todas las sugerencias.

