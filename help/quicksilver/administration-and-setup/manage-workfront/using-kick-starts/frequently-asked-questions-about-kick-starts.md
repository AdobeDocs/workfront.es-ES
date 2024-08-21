---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: KickStart, KickStart, KickStart, KickStart
navigation-topic: use-kick-starts
title: Preguntas más frecuentes sobre Kick-Starts
description: Encuentre respuestas a las preguntas más frecuentes acerca de la importación y exportación de datos de Workfront mediante Kick-Starts.
author: LIsa
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 01487bb9cb195d6fa89bbe0fbdb7678254642714
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Preguntas frecuentes sobre Kick-Starts

Las siguientes son las preguntas más frecuentes sobre Kick-Starts:

## ¿Por qué aparece este error al intentar importar un archivo de KickStart?: &quot;El archivo era correcto, pero no se importó nada?&quot;

### Respuesta

Es posible que falte una de las tres cosas siguientes en el archivo de KickStart:

1. La columna **isNew** debe establecerse en **TRUE** para todos los elementos que desee importar. **isNew** debe ser **TRUE** porque solo puede importar datos nuevos con un Kick-Start. No se pueden modificar los datos existentes mediante KickStart. Puede tener otras filas en la hoja de cálculo con **isNew = FALSE**, pero estas filas no se importarán.

1. &#x200B;El archivo debe tener una fila vacía antes de que comiencen los encabezados de los datos.
1. &#x200B;Las hojas de Excel deben tener los nombres correctos.

Al trabajar con Kick-Starts, recomendamos descargar primero la plantilla de Kick-start, rellenarla manualmente con los datos correctos y, a continuación, importarla de nuevo en Adobe Workfront.

Para obtener más información sobre cómo importar correctamente datos en Workfront mediante Kick-Starts, consulte [Importar datos en Adobe Workfront mediante una plantilla de Kick-Start](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## ¿Por qué recibo este error al intentar importar horas en Workfront usando un archivo de KickStart?: &quot;No se encontró un usuario con valor(es) &quot;null&quot; de clave principal?&quot;

### Respuesta

El error hace referencia al GUID del usuario asociado con las horas.

Para solucionar esto:

1. Exporte solamente una plantilla de KickStart en blanco para el objeto **Hours**.\
   Para obtener más información acerca de la exportación de un archivo de KickStart en blanco, consulte &quot;Exportación de la plantilla de KickStart&quot; en [Importación de datos en Adobe Workfront mediante una plantilla de KickStart](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Copie manualmente los datos del Kick-Start original y péguelos en el archivo vacío.\
   Haga esto por cada columna.
1. Intente importar el nuevo archivo de nuevo.\
   Kick-Start debe importarse correctamente.

## ¿Por qué el campo de país no se rellena en el perfil de usuario en una importación de KickStart?

### Problema

Al importar un KickStart de usuario con el campo **setCountry**, esos datos no llegan al país en el perfil de usuario.

### Respuesta

Si el usuario está habilitado para Unified User Management (UUM) o Adobe Identity Management System (IMS), el campo **País** solo acepta valores de código de país (por ejemplo, EE. UU., GB, IN). Compruebe que el campo **setCountry** de la plantilla de KickStart esté usando valores de código de país antes de realizar la importación.

Para obtener más información sobre cómo importar correctamente datos en Workfront mediante Kick-Starts, consulte [Importar datos en Adobe Workfront mediante una plantilla de Kick-Start](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
