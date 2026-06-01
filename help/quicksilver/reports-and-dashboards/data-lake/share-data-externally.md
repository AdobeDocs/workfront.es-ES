---
content-type: overview;reference
product-area: reports and dashboards
navigation-topic: data connect
title: Establecimiento de una conexión con Workfront Data Conect
description: Workfront Data Connect le permite utilizar los datos de Workfront de su organización con herramientas de inteligencia empresarial o almacenarlos en un almacén de datos externo.
author: Courtney
feature: Reports and Dashboards
exl-id: 8348f5ff-c1f8-4608-b683-15f6407c6128
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: d7577da92b7efda5cba26104efac124f75a271c5
workflow-type: tm+mt
source-wordcount: '1489'
ht-degree: 22%

---

# Establecimiento de una conexión con Workfront Data Conect

Workfront Data Connect le permite utilizar los datos de Workfront de su organización con herramientas de inteligencia empresarial o almacenarlos en un almacén de datos externo.

Para conectar el repositorio de datos de Data Connect con un producto externo, primero debe crear una conexión como se describe en [Crear una cuenta de lector o una conexión para Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md). A continuación, debe agregar las IP necesarias a la lista de permitidos tal como se describe en [Agregar IP a la lista de permitidos](#add-ips-to-the-allowlist) siguiente.

La mayoría de los productos necesitarán la siguiente información sobre su lago de datos para establecer una conexión:

| Nombre de campo | Valor |
|---------------|-------------|
| Servidor | Dirección URL de la conexión, sin la parte `https://` (que se encuentra en la página **Conexión de datos** de Workfront*) |
| Puerto | `443` |
| Base de datos | `WORKFRONT` |
| Almacén | `READER_WH` |
| Esquema | `WF` |
| Función | `READER_ROLE` |
| Nombre de usuario | Nombre de usuario elegido al crear la conexión (encontrado en la página **Data Connect** de Workfront*) |
| Contraseña | Contraseña elegida en el primer inicio de sesión en Snowflake* |

*Para obtener información sobre dónde encontrar la página de **Data Connect** que contiene sus conexiones, consulte [Crear una cuenta de lector o una conexión para Snowflake](/help/quicksilver/reports-and-dashboards/data-lake/create-a-reader-account.md).

>[!IMPORTANT]
>
>Una vez añadida una entrada a la lista de permitidos IP, ya no se permitirán otras direcciones IP. Asegúrese de haber introducido todas las direcciones IP necesarias (tanto para las experiencias de creación como de lectura de la herramienta de visualización) antes de intentar utilizar la herramienta. Si no es así, puede encontrarse un error relacionado con las credenciales no válidas.
>
>Si no tiene ninguna dirección IP incluida en la lista de permitidos pero sigue teniendo problemas para conectarse a una herramienta de BI, compruebe en la configuración del servidor proxy la herramienta de BI.

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Paquete de Adobe Workfront</td> 
   <td><p>Ultimate</p>
    <p>Workflow Ultimate</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Estándar</p>
   <p>Plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir direcciones IP a la lista de permitidos

1. Haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configuración**.

1. En el panel izquierdo, haga clic en **Sistema** > **Conexión de datos**.

1. Haga clic en la pestaña **IP permitidas** y luego haga clic en el botón **Añadir una dirección IP a su lista de permitidos**.

1. Escriba un nombre de la dirección IP en **Descripción de la dirección IP** e introduzca la dirección IP (o bloque CIDR) para la herramienta que desea utilizar en **Dirección IP**; a continuación, haga clic en **Añadir IP a la Lista de permitidos**.

   ![Agregar dirección IP](/help/quicksilver/reports-and-dashboards/data-lake/assets/add-IP-allowlist.png) {width="500"}

## Buscar rangos de IP de Azure para Microsoft Power BI

El tráfico de Microsoft Power BI a Data Connect no procede de una sola dirección fija. Microsoft publica los rangos de IP como bloques CIDR en un archivo JSON grande. En esta sección se explica cómo encontrar los bloques para las regiones que realmente utiliza.

### Fuente oficial de Microsoft para rangos de IP de Azure y etiquetas de servicio

Microsoft publica la lista en la [página de descarga de intervalos de IP de Azure y etiquetas de servicio: nube pública](https://www.microsoft.com/en-us/download/details.aspx?id=56519). Descargue el archivo JSON actual (el nombre de archivo suele ser similar a `ServiceTags_Public_YYYYMMDD.json`). Actualice la lista de permitidos cuando Microsoft actualice este archivo o cuando aparezcan problemas de conectividad tras un cambio de Microsoft.

>[!NOTE]
>
>El archivo JSON es muy grande, a menudo con más de 100 000 líneas. Eso es esperable. Las secciones que necesita son pequeñas; no necesita leer todo el archivo a mano.

### Power BI frente a Power Query Online

Los clientes a veces informan de &quot;Power BI&quot; cuando el tráfico realmente proviene de componentes de Power Query que Microsoft trata como un servicio de Azure independiente en la lista de etiquetas de servicio.

| Si sus usuarios... | Busque esta etiqueta de servicio en el archivo JSON |
|----------------|---------------------------------------|
| Utilice el servicio de Power BI, los conjuntos de datos alojados en Azure o las puertas de enlace en el contexto de la nube | `PowerBI` (entradas globales o regionales como `PowerBI.EastUS`) |
| Uso de Power Query Online, flujos de datos en la nube y experiencias similares | `PowerQueryOnline` (entradas globales o regionales como `PowerQueryOnline.EastUS`) |

Si su organización utiliza ambas experiencias, agregue bloques CIDR de `PowerBI` y `PowerQueryOnline` para las mismas regiones. Si solo agrega uno, es posible que algunos usuarios sigan bloqueados mientras que otros lo logran.

### Elija etiquetas regionales, no el agregado global

El archivo JSON contiene una sola entrada de todas las regiones para `PowerBI` (y de manera similar para `PowerQueryOnline`) que agrega muchas regiones y puede contener cientos de bloques CIDR, además de muchas entradas regionales más pequeñas como `PowerBI.WestUS`, `PowerBI.WestUS2` y `PowerBI.WestUS3`. Cada objeto regional enumera únicamente los prefijos de esa región, normalmente decenas de líneas como máximo. No se recomienda añadir la entrada global a menos que tenga un requisito documentado para permitir todas las regiones de Azure. Para la mayoría de los clientes de Data Connect, las entradas regionales son las predeterminadas correctas. Añada las regiones en las que realmente se ejecutan los inquilinos y usuarios de Power BI, además de un pequeño búfer para la redundancia (por ejemplo, una región secundaria de recuperación ante desastres que utiliza su compañía).

### Elige tus regiones

Los nombres de región de Microsoft en el archivo tienen el aspecto de `EastUS`, `WestEurope`, `GermanyWestCentral`, etc. Utilice las regiones donde están alojados su capacidad y los usuarios de Power BI, no donde está su oficina, aunque a menudo están alineados.

| Escenario | Qué agregar primero |
|----------|-------------------|
| Uso de Estados Unidos | Comience con las regiones de EE. UU. que conozca que usa su inquilino (ejemplos: `EastUS`, `EastUS2`, `WestUS`, `WestUS2`, `WestUS3`, `CentralUS`, `SouthCentralUS`). No necesita todas las regiones de EE. UU. a menos que el administrador de Microsoft confirme el alojamiento de varias regiones. |
| Uso de la Unión Europea o del Reino Unido | Comience con las regiones que utiliza su inquilino (ejemplos: `WestEurope`, `NorthEurope`, `FranceCentral`, `GermanyWestCentral`, `SwedenCentral`, `UKSouth`). Agregue más solo si los usuarios abarcan regiones de Microsoft adicionales. |
| Uso de Asia-Pacífico | Agregue las regiones confirmadas por el administrador de Power BI o Azure (ejemplos: `SoutheastAsia`, `EastAsia`, `AustraliaEast`). |
| Varias regiones geográficas | Agregue ambos conjuntos de etiquetas regionales (por ejemplo, UE y EE.UU.) para cada servicio (`PowerBI` y `PowerQueryOnline` si ambos están en uso). |
| Región desconocida | Pregunte al administrador de Microsoft 365 o Power BI qué regiones de Azure alojan los recursos de Power BI o revise la configuración del inquilino de administración de Power BI. Si debe desbloquear rápidamente para realizar pruebas, agregue un par de regiones conocido (por ejemplo, `EastUS` y `WestUS`) y monitorice y, a continuación, reduzca la lista una vez que confirme. |

### Buscar rangos de IP y agregarlos a la lista de permitidos

Para recopilar rangos de IP de Microsoft y añadirlos a la lista de permitidos de Workfront:

1. Abra la página de descarga de [Rangos de IP de Azure y etiquetas de servicio - Nube pública](https://www.microsoft.com/en-us/download/details.aspx?id=56519), descargue el archivo JSON de etiquetas de servicio y guárdelo localmente (por ejemplo, `Downloads\ServiceTags_Public_YYYYMMDD.json`).

1. Abra el archivo en cualquier editor que también administre archivos JSON grandes, como Visual Studio Code.

1. Utilice la característica Buscar del editor (`Ctrl+F` en Windows o `Cmd+F` en macOS) para localizar objetos JSON cuyo campo de `"name"` sea igual a una etiqueta de servicio como `PowerBI.EastUS` o `PowerQueryOnline.WestEurope`. Búsquedas útiles:

   * `"name": "PowerBI.WestUS"` — saltar a West US Power BI.
   * `"name": "PowerQueryOnline.WestUS"`: salte a West US Power Query Online.
   * `PowerBI.`: enumera todas las etiquetas regionales de Power BI y, a continuación, refine el nombre de su región.

1. En cada objeto coincidente, busque la matriz denominada `addressPrefixes`. Cada cadena de esa matriz es un bloque CIDR (por ejemplo, `20.59.79.96/27` o un prefijo IPv6). Estos son los valores que agregará a la lista de permitidos de Workfront.

1. Agregue cada CIDR a la lista de permitidos de Workfront como se describe en [Agregue direcciones IP a la lista de permitidos](#add-ips-to-the-allowlist) en este artículo. Espere unos minutos para la propagación de la directiva si su entorno almacena en caché las reglas.

1. Desde Power BI o Power Query Online, ejecute una pequeña consulta de prueba con Data Connect para validar la conexión. Si falla, capture el tiempo aproximado y pregunte al equipo de red si las denegaciones se alinean con los intervalos que faltan. Vuelva a comprobar si se perdió `PowerQueryOnline` cuando solo se agregó `PowerBI`, lo cual es un hueco común.

Por ejemplo, si el administrador de Microsoft confirma que las cargas de trabajo de Power BI utilizan las versiones oeste de EE. UU., oeste de EE. UU. 2 y oeste de EE. UU. 3, y los usuarios utilizan Power BI y Power Query Online, debe abrir seis objetos: `PowerBI.WestUS`, `PowerBI.WestUS2`, `PowerBI.WestUS3` y los `PowerQueryOnline.<Region>` coincidentes para cada uno, y después copiar `addressPrefixes` de los seis.

### Referencia de estructura de JSON

Conceptualmente, cada bloque de etiqueta de servicio tiene el siguiente aspecto. Los archivos reales incluyen más metadatos.

```json
{
  "name": "PowerBI.WestUS2",
  "id": "PowerBI.WestUS2",
  "properties": {
    "region": "westus2",
    "systemService": "PowerBI",
    "addressPrefixes": [
      "203.0.113.0/24",
      "2001:db8::/32"
    ],
    "networkFeatures": ["API", "NSG", "UDR", "FW"]
  }
}
```

La matriz `addressPrefixes` contiene los bloques CIDR que agregará a Workfront. Otros campos son para escenarios de red de Azure y no se aplican aquí.

### Mantener la lista de permitidos

* Microsoft cambia los intervalos de IP con el tiempo. Cuando Microsoft publica un archivo JSON actualizado, actualice o compare la lista de permitidos periódicamente, especialmente después de un incidente de conectividad.
* Si su entorno admite IPv6 en Snowflake y Microsoft muestra los prefijos de IPv6, inclúyalos si la directiva de seguridad permite IPv6. De lo contrario, debe coordinarse con el equipo de red.

## Eliminar una dirección IP de la lista de permitidos

1. Haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configuración**.

1. En el panel izquierdo, haga clic en **Sistema** > **Conexión de datos**.

1. Haga clic en la pestaña **IP permitidas** y, a continuación, haga clic en el icono de la papelera ![Eliminar icono](/help/quicksilver/reports-and-dashboards/data-lake/assets/delete.png) a la derecha de la dirección IP que desea eliminar.

1. En la ventana que aparece, marque la casilla para confirmar y luego haga clic en **Eliminar**.

## Uso compartido de datos con herramientas de inteligencia empresarial

A continuación se enumeran una serie de herramientas comunes de inteligencia empresarial; visite sus sitios de documentación para obtener más información sobre la conexión a su lago de datos.

* Tableau
* Power BI
* Domo
* SAP HANA

## Almacenar datos en un almacén de datos externo

A continuación se enumeran una serie de almacenes de datos comunes; visite sus sitios de documentación para obtener más información sobre la conexión a su lago de datos.

* Databricks
* AWS Redshift
