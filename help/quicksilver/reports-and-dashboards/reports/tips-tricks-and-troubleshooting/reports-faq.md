---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Preguntas más frecuentes sobre los informes
description: Preguntas más frecuentes sobre los informes
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1502'
ht-degree: 0%

---

# Preguntas más frecuentes sobre los informes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

A continuación se presentan las preguntas más frecuentes sobre los informes.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar, Trabajar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## ¿Por qué mi cálculo personalizado para una diferencia de hora no muestra el resultado correcto en una columna?

En un informe de proyecto tengo un cálculo que resta las horas reales (2) del horario planificado (4). El resultado que obtengo es 120 cuando debería ser 2.\
Mi cálculo es:
<pre>valueexpression=SUB(workRequired,realWorkRequired)</pre>

### Respuesta

Los campos que utilizan horas en Workfront se almacenan en minutos. Al utilizar el campo en un cálculo, el resultado será en minutos. Para obtener el resultado en horas, debe dividir el resultado del cálculo en 60.

El cálculo correcto es:

<pre>valueexpression=SUB(workRequired,realWorkRequired)/60</pre>

## ¿Por qué el valor de cada uno de los elementos de gráfico de un informe no se muestra en el gráfico?

### Respuesta

Si hay más de 50 elementos de gráfico en un gráfico de informes, el valor de cada elemento no se muestra en el gráfico.

Cuando hay menos de 50 elementos en un gráfico, el valor de cada elemento se muestra en el gráfico. Considere la posibilidad de agregar un filtro o modificar las agrupaciones en el informe para limitar la cantidad de elementos que se muestran en cada elemento del gráfico.

## ¿Por qué mi informe devuelve demasiados resultados para mostrar el gráfico?

Cuando ejecuto un informe que tiene un gráfico, veo el mensaje de error &quot;¡Guau!... Este informe devolvió MUCHOS datos que hacen que el gráfico sea ilegible. Considere reducir los resultados agregando un filtro o cambiando las agrupaciones en el gráfico&quot;.

### Respuesta

Este error significa que el gráfico contiene hasta 618 resultados diferentes, por ejemplo, más de 618 barras en un gráfico de barras. Para resolver el problema de visualización, debe refinar los resultados modificando el filtro actual y agrupando las selecciones.

