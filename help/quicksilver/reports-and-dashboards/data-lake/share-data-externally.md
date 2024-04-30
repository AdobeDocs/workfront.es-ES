---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data lake
title: Establezca una conexión con el lago de datos de Workfront
description: El lago de datos de Workfront le permite utilizar los datos de Workfront de su organización con herramientas populares de inteligencia empresarial o almacenarlos en un almacén de datos externo.
author: Nolan
feature: Reports and Dashboards
recommendations: noDisplay, noCatalog
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
source-git-commit: 508e3c786bc6cfe676fb2cb33080c99b76c3d6a0
workflow-type: tm+mt
source-wordcount: '502'
ht-degree: 1%

---

# Establezca una conexión con el lago de datos de Workfront

El lago de datos de Workfront le permite utilizar los datos de Workfront de su organización con herramientas de inteligencia empresarial o almacenarlos en un almacén de datos externo.

Para conectar los datos del lago de datos de Workfront con un producto externo, primero debe agregar las IP necesarias a la lista de permitidos, tal como se describe en [Añadir direcciones IP a la lista de permitidos](#add-ips-to-the-allowlist) más abajo. Además, la mayoría de los productos necesitarán información adicional sobre su lago de datos para establecer una conexión:

| Nombre de campo | Valor |
|---------------|-------------|
| Servidor | La dirección URL de la conexión, sin `https://` parte (que se encuentra en la **Acceso a datos** página en Workfront*) |
| Puerto | `443` |
| Base de datos | `WORKFRONT` |
| Almacén | `READER_WH` |
| Esquema | `WF` |
| Función | `READER_ROLE` |
| Nombre de usuario | El nombre de usuario elegido al crear la conexión (que se encuentra en la **Acceso a datos** página en Workfront*) |
| Contraseña | La contraseña elegida al iniciar sesión el primer Snowflake* |

*Para obtener información sobre dónde encontrar el **Acceso a datos** página que contiene las conexiones del lago de datos, consulte [Crear una cuenta de Reader (servicio) para Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Una vez que se añade una entrada a la lista de permitidos IP, ya no se permiten las demás direcciones IP. Asegúrese de haber introducido todas las direcciones IP necesarias (tanto para la experiencia de creación como de lectura de la herramienta de visualización) antes de intentar utilizar la herramienta. Si no es así, puede encontrar un error relacionado con las credenciales no válidas.

## Añadir direcciones IP a la lista de permitidos

1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Acceso a datos**.

1. Haga clic en **IP permitidas** y, a continuación, haga clic en **Añadir una dirección IP a la Lista de permitidos** botón.

1. Introduzca un nombre para la dirección IP en **Descripción de dirección IP** e introduzca la dirección IP (o bloque CIDR) de la herramienta que desea utilizar en **Dirección IP**, luego haga clic en **Añadir IP a la Lista de permitidos**.

   ![Añadir dirección IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Eliminar una dirección IP de la lista de permitidos

1. Haga clic en **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el botón **[!UICONTROL Menú principal]** icono ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Acceso a datos**.

1. Haga clic en **IP permitidas** pestaña, luego haga clic en el icono de la papelera ![Icono Eliminar](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a la derecha de la dirección IP que desea eliminar.

1. En la ventana que aparece, marque la casilla para confirmar y luego haga clic en **Eliminar**.

## Uso compartido de datos con herramientas de Business Intelligence

A continuación se enumeran una serie de herramientas comunes de inteligencia empresarial; los vínculos le llevarán al sitio de documentación del servicio para obtener más información sobre la conexión a su lago de datos.

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [Domo](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## Almacenar datos en un almacén de datos externo

A continuación se enumeran una serie de almacenes de datos comunes; los vínculos le llevarán al sitio de documentación de cada servicio, donde podrá obtener más información sobre la conexión a su lago de datos.

* [Databricks](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
