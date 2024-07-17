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
source-git-commit: 91371c862be6f3b99f0450ff359f601dc913dc0c
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 1%

---

# Establezca una conexión con el lago de datos de Workfront

El lago de datos de Workfront le permite utilizar los datos de Workfront de su organización con herramientas de inteligencia empresarial o almacenarlos en un almacén de datos externo.

Para conectar los datos del lago de datos de Workfront con un producto externo, primero debe agregar las IP necesarias a la lista de permitidos, tal como se describe en [Agregar IP a la lista de permitidos](#add-ips-to-the-allowlist) siguiente. Además, la mayoría de los productos necesitarán información adicional sobre su lago de datos para establecer una conexión:

| Nombre de campo | Valor |
|---------------|-------------|
| Servidor | Dirección URL de la conexión, sin la parte `https://` (que se encuentra en la página **Acceso a datos** de Workfront*) |
| Puerto | `443` |
| Base de datos | `WORKFRONT` |
| Almacén | `READER_WH` |
| Esquema | `WF` |
| Función | `READER_ROLE` |
| Nombre de usuario | Nombre de usuario elegido al crear la conexión (encontrado en la página **Acceso a datos** de Workfront*) |
| Contraseña | La contraseña elegida al iniciar sesión el primer Snowflake* |

*Para obtener información sobre dónde encontrar la página de **Acceso a datos** que contiene las conexiones del lago de datos, consulte [Crear una cuenta de lector (servicio) para el Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Una vez que se añade una entrada a la lista de permitidos IP, ya no se permiten las demás direcciones IP. Asegúrese de haber introducido todas las direcciones IP necesarias (tanto para la experiencia de creación como de lectura de la herramienta de visualización) antes de intentar utilizar la herramienta. Si no es así, puede encontrar un error relacionado con las credenciales no válidas.
>
>Si no tiene ninguna dirección IP incluida en la lista de permitidos pero sigue teniendo problemas para conectarse a una herramienta de BI, compruebe la configuración del servidor proxy para la herramienta de BI.


## Añadir direcciones IP a la lista de permitidos

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Acceso a datos**.

1. Haz clic en la pestaña **IP permitidas** y luego haz clic en el botón **Agregar una dirección IP a tu Lista de permitidos**.

1. Escriba un nombre para la dirección IP en **Descripción de la dirección IP** e introduzca la dirección IP (o bloque CIDR) para la herramienta que desea usar en **Dirección IP**; a continuación, haga clic en **Agregar IP a la Lista de permitidos**.

   ![Agregar dirección IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Eliminar una dirección IP de la lista de permitidos

1. Haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configurar**.

1. En el panel izquierdo, haga clic en **Sistema** > **Acceso a datos**.

1. Haga clic en la ficha **IP permitidas** y, a continuación, haga clic en el icono de la papelera ![Eliminar icono](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a la derecha de la dirección IP que desee eliminar.

1. En la ventana que aparece, marque la casilla para confirmar y luego haga clic en **Eliminar**.

## Uso compartido de datos con herramientas de Business Intelligence

A continuación se enumeran una serie de herramientas comunes de inteligencia empresarial; los vínculos le llevarán al sitio de documentación del servicio para obtener más información sobre la conexión a su lago de datos.

* [Tableau](https://help.tableau.com/current/pro/desktop/en-us/basicconnectoverview.htm)
* [Power BI](https://learn.microsoft.com/power-query/connectors/snowflake)
* [Dominio](https://www.domo.com/appstore/connector/snowflake-connector/overview)
* SAP HANA

## Almacenar datos en un almacén de datos externo

A continuación se enumeran una serie de almacenes de datos comunes; los vínculos le llevarán al sitio de documentación de cada servicio, donde podrá obtener más información sobre la conexión a su lago de datos.

* [Databricks](https://docs.databricks.com/en/connect/index.html)
* [AWS Redshift](https://docs.aws.amazon.com/redshift/latest/gsg/federated-query.html)
