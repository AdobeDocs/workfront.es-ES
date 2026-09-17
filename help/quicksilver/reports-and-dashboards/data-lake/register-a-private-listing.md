---
content-type: reference
product-area: reports and dashboards
navigation-topic: data connect
title: Registrar un anuncio privado para Workfront Data Connect
description: Registre un anuncio privado de Snowflake para compartir los datos de Workfront Data Connect directamente con la cuenta de Snowflake de su organización.
author: Courtney
feature: Reports and Dashboards
exl-id:
last-update: 2026-09-15T00:00:00.000Z
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ed31fce397f9e99e7049d4f55eaca94f43dfcf5c
workflow-type: tm+mt
source-wordcount: '1060'
ht-degree: 6%
---
# Registrar un anuncio privado para Workfront Data Connect

Puede compartir sus datos de Workfront Data Connect directamente con la cuenta de Snowflake de su organización registrando un anuncio privado. Este método de conexión utiliza la capacidad de listado privado de Snowflake para compartir datos de forma segura entre organizaciones sin exponerlos públicamente, y funciona en varias regiones y plataformas de alojamiento.

Un anuncio privado resulta útil cuando desea unir los datos de Workfront con otros datos del almacén de datos empresarial. Como los datos aterrizan en su propia cuenta de Snowflake, puede consultarlos junto con el resto de los datos.

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

También necesita una cuenta de Snowflake con permisos para aceptar listas y crear bases de datos, y un derecho de Workfront Data Connect.

## Lo que comparte un anuncio privado

Un anuncio privado le permite acceder a lo siguiente:

* Más de 100 vistas de datos para objetos de Workfront. Para obtener descripciones de cada vista, consulte [Diccionario de datos de Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/data-dictionary.md).
* Las `*_event` vistas de datos, que contienen cada transacción de cambio enviada a las canalizaciones de datos de Data Connect.
* Valores de datos personalizados para objetos ampliables con datos. Para ver un ejemplo, vea el ejemplo de la consulta de datos personalizada en [ejemplos de consultas de Workfront Data Connect](/help/quicksilver/reports-and-dashboards/data-lake/basic-query-examples.md).

## Diferencias con respecto a una conexión de cuenta de lector

Un anuncio privado comparte un conjunto de vistas diferente a una conexión de cuenta de lector y los datos llegan en un horario diferente. Tenga en cuenta las siguientes diferencias:

