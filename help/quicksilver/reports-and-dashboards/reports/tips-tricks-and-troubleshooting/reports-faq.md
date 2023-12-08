---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Preguntas frecuentes sobre informes
description: Preguntas frecuentes sobre informes
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: d8e3c2da7f8fcd062e1bf2bb5de43a6238f5eadd
workflow-type: tm+mt
source-wordcount: '1512'
ht-degree: 0%

---

# Preguntas frecuentes sobre informes

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

Las siguientes son las preguntas más frecuentes sobre los informes.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Planificar, Trabajo</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a informes, tableros y calendarios</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## ¿Por qué el cálculo personalizado de una diferencia de hora no muestra el resultado correcto en una columna?

En un informe de proyecto tengo un cálculo que resta las horas reales (2) de las horas planificadas (4). El resultado que estoy obteniendo es 120 cuando debería ser 2.\
Mi cálculo es:
<pre>valueexpression=SUB(workRequired,actualWorkRequired)</pre>

### Respuesta

Los campos que utilizan horas en Workfront se almacenan en minutos. Al utilizar el campo en un cálculo, el resultado se expresa en minutos. Para obtener el resultado en horas, debe dividir el resultado del cálculo entre 60.

El cálculo correcto es:

<pre>valueexpression=SUB(workRequired,actualWorkRequired)/60</pre>

## ¿Por qué el valor de cada uno de mis elementos de gráfico en un informe no se muestra en el gráfico?

### Respuesta

Si un gráfico contiene más de 50 elementos de gráfico, el valor de cada uno de ellos no se muestra en el gráfico.

Cuando un gráfico contiene menos de 50 elementos, el valor de cada uno de ellos se muestra en el gráfico. Considere la posibilidad de añadir un filtro o modificar las agrupaciones del informe para limitar la cantidad de elementos que se muestran en cada elemento del gráfico.

## ¿Por qué el informe devuelve demasiados resultados para mostrar el gráfico?

Cuando ejecuto un informe que tiene un gráfico, veo el mensaje de error &quot;Vaya... Este informe devolvió MUCHOS datos que hacen que el gráfico sea ilegible. Considere la posibilidad de reducir los resultados añadiendo un filtro o cambiando las agrupaciones en el gráfico&quot;.

### Respuesta

Este error significa que el gráfico contiene hasta 618 resultados distintos; por ejemplo, más de 618 barras en un gráfico de barras. Para resolver el problema de visualización, debe refinar los resultados modificando las selecciones de filtro y agrupación actuales.

