---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: La herramienta Power BI no se puede conectar con la contraseña proporcionada
description: Cuando intenta iniciar sesión en Data Connect desde la herramienta Power BI, se produce un error de inicio de sesión.
author: Courtney
feature: Reports and Dashboards
exl-id: c3f2b4a9-0831-48f0-871b-486d09ae5ea4
TQID: https://experienceleague.adobe.com/Z4RrMAPGd3CCti-cQFiJ7hlf-h8-suXeuoYfzk-9aKo
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
  - id: c1579802-ddd4-4214-8a91-97b2066abe11
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 229
ht-degree: 6%

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
