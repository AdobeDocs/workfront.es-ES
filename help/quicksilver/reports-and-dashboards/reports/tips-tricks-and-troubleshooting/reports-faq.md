---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Preguntas frecuentes sobre informes
description: Preguntas frecuentes sobre informes
author: Nolan
feature: Reports and Dashboards
exl-id: 5e267d45-7922-4c0f-8530-59a8c152f625
source-git-commit: 957c6e6955a828aa40ac996490d66e9c46f594bc
workflow-type: tm+mt
source-wordcount: '1510'
ht-degree: 87%

---

# Preguntas frecuentes sobre informes

<!--Audited: 05/2025-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is the ONE anchor article for all FAQs about Reporting. Add a new FAQ in the TOC at the top first, then add the answer as a section at the bottom.)</p>
-->

Las siguientes son las preguntas más frecuentes sobre los informes.

## Requisitos de acceso

+++ Amplíe para ver los requisitos de acceso.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td><p>Nuevo: estándar</p> 
   <p>Actual: Trabajo o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de Edición a informes, paneles y calendarios</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Permisos de administración para un informe</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## ¿Por qué mi cálculo personalizado para una diferencia horaria no muestra el resultado correcto en una columna?

<!--this section is linked from the Actual Hours article for Tasks in the Task Information folder; edit the links or do not delete or change this section-->

En un informe de proyecto tengo un cálculo que resta las horas reales de las planificadas.

El resultado que estoy obteniendo es incorrecto.

<!--this changed with this issue in May 2025; Actual Hours changed from actualWorkRequired to actualWorkRequiredDouble: https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/task/68108e860000120e90a79cb82e5811c2/updates : On a project report I have a calculation that subtracts Actual Hours (2) from Planned Hours (4). The result I am getting is 120 when it should be 2.  -->

Mi cálculo es:

`valueexpression=SUB(workRequired,actualWorkRequired)`

### Respuesta

La mayoría de los campos que utilizan horas en Workfront se almacenan en minutos. Cuando se utilizan estos campos en un cálculo, el resultado suele ser en minutos. Para obtener el resultado en horas, debe dividir el resultado del cálculo o del campo al que hace referencia por 60.

Las horas planificadas se almacenan en minutos.

En función del campo Horas reales que desee utilizar para el cálculo, las fórmulas correctas son:

* Para las horas reales heredadas que se almacenan en minutos:

  `valueexpression=SUB(workRequired,actualWorkRequired)/60`

* Para las horas reales que se almacenan en horas:

  `valueexpression=SUB(workRequired/60,actualWorkRequiredDouble)`

Para obtener más información, vea [Ver horas reales](/help/quicksilver/manage-work/tasks/task-information/actual-hours.md).

## ¿Por qué no se muestra en el gráfico el valor de cada uno de los elementos de mi gráfico en un informe?

### Respuesta

Si un gráfico de informe contiene más de 50 elementos, el valor de cada elemento no se mostrará en el gráfico.

Cuando un gráfico contiene menos de 50 elementos, el valor de cada elemento se mostrará en el gráfico. Considere la posibilidad de añadir un filtro o modificar las agrupaciones del informe para limitar la cantidad de elementos que se muestran en cada elemento del gráfico.

## ¿Por qué mi informe devuelve demasiados resultados para mostrar el gráfico?

Cuando ejecuto un informe que tiene un gráfico, aparece el mensaje de error “Vaya... Este informe ha devuelto MUCHOS datos, lo que hace que el gráfico sea ilegible. Considere la posibilidad de reducir los resultados añadiendo un filtro o cambiando las agrupaciones en el gráfico.”

### Respuesta

Este error significa que su gráfico contiene hasta 618 resultados distintos, por ejemplo, más de 618 barras en un gráfico de barras. Para resolver el problema de visualización, es necesario refinar los resultados modificando las selecciones actuales de filtros y agrupaciones.