Para obtener información sobre la modificación de filtros y agrupaciones, consulte los artículos [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) y [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## ¿Por qué veo mis tareas (o problemas) cuando accedo al mismo informe (o calendario) que mi compañero y ven sus tareas en su lugar?

### Respuesta

El informe o el calendario pueden tener una variable de filtro comodín que señala al usuario que ha iniciado sesión. En este caso, el informe muestra la información en función del usuario que ha iniciado sesión. Ajuste el filtro para quitar el comodín que señala al usuario que ha iniciado sesión.\
![](assets/qs--user.id-filter-variable-350x79.png)

Para obtener una lista completa de la información general sobre las variables de filtro comodín basadas en usuarios, consulte [Resumen de variables de filtro comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## ¿Por qué los datos de mi informe parecen incompletos?

### Respuesta

Esto puede suceder en la mayoría de los casos si tiene un acceso limitado que le impide ver los elementos en el sistema. Además, los elementos que desea ver no se han compartido con usted.

El creador del informe puede editarlo para ejecutarlo con los derechos de acceso de un administrador del sistema o cualquier usuario de Plan que tenga acceso para ver los datos.

Para obtener más información, consulte [Ejecutar y entregar un informe con los derechos de acceso de otro usuario](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## ¿Cómo puedo informar sobre las tareas (o problemas) a las que estoy asignado, independientemente de si soy el propietario de las mismas o no?

### Respuesta

Para ver todas las tareas o problemas que se le han asignado, tanto si es el propietario (o la persona asignada principal) como si no, utilice el siguiente filtro en un informe de tareas o problemas:

1. Acceder a un informe de tarea o problema.
1. En el **Filtros** pestaña, haga clic en **Agregar una regla de filtro**.

1. En el **Empiece a escribir el nombre del campo...** campo, empiece a escribir **Nombre de usuarios de asignación**, luego selecciónelo cuando aparezca en la lista.

   >[!NOTE]
   >
   >No use el **Asignado a nombre** , ya que filtra únicamente las tareas y problemas para los que es el principal asignado o propietario.

1. Seleccione el **Igual** modificador.
1. Empiece a escribir *$$USER.ID* en el cuadro de texto y selecciónelo en la lista desplegable que aparece.\
   Esto garantiza que verá todas las tareas y problemas asignados al usuario que ha iniciado sesión. Puede reemplazar el comodín por un nombre de usuario específico.\
   ![](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Haga clic en **Guardar + Cerrar**.

## ¿Por qué los vínculos Agregar problemas o Agregar tareas no aparecen en la parte inferior de mis listas de problemas y tareas de un proyecto?

### Respuesta

En primer lugar, asegúrese de que dispone del acceso y los permisos correctos para agregar problemas y tareas a un proyecto. En este caso, debería ver la variable **Agregar problemas** y **Agregar tareas** vínculos en la parte inferior de **Problemas** y **Tareas** listas.

Sin embargo, hay algunas cosas que pueden impedir que se muestren estos vínculos:

* Si tiene el filtro rápido aplicado a estas listas, los vínculos no se muestran. Elimine el filtro rápido y los vínculos deberían mostrarse para que pueda agregar problemas y tareas a sus proyectos.\
  Para obtener información sobre el filtro rápido, consulte [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Si tiene un **Agrupación** aplicados a estas listas, los vínculos no se muestran. Retire el **Agrupación** y los vínculos deberían mostrarse para que pueda agregar problemas y tareas a sus proyectos.\
  Para obtener información sobre la creación de agrupaciones, consulte [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Si tiene un **Ver** Si se aplican a estas listas que tienen seleccionada una moneda distinta de la predeterminada para el proyecto, los vínculos no se muestran. Cambie el **Ver** hasta **Divisa original del proyecto** y los vínculos deberían mostrarse para que pueda agregar problemas y tareas a sus proyectos.\
  Para obtener más información sobre cómo cambiar la divisa en la vista, consulte [Crear informes de datos financieros con tasas de cambio únicas](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![](assets/nwe-project-original-currency-350x229.png)

## ¿La información de mi informe o panel se actualiza automáticamente?

### Respuesta

La información de los informes o paneles no se actualiza automáticamente.

La información se puede actualizar manualmente en un informe almacenado en caché.\
Para obtener más información sobre la actualización de un informe almacenado en caché, consulte [Ejecutar un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

La información se puede actualizar manualmente en un panel almacenado en caché.\
Para obtener más información sobre cómo actualizar un panel en caché, consulte la sección [Mostrar paneles](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) en el artículo [Introducción a los paneles](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## ¿Puedo cambiar el propietario de un informe?

### Respuesta

No puede cambiar el propietario de un informe. Sin embargo, el usuario que creó el informe puede permitir que otros usuarios lo editen. La forma de permitir que los usuarios editen un informe depende del tipo de usuario que sea.

* Los administradores del sistema pueden permitir que los usuarios con una licencia de planificación editen los informes configurando la opción Editar en la fila Informes para incluir el acceso a Crear un informe.\
  Para obtener más información, consulte [Conceder acceso a informes, tableros y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Cualquier usuario final con acceso para crear y compartir informes puede permitir que otros editen informes individuales compartiéndolos y concediendo a otros usuarios permisos de administración.\
  Para obtener más información, consulte [Uso compartido de informes en Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Si tiene permisos para ver o administrar un informe, también puede realizar una copia del informe, de la que será el propietario de forma predeterminada. Para obtener más información sobre cómo copiar un informe, consulte [Creación de una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## ¿Por qué no puedo acceder a un informe propiedad de un usuario desactivado?

### Respuesta

En ocasiones, el propietario del informe es también el usuario especificado en la variable **Ejecutar este informe con los derechos de acceso de:** en el informe. Si la variable **Ejecutar este informe con los derechos de acceso de:** Cuando se desactiva el usuario, el informe ya no se muestra a los usuarios que han compartido el informe con ellos. Si esto sucede, puede volver a tener acceso al informe saliendo de la **Ejecutar este informe con los derechos de acceso de:** en blanco o introduciendo un usuario activo en el campo.

Para obtener más información sobre **Ejecutar este informe con los derechos de acceso de:** campo, consulte [Ejecutar y entregar un informe con los derechos de acceso de otro usuario](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Para obtener información sobre cómo identificar todos los informes propiedad de usuarios desactivados, consulte [Creación de un informe sobre las actividades de creación de informes](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## ¿Cómo puedo acceder a un tablero que contiene un informe propiedad de un usuario eliminado?

### Respuesta

Cuando elimine un usuario, aún podrá acceder a los informes que haya creado; sin embargo, también se eliminarán los tableros que incluyeran el informe. Esto significa que ya no puede acceder a lo siguiente:

* Panel que contiene el informe
* Sección personalizada que contiene un tablero del informe

Para obtener más información sobre las implicaciones de eliminar un usuario, consulte [Eliminar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Si tiene acceso de visualización al informe, puede hacer lo siguiente:

1. Cree una copia del informe.\
   Para obtener información sobre cómo crear una copia de un informe, consulte [Creación de una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Actualice el tablero para incluir el informe copiado.\
   Para obtener información sobre cómo editar un tablero, consulte [Edición de un tablero](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
