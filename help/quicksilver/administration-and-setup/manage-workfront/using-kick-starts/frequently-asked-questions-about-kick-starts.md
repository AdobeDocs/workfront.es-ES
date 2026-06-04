---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: kickstart,kick-start,kickstarts,kick-starts
navigation-topic: use-kick-starts
title: Preguntas más frecuentes sobre Kick-Starts
description: Encuentre respuestas a las preguntas frecuentes sobre la importación y exportación de datos de Workfront mediante Kick-Starts.
author: LIsa
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
TQID: https://experienceleague.adobe.com/XpKG-fYAFVRk89b5TjSWyrzqv5z1zzIavWJQNLuKlsc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 441
ht-degree: 98%

---

# Preguntas frecuentes sobre Kick-Starts

A continuación, se muestran las preguntas frecuentes sobre Kick-Starts:

## ¿Por qué aparece este error al intentar importar un archivo de KickStart?: &quot;El archivo era correcto, pero no se importó nada&quot;

### Respuesta

Es posible que falte una de las tres cosas siguientes en el archivo de KickStart:

1. La columna **isNew** debe establecerse en **TRUE** para todos los elementos que desee importar. **isNew** debe ser **TRUE** porque solo puede importar datos nuevos con un Kick-Start. No puede modificar los datos existentes mediante KickStart. Puede tener otras filas en la hoja de cálculo con **isNew = FALSE**, pero estas filas no se importarán.

1. El archivo debe tener una fila vacía antes de que comiencen los encabezados de los datos.
1. La hoja u hojas de Excel deben tener los nombres correctos.

Al trabajar con Kick-Starts, le recomendamos que primero descargue la plantilla de Kick-start, la rellene manualmente con los datos correctos y, a continuación, la importe de nuevo a Adobe Workfront.

Para obtener más información sobre cómo importar correctamente datos en Workfront mediante Kick-Starts, consulte [Importar datos a Adobe Workfront mediante una plantilla de Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## ¿Por qué aparece este error al intentar importar horas a Workfront usando un archivo de KickStart?: “No se encontró un usuario con valor(es) de clave principal “null”

### Respuesta

El error hace referencia al GUID del usuario asociado a las horas.

Para solucionar este problema:

1. Exporte solamente una plantilla de KickStart en blanco para el objeto **Horas**.\
   Para obtener más información sobre la exportación de un archivo de KickStart en blanco, consulte &quot;Exportación de la plantilla de KickStart&quot; en [Importación de datos a Adobe Workfront mediante una plantilla de KickStart](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Copie manualmente los datos del Kick-Start original y péguelos en el archivo vacío.\
   Hágalo para cada columna.
1. Intente importar otra vez el nuevo archivo.\
   Kick-Start debe importarse correctamente.

## ¿Por qué el campo de país no se rellena en el perfil de usuario en una importación de KickStart?

### Problema

Al importar un KickStart de usuario con el campo **setCountry**, esos datos no llegan al país en el perfil de usuario.

### Respuesta

Si el usuario está habilitado para Unified User Management (UUM) o Adobe Identity Management System (IMS), el campo **País** solo acepta valores de código de país (por ejemplo, US, GB, IN). Compruebe que el campo **setCountry** de la plantilla de KickStart esté usando valores de código de país antes de realizar la importación.

Para obtener más información sobre cómo importar correctamente datos en Workfront mediante Kick-Starts, consulte [Importar datos a Adobe Workfront mediante una plantilla de Kick-Start](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
