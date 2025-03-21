---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: La herramienta Power BI no se puede conectar con la contraseña proporcionada
description: Cuando intenta iniciar sesión en Data Connect desde la herramienta Power BI, se produce un error de inicio de sesión.
author: Courtney
feature: Reports and Dashboards
source-git-commit: 40050915153af6e1f70024461e193fb536d74e35
workflow-type: tm+mt
source-wordcount: '229'
ht-degree: 1%

---


# La herramienta Power BI no se puede conectar con la contraseña proporcionada

## Problema

Cuando intente iniciar sesión en Data Connect desde la herramienta Power BI, verá el siguiente error:

`Cannot connect from BI tool with provided password`

## Causa

Al crear la conexión JDBC, Workfront proporciona una contraseña temporal para la conexión de datos.

Antes de acceder a Data Connect a través de Power BI, primero debe iniciar sesión con los datos de conexión proporcionados, actualizar la contraseña temporal y, a continuación, iniciar sesión.


## Solución

Restablezca la contraseña de conexión en Workfront y, a continuación, cree una nueva contraseña con el vínculo proporcionado en el cuadro de diálogo Editar conexión.

### Restablecer la contraseña de conexión en Workfront

1. Vaya a Workfront > Configuración > Sistema > Data Connect.
1. Busque y abra la conexión desde la lista.
1. En **Restablecer contraseña de conexión**, marque la casilla para confirmar que desea restablecer la contraseña.
1. Haga clic en **Restablecer contraseña de conexión**.
   ![restablecer contraseña de conexión](assets/reset-password.png)
1. Continúe en la sección siguiente.

### Cree una nueva contraseña para la conexión

1. Copie la dirección URL y péguela en una nueva pestaña del explorador.
1. En Workfront, copie y pegue el Nombre de usuario de conexión y la Contraseña predeterminada en la nueva pestaña del explorador.
   ![copiar url y contraseña predeterminada](assets/link-password.png)
1. Haga clic en **Iniciar sesión**.
1. Escriba una nueva contraseña y luego haga clic en **Enviar**.
1. Vaya a la herramienta Power BI e inicie sesión con la nueva contraseña.