Para obtener información sobre la modificación de filtros y agrupaciones, consulte los artículos [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) y [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## ¿Por qué veo mis tareas (o problemas) cuando accedo al mismo informe (o calendario) que mi compañero y ellos ven sus tareas en su lugar?

### Respuesta

El informe o el calendario pueden tener una variable de filtro comodín que apunte al usuario que ha iniciado sesión. En este caso, el informe muestra la información en función del usuario que ha iniciado sesión. Ajuste el filtro para eliminar el comodín que señala al usuario que ha iniciado sesión.\
![](assets/qs--user.id-filter-variable-350x79.png)

Para obtener una lista completa de las variables de filtro comodín basadas en el usuario, consulte [Variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## ¿Por qué los datos de mi informe parecen incompletos?

### Respuesta

Esto puede suceder en la mayoría de los casos si tiene un acceso limitado que impide que vea elementos en el sistema. Además, los elementos que desea ver no se comparten con usted.

El creador del informe puede editar el informe para ejecutarlo con los derechos de acceso de un administrador del sistema o de cualquier usuario de Plan que tenga acceso a ellos.

Para obtener más información, consulte [Ejecutar y enviar un informe con los derechos de acceso de otro usuario](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## ¿Cómo informo sobre las tareas (o problemas) que tengo asignadas, independientemente de si soy el propietario de ellas o no?

### Respuesta

Para ver todas las tareas o problemas que se le han asignado, ya sea propietario (o usuario asignado principal) o no, utilice el siguiente filtro en un informe de problemas o tareas:

1. Acceda a un informe de tareas o problemas.
1. En el **Filtros** , haga clic en **Agregar una regla de filtro**.

1. En el **Empiece a escribir el nombre del campo...** campo, empezar a escribir **Nombre de usuarios de asignación** y, a continuación, selecciónela cuando aparezca en la lista.

   >[!NOTE]
   >
   >No use el **Asignado a nombre** , ya que esto solo filtra las tareas y los problemas para los que es el usuario asignado principal o el propietario.

1. Seleccione el **Igual** modificador.
1. Empezar a escribir *$$USER.ID* en el cuadro de texto y selecciónelo en la lista desplegable que aparece.\
   Esto garantiza que vea todas las tareas y problemas asignados al usuario que ha iniciado sesión. Puede reemplazar el comodín por un nombre de usuario específico.\
   ![](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Haga clic en **Guardar + Cerrar**.

## ¿Por qué los vínculos Agregar problemas/Agregar tareas no aparecen en la parte inferior de mis listas Problemas y Tareas en un proyecto?

### Respuesta

En primer lugar, asegúrese de que tiene el acceso y los permisos correctos para agregar problemas y tareas a un proyecto. En este caso, debería ver la variable **Agregar problemas** y **Agregar tareas** vínculos en la parte inferior del **Problemas** y **Tareas** listas.

Sin embargo, hay algunas cosas que pueden impedir que se muestren estos vínculos:

* Si ha aplicado el filtro rápido a estas listas, los vínculos no se muestran. Elimine el filtro rápido y se mostrarán los vínculos para que pueda añadir problemas y tareas a sus proyectos.\
   Para obtener información sobre el filtro rápido, consulte [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Si tiene una **Agrupación** aplicados a estas listas, los vínculos no se muestran. Elimine el **Agrupación** y los vínculos deben mostrarse para que pueda añadir problemas y tareas a sus proyectos.\
   Para obtener información sobre la creación de agrupaciones, consulte [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Si tiene una **Ver** aplicados a estas listas que tienen una moneda seleccionada que no sea la moneda predeterminada para el proyecto, no se muestran los vínculos. Cambie el **Ver** a **Moneda original del proyecto** y los vínculos deben mostrarse para que pueda añadir problemas y tareas a sus proyectos.\
   Para obtener más información sobre cómo cambiar la moneda en la vista, consulte [Crear informes de datos financieros con tipos de cambio únicos](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![](assets/nwe-project-original-currency-350x229.png)

## ¿La información de mi informe o panel se actualiza automáticamente?

### Respuesta

La información de los informes o los tableros no se actualiza automáticamente.

La información se puede actualizar manualmente en un informe en caché.\
Para obtener más información sobre cómo actualizar un informe en caché, consulte [Ejecutar un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

La información se puede actualizar manualmente en un tablero en caché.\
Para obtener más información sobre la actualización de un tablero en caché, consulte la sección [Mostrar tableros](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) en el artículo [Introducción a los paneles](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## ¿Puedo cambiar el propietario de un informe?

### Respuesta

No se puede cambiar el propietario de un informe. Sin embargo, el usuario que creó el informe puede permitir que otros usuarios lo editen. La forma de permitir que los usuarios editen un informe depende del tipo de usuario que sea.

* Los administradores del sistema pueden permitir que los usuarios con una licencia de Plan editen los informes configurando la opción Editar en la fila Informes para incluir el acceso a Crear un informe.\
   Para obtener más información, consulte [Conceder acceso a informes, tableros y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Cualquier usuario final con acceso para crear y compartir informes puede permitir que otros editen informes individuales al compartirlos y otorgarles permisos de administración.\
   Para obtener más información, consulte [Compartir un informe en Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Si tiene permisos para ver o administrar un informe, también puede realizar una copia del informe, que será el propietario de forma predeterminada. Para obtener más información sobre cómo copiar un informe, consulte [Creación de una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## ¿Por qué no puedo acceder a un informe propiedad de un usuario desactivado?

### Respuesta

A veces, el propietario del informe también es el usuario especificado en la variable **Ejecute este informe con los derechos de acceso de:** en el informe. Si la variable **Ejecute este informe con los derechos de acceso de:** está desactivado, el informe ya no se muestra para los usuarios que han compartido el informe con ellos. Cuando esto sucede, puede hacer que el informe vuelva a ser accesible si deja la variable **Ejecute este informe con los derechos de acceso de:** en blanco o al introducir un usuario activo en el campo .

Para obtener más información sobre **Ejecute este informe con los derechos de acceso de:** campo, consulte [Ejecutar y enviar un informe con los derechos de acceso de otro usuario](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Para obtener información sobre la identificación de todos los informes que son propiedad de usuarios desactivados, consulte [Crear un informe sobre las actividades de informes](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## ¿Cómo puedo acceder a un tablero que contiene un informe propiedad de un usuario eliminado?

### Respuesta

Al eliminar un usuario, aún puede acceder a cualquier informe que haya creado; sin embargo, cualquier tablero que incluya el informe también se eliminará. Esto significa que ya no puede acceder a lo siguiente:

* Un tablero que contiene el informe
* Sección personalizada que contiene un tablero del informe

Para obtener más información sobre las implicaciones de la eliminación de un usuario, consulte [Eliminar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Si tiene acceso de vista al informe, puede hacer lo siguiente:

1. Cree una copia del informe.\
   Para obtener información sobre cómo crear una copia de un informe, consulte [Creación de una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Actualice el tablero para incluir el informe copiado.\
   Para obtener información sobre cómo editar un tablero, consulte [Editar un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
