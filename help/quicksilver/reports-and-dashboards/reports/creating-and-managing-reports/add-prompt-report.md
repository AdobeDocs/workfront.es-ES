---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Agregar solicitudes a un informe
description: Los filtros y las indicaciones son similares en el sentido de que ambos restringen la cantidad de información que se muestra en un informe.
author: Nolan
feature: Reports and Dashboards
exl-id: b4058fb3-7360-474f-8be1-1c6b584749b0
source-git-commit: ''
workflow-type: tm+mt
source-wordcount: '1252'
ht-degree: 0%

---

# Agregar solicitudes a un informe

## La diferencia entre mensajes y filtros

Los filtros y las indicaciones son similares en el sentido de que ambos restringen la cantidad de información que se muestra en un informe.

Se crea un filtro cuando se desea que la información mostrada en el informe se filtre con los mismos criterios cada vez que se ejecuta el informe. Los filtros se crean una vez y están codificados en el informe. Para obtener más información sobre la creación de filtros, consulte el artículo [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

Las solicitudes son filtros abiertos que se pueden personalizar y aplicar de forma diferente cada vez que se ejecuta un informe.

Cuando agregue mensajes al informe, puede personalizar la información de filtrado editando los criterios del mensaje cada vez que ejecute el informe. El informe se ejecuta con un filtro diferente cada vez, dependiendo de los modificadores que elija, en lugar de codificar los modificadores una vez en el filtro del informe.

Las solicitudes actúan como un filtro personalizable en los informes que se pueden actualizar justo antes de ejecutar el informe. Puede crear informes genéricos y luego reducir los resultados en función de la información que desee ver para ese día o de la información que sea relevante para un conjunto de criterios individuales. Por ejemplo, si tiene un informe de horas y desea cambiar la información del informe en función de los siguientes criterios:

* Fechas en las que se registraron las horas
* Los usuarios que entraron en las horas
* Cantidad de horas introducidas

Se crearían tres mensajes en los que las condiciones son los criterios necesarios y el informe tendría un aspecto diferente cada vez que se ejecute, según la información que se elija para las solicitudes.

Un filtro le puede indicar a Adobe Workfront que muestre solo esas horas introducidas entre junio y agosto de este año. Sin embargo, con una solicitud, puede utilizar un intervalo de tiempo diferente cada vez que ejecute el informe (por ejemplo, entre enero y febrero u octubre y diciembre).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Editar acceso a filtros, vistas y grupos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisitos previos

Debe crear un informe antes de poder agregarle una solicitud.

Para obtener instrucciones sobre cómo crear un informe, consulte [Crear un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-report.md)

## Crear una solicitud

1. Vaya al informe donde desee agregar una solicitud.
1. Expandir **Acciones de informe** y, a continuación, haga clic en **Editar**.

1. Haga clic en **Configuración de informes**.
1. En el **Mensajes del informe** área, haga clic en **Agregar un mensaje**.\
   ![](assets/qs-add-a-prompt-350x216.png)

1. (Condicional) Seleccione el campo en el que desea que se base la solicitud. Comience a escribir el nombre del campo y haga clic en para seleccionarlo cuando aparezca en la lista.\
   Las opciones disponibles para los usuarios que ejecuten el informe diferirán según el campo seleccionado.\
   Por ejemplo, si selecciona un campo de fecha como Fecha de finalización real en un informe de tarea, &quot;Fecha de finalización real&quot; es el nombre de la solicitud. Al editar este mensaje mientras ejecuta este informe, puede elegir entre un conjunto de modificadores para crear la instrucción de filtrado. Este proceso es idéntico al de la creación de un filtro. Para obtener más información sobre los modificadores, consulte [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. (Condicional) Haga clic en **Mensaje personalizado** para crear un mensaje personalizado.

   Una solicitud personalizada es una solicitud predefinida en la que incrusta el código de los criterios de filtrado antes de ejecutar el informe. En este sentido, un mensaje personalizado está más cerca de un filtro que un mensaje.

   Sin embargo, el mensaje sigue siendo tan flexible como un mensaje normal porque puede elegir entre varias instrucciones predefinidas, en lugar de tener un filtro predefinido en el informe.

   Especifique la siguiente información para el mensaje personalizado: La condición de una solicitud personalizada solo se puede editar mediante el modo de texto. Esto permite aplicar varias condiciones en un solo campo.

   * **Nombre del campo:** Este es el nombre de la solicitud, tal como lo ve antes de ejecutar el informe.
   * **Etiqueta:** Este es el nombre de una de las opciones dentro de la solicitud, tal como lo ve antes de ejecutar el informe.
   * **Condición:** Introduzca una condición que defina la solicitud.

   Utilice la misma sintaxis que usaría al introducir un filtro de modo de texto y una las instrucciones mediante &quot;&amp;&quot;. Para obtener más información sobre la edición de un filtro en el modo de texto, consulte [Edición de un filtro mediante el modo de texto](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md).

   Por ejemplo, la variable **Condición** del indicador personalizado para las siguientes situaciones podría tener este aspecto:

   * todas las tareas de futuros proyectos en los que el estado del proyecto sea Idea, Solicitado, Planificado y Actual:

      ```
      project:plannedStartDate=$$TODAY&project:plannedStartDate_Mod=gte&project:status=IDA,REQ,PLN,CUR&project:status_Mod=in
      ```

   * todas las tareas en proyectos completados (anteriores) en los que el estado del proyecto está completado o muerto:

      ```
      project:actualCompletionDate=$$TODAY&project:actualCompletionDate_Mod=lte&project:status=CPL,DED&project:status_Mod=in
      ```
   Para obtener más información sobre los modificadores de modo de texto, consulte [Modificadores de filtro y condición](../../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

   >[!NOTE]
   >
   >Al ejecutar el informe, no se pueden cambiar las condiciones de un mensaje personalizado, como lo haría con un mensaje estándar. Puede tener tantas condiciones predefinidas para un mensaje personalizado como necesite.

1. (Opcional) Repita los pasos 4 o 5 para crear tantos mensajes como sea necesario.
1. Haga clic en **Listo** y haga clic en **Guardar y cerrar** para guardar el informe.

## Aplicar una solicitud a un informe

Cuando se añade una solicitud a un informe, la pestaña predeterminada del informe es siempre la ficha Mensajes .

Para ejecutar un informe con una solicitud de confirmación:

1. Vaya al informe con el mensaje .

   ![](assets/qs-prompt-drop-downs-350x229.png)

1. Seleccione una condición para una o todas las indicaciones que se muestran en la **Mensajes** pestaña .\
   (Opcional) Puede dejar los mensajes en blanco y no filtrar el informe según las condiciones del mensaje.

1. Haga clic en **Ejecutar informe**.\
   (Condicional) Si rellena los mensajes, el informe se filtrará según las condiciones que haya elegido para los mensajes.\
   (Condicional) Si deja las indicaciones en blanco, el informe no se filtra con las condiciones del mensaje. El informe se muestra como si no se hubiera filtrado.

   >[!NOTE]
   >
   >Un informe que contiene un filtro además de una solicitud filtra los resultados según los criterios definidos en el filtro y la solicitud combinada.

## Limitaciones en el uso compartido de los informes solicitados

>[!CAUTION]
>
>Cuando comparte un informe solicitado fuera de Workfront, el usuario que esté viendo el informe debe iniciar sesión en Workfront para ejecutar el informe con la solicitud. Si el usuario que está viendo el informe no ha iniciado sesión, todos los resultados del informe se mostrarán sin aplicar la solicitud.

A continuación se indican las limitaciones para compartir informes solicitados desde Workfront:

* Cuando comparte un informe públicamente, los usuarios no pueden ejecutar el informe aplicando la solicitud, a menos que tengan credenciales de Workfront e inicien sesión primero para ver el informe en Workfront.

   Para obtener más información sobre cómo compartir informes, consulte el artículo [Compartir un informe en Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).
* Cuando se programa un informe solicitado para su envío, el informe incluido en el adjunto de correo electrónico incluye los datos del informe que se solicita. Cuando el usuario hace clic en el vínculo del correo electrónico para acceder al informe, primero debe iniciar sesión para ver el informe y ejecutar el mensaje por su cuenta.

   Para obtener información sobre cómo programar un informe enviado, consulte [Programar un envío automático de informes](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-automatic-report-delivery.md).