* Un anuncio privado solo comparte las vistas `*_event`. Las vistas `*_current` y `*_daily_history` están disponibles a través de una cuenta de lector, pero no a través de un anuncio privado. Puede crearlos en su propia cuenta de Snowflake. Para obtener más información, consulte [Configurar las vistas Historial actual y Historial diario](#set-up-current-and-daily-history-views) en este artículo.
* Un anuncio privado puede no incluir todas las vistas disponibles a través de una cuenta de lector. Algunos ejemplos de vistas que no se comparten son los objetos de Workfront Planning, `MONITORING_DATA_REFRESHES`, `BOOKINGS` y `CLASSIFIER`. Esta lista no es exhaustiva.
* Las cargas de Data Connect cambian los eventos cada 4 horas. Dado que una lista privada requiere un paso de replicación adicional para que los datos aparezcan, espere que los datos tarden aproximadamente 1 hora más en llegar que a través de una cuenta de lector.
* La duplicación de datos se ejecuta a las 01:01, 05:01, 09:01, 13:01, 17:01 y 21:01 UTC. Los datos suelen estar disponibles unos 10 minutos después de cada ejecución.
* Las vistas `MONITORING_DATA_REFRESHES` y `JOB_HISTORY` no reflejan las horas en que los datos están disponibles a través de un anuncio privado. Aunque la vista `JOB_HISTORY` se comparte a través de la lista privada, se recomienda leerla a través de una cuenta de lector para identificar los trabajos con errores más rápidamente.

## Registrar un anuncio privado

Para registrar un anuncio privado, primero recopile los detalles de su cuenta de Snowflake y, a continuación, añada el anuncio en Workfront.

### Recopile los detalles de su cuenta de Snowflake

Workfront utiliza los detalles de su cuenta de Snowflake para dirigir el anuncio a su cuenta. Reúna los siguientes detalles:

* Localizador de cuentas
* URL de cuenta
* Organización de la cuenta
* Nombre de cuenta

Cada uno de estos valores está disponible en el modal Account Details de Snowflake.

Para encontrar los detalles de su cuenta:

1. Cuando haya iniciado sesión en su cuenta de Snowflake, haga clic en el menú de usuario en la esquina inferior izquierda.

1. Seleccione su cuenta en la sección **Cuenta** del menú.

1. Haga clic en **Ver detalles de la cuenta** para la cuenta.

1. Registre cada uno de los valores enumerados arriba.

Decida también el nombre de la base de datos a través de la cual desea acceder a los datos de Workfront vinculados. Este nombre se introduce al registrar el anuncio.

### Añadir el anuncio privado en Workfront

La lista privada se registra mediante la interfaz de Adobe Workfront.

>[!IMPORTANT]
>
>Solo puedes crear un anuncio privado por cada localizador de cuentas.

1. Haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront o (si está disponible), haga clic en el icono de **[!UICONTROL Menú principal]** ![Menú principal](/help/_includes/assets/main-menu-icon-left-nav.png) en la esquina superior izquierda y, a continuación, haga clic en **Configuración**.

1. En el panel izquierdo, haga clic en **Sistema** > **Conexión de datos**.

1. Haga clic en la ficha **conexiones de Snowflake**.

1. Haga clic en **Agregar listado privado**.

1. Complete el formulario con los detalles de la cuenta que ha recopilado, incluido el nombre de su base de datos preferido.

1. Haga clic en **Agregar listado privado**.

### Conectarse al listado en Snowflake

En su cuenta de Snowflake, establezca una conexión con el listado privado como fuente de datos externa. A continuación, puede consultar los datos de Workfront junto con el resto de los datos.

## Configuración de las vistas Historial actual y Historial diario

Una conexión de cuenta de lector proporciona tres vistas de datos para cada tabla de objetos:

* **Actual**: una representación de baja latencia de los datos tal como existe actualmente en la aplicación de origen.
* **Historial diario**: una representación de los datos tal como estaban a las 11:59 PM UTC de cada día.
* **Evento**: cada transacción de cambio enviada a las canalizaciones de datos de Data Connect.

Un anuncio privado solo comparte la vista de eventos. Esta sección proporciona SQL para crear las vistas Actual, Historial diario y Evento en su propia cuenta de Snowflake.

Todas las vistas de eventos incluidas en la lista tienen los campos necesarios para la lógica de vista que aparece a continuación. En estos ejemplos se supone que ha creado una nueva base de datos y esquema de su elección en la cuenta de Snowflake de destino y que utilizan la vista `projects_event`. En cada ejemplo, reemplace `<listing_db>` y `<listing_schema>` por sus propios valores.

>[!TIP]
>
>Le recomendamos que reemplace `select *` por una lista de las columnas que usa para su análisis. Si usa `select *` y las columnas se agregan posteriormente a la vista de eventos del listado, debe volver a crear la vista para habilitar las nuevas columnas.

### Vistas actuales

La Vista actual de un objeto es el último registro de evento de cambio almacenado en Data Connect. Si el último registro está en estado eliminado, el registro se omite de la vista Actual. Todas las vistas de eventos tienen la misma estructura.

```sql
create or replace view projects_current copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event
where end_effective_timestamp = '2300-01-01'::timestamp_ntz
 and nvl(deleted, 0) != 1;
```

Las columnas `deleted` y `end_effective_timestamp` no son necesarias en la vista Actual. La vista filtra los datos a un único valor y elimina el registro por completo si se elimina el registro.

### Vistas de historial diario

La vista Historial diario identifica el registro de evento de cambio que estaba activo a las 23:59:59 horas de una fecha determinada, de modo que puede analizar la tendencia del estado del registro a lo largo del tiempo. En el ejemplo siguiente se muestra el estado de un registro de proyecto al final de cada día del calendario.

```sql
create or replace view projects_daily_history copy grants
as
select d.calendardate as
 , p.*
from <listing_db>.<listing_schema>.calendar_dates d
join <listing_db>.<listing_schema>.projects_event p
 on p.begin_effective_timestamp <= d.calendareodtimestamp
and d.calendareodtimestamp < p.end_effective_timestamp
where d.calendareodtimestamp < current_date() - 1
 and nvl(deleted, 0) != 1;
```

### Vistas de eventos

Para mantener la coherencia, le recomendamos que cree una copia de la vista de evento a partir de la base de datos de listado y la coloque en el mismo esquema que las vistas Historial actual y Historial diario.

```sql
create or replace view projects_event copy grants
as
select *
from <listing_db>.<listing_schema>.projects_event;
```