Para obtener información sobre la modificación de filtros y agrupaciones, consulte los artículos [Descripción general de filtros](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md) y [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

## ¿Por qué veo mis tareas (o problemas) cuando accedo al mismo informe (o calendario) que mi compañero de trabajo y ellos ven sus tareas en su lugar?

### Respuesta

El informe o calendario puede tener una variable de filtro carácter comodín que apunte al usuario que ha iniciado sesión. En este caso, el informe muestra información basada en el usuario que ha iniciado sesión. Ajuste el filtro para eliminar el carácter comodín que apunta al usuario que ha iniciado sesión.\
![variable de filtro de ID de usuario](assets/qs--user.id-filter-variable-350x79.png)

Para obtener una lista completa de la información general sobre las variables de filtro de carácter comodín basadas en usuarios, consulte [Información general sobre las variables de filtro de carácter comodín](../../../reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

## ¿Por qué los datos de mi informe parecen incompletos?

### Respuesta

Esto puede ocurrir en la mayoría de los casos si tiene un acceso limitado que le impide ver los elementos del sistema. Además, no se ha compartido el uso de los elementos que desea ver.

El creador del informe puede editarlo para ejecutarlo con los derechos de acceso de un usuario con rol de administrador del sistema o cualquier usuario con Plan que tenga acceso para ver los datos.

Para obtener más información, consulte [Ejecutar y enviar un informe con los derechos de acceso de otro usuario](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md).

## ¿Cómo puedo informar sobre las tareas (o problemas) que se me han asignado, independientemente de si soy su propietario o no?

### Respuesta

Para ver todas las tareas o problemas que se le han asignado, tanto si es el propietario (o la persona asignada principal) como si no, utilice el siguiente filtro en un informe de tareas o problemas:

1. Acceda a un informe de tareas o problemas.
1. En la pestaña **Filtros**, haga clic en **Añadir una regla de filtro**.

1. En el campo **Empiece a escribir el nombre del campo…**, empiece a escribir el **nombre de los usuarios de la asignación** y, a continuación, selecciónelo cuando aparezca en la lista.

   >[!NOTE]
   >
   >No utilice el campo **Asignado al nombre**, ya que este filtro es solo para las tareas y problemas de los que se es el usuario principal asignado o propietario.

1. Seleccione el modificador **Igual**.
1. Empiece a escribir *$$USER.ID* en el cuadro de texto y selecciónelo en la lista desplegable que aparece.\
   Esto garantiza que se vean todas las tareas y problemas asignados al usuario que ha iniciado sesión. Puede sustituir el comodín por un nombre de usuario específico.\
   ![Tareas asignadas a mí](assets/qs-tasks-assigned-to-me-assignment-users-name-filter-350x63.png)

1. Haga clic en **Guardar + Cerrar**.

## ¿Por qué los vínculos Añadir problemas o Añadir tareas no aparecen en la parte inferior de mis listas de tareas y problemas de un proyecto?

### Respuesta

En primer lugar, asegúrese de que dispone del acceso y los permisos correctos para añadir problemas y tareas a un proyecto. Si es así, debería ver los vínculos **Añadir problemas** y **Añadir tareas** en la parte inferior de las listas **Problemas** y **Tareas**.

Sin embargo, determinados factores pueden impedir que se muestren estos vínculos:

* Si se ha aplicado el filtro rápido a estas listas, los vínculos no se mostrarán. Quite el filtro rápido y los vínculos se mostrarán para poder añadir problemas y tareas a los proyectos.\
  Para obtener información sobre el filtro rápido, consulte [Introducción a las listas en Adobe Workfront](../../../workfront-basics/navigate-workfront/use-lists/view-items-in-a-list.md).

* Si se ha aplicado una **agrupación** a estas listas, los vínculos no se mostrarán. Quite la **agrupación** y los vínculos se mostrarán para poder añadir problemas y tareas a los proyectos.\
  Para obtener información acerca de la creación de agrupaciones, consulte [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

* Si se ha aplicado una **vista** a estas listas, en la que se ha seleccionado una moneda distinta de la predeterminada para el proyecto, los vínculos no se mostrarán. Cambie la **vista** a **Moneda original del proyecto** y los vínculos se mostrarán para poder añadir problemas y tareas a los proyectos.\
  Para obtener más información sobre el cambio de moneda en la vista, consulte [Crear informes de datos financieros con tipos de cambio únicos](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-financial-data-reports-unique-exchange-rates.md).

![Divisa del proyecto](assets/nwe-project-original-currency-350x229.png)

## ¿La información de mi informe o panel se actualiza automáticamente?

### Respuesta

La información de los informes o paneles no se actualiza automáticamente.

La información se puede actualizar manualmente en un informe almacenado en caché.\
Para obtener más información sobre la actualización de un informe almacenado en caché, consulte [Ejecutar un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-report.md).

La información se puede actualizar manualmente en un panel almacenado en caché.\
Para obtener más información acerca de la actualización de un panel en caché, consulte la sección [Paneles de visualización](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md#running-dashboards) en el artículo [Introducción a los paneles](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## ¿Puedo cambiar el propietario de un informe?

### Respuesta

No se puede cambiar el propietario de un informe. Sin embargo, el usuario que ha creado el informe puede permitir que otros usuarios lo editen. La forma de permitir que los usuarios editen un informe depende del tipo de usuario.

* Los administradores del sistema pueden permitir que los usuarios con licencia Plan editen los informes configurando la opción Editar en la fila Informes para incluir el acceso a Crear un informe.\
  Para obtener más información, consulte [Conceder acceso a informes, paneles y calendarios](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md).

* Cualquier usuario final con acceso para crear y compartir informes puede permitir que otros editen informes individuales compartiéndolos y concediendo a otros usuarios permisos de administración.\
  Para obtener más información, consulte [Compartir un informe en Adobe Workfront](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md).

Si tiene permisos para ver o administrar un informe, también puede realizar una copia de este, de la que será el propietario de forma predeterminada. Para obtener más información sobre la copia de un informe, consulte [Crear una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

## ¿Por qué no puedo acceder a un informe de propiedad de un usuario desactivado?

### Respuesta

En ocasiones, el propietario del informe también es el usuario especificado en el campo **Ejecutar este informe con los derechos de acceso de:** del informe. Si el usuario **Ejecutar este informe con los derechos de acceso de:** está desactivado, el informe ya no se mostrará a los usuarios que hayan compartido el informe con ellos. Cuando esto suceda, puede volver a tener acceso al informe si deja en blanco **Ejecutar este informe con los derechos de acceso de:** o escribe un usuario activo en el campo.

Para obtener más información acerca del campo **Ejecutar este informe con los derechos de acceso de:**, consulte [Ejecutar y entregar un informe con los derechos de acceso de otro usuario](../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md). Para obtener información sobre cómo identificar todos los informes que pertenecen a usuarios desactivados, consulte [Crear un informe sobre las actividades de creación de informes](../../../reports-and-dashboards/reports/report-usage/create-report-reporting-activities.md).

## ¿Cómo puedo acceder a un panel que contiene un informe que pertenece a un usuario eliminado?

### Respuesta

Cuando elimine un usuario, aún podrá acceder a los informes que este haya creado; sin embargo, también se eliminarán los paneles que incluye el informe. Esto significa que ya no puede acceder a lo siguiente:

* Panel que contiene el informe
* Sección personalizada que contiene un panel del informe

Para obtener más información sobre las implicaciones de eliminar un usuario, consulte [Eliminar usuarios](../../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

Si tiene acceso de visualización del informe, puede hacer lo siguiente:

1. Crear una copia del informe.\
   Para aprender a crear una copia de un informe, vea [Crear una copia de un informe](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-copy-report.md).

1. Actualizar el panel para incluir el informe copiado.\
   Para obtener información sobre cómo editar un panel, consulte [Editar un panel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/edit-dashboard.md).
