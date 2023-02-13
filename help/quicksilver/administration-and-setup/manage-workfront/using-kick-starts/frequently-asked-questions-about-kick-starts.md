---
user-type: administrator
content-type: faq
product-area: system-administration
keywords: inicio rápido,inicio inicial,inicio rápido,inicio inicial
navigation-topic: use-kick-starts
title: Preguntas frecuentes sobre Kick-Starts
description: Encuentre respuestas a las preguntas más frecuentes sobre la importación y exportación de datos de Workfront mediante Kick-Starts.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f286e03e-93a8-43f5-8c2d-2c36203776a8
source-git-commit: 1ebdb3797e30a7e06f4dfd4a7e0e5f540351c126
workflow-type: tm+mt
source-wordcount: '415'
ht-degree: 0%

---

# Preguntas frecuentes sobre Kick-Starts

Las siguientes son las preguntas más frecuentes sobre Kick-Starts:

## ¿Por qué recibo este error al intentar importar un archivo de inicio rápido? &quot;Tu archivo era correcto, pero no se importó nada?&quot;

### Respuesta

Puede que falte una de las tres cosas siguientes en el archivo Inicio rápido:

1. La variable **isNew** se debe configurar como **TRUE** para todos los elementos que desea importar. **isNew** debe **TRUE** porque solo puede importar nuevos datos con un inicio rápido. No se pueden modificar los datos existentes mediante Inicio rápido. Puede tener otras filas en la hoja de cálculo con **isNew = FALSE** pero, estas filas no se importarán.

1. &#x200B; El archivo debe tener una fila vacía antes del inicio de los encabezados de los datos.
1. &#x200B; Las hojas de Excel necesitan tener los nombres correctos.

Al trabajar con Inicio rápido, se recomienda descargar primero la plantilla de inicio rápido, rellenarla manualmente con los datos correctos y luego importarla de nuevo en Adobe Workfront.

Para obtener más información sobre la importación correcta de datos en Workfront mediante Kick-Starts, consulte [Importar datos en Adobe Workfront mediante una plantilla de inicio rápido](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

## ¿Por qué recibo este error al intentar importar horas en Workfront mediante un archivo de inicio rápido? &quot;¿No se encuentra el usuario con los valores de clave principal &quot;null&quot;?&quot;

### Respuesta

El error hace referencia al GUID del usuario asociado con las horas.

Para solucionar esto:

1. Exportar una plantilla de inicio rápido en blanco para la variable **Horas** solo objeto.\
   Para obtener más información sobre la exportación de un archivo de inicio rápido en blanco, consulte &quot;Exportación de la plantilla de inicio rápido&quot; en  [Importar datos en Adobe Workfront mediante una plantilla de inicio rápido](../../../administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).

1. Copie manualmente los datos del Inicio de clic original y péguelos en el archivo vacío.\
   Haga esto para cada columna.
1. Intente importar el nuevo archivo de nuevo.\
   El inicio rápido debería importarse correctamente.

## ¿Por qué el campo de país no se rellena en el perfil de usuario en una importación de inicio rápido?

### Problema

Al importar un Inicio de la marca de usuario con el campo **setCountry**, esos datos no llegan al país en el perfil del usuario.

### Respuesta

Si el usuario está habilitado para la administración unificada de usuarios (UUM) o el sistema Identity Management de Adobe (IMS), la variable **País** solo acepta valores de código de país (por ejemplo, EE. UU., GB, IN). Compruebe que la variable **setCountry** en la plantilla Inicio rápido está utilizando valores de código de país antes de la importación.

Para obtener más información sobre la importación correcta de datos en Workfront mediante Kick-Starts, consulte [Importar datos en Adobe Workfront mediante una plantilla de inicio rápido](/help/quicksilver/administration-and-setup/manage-workfront/using-kick-starts/import-data-via-kickstarts.md).
