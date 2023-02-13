---
product-area: reporting
navigation-topic: text-mode-reporting
title: Creación de filtros complejos de modo de texto utilizando instrucciones EXISTS
description: Creación de filtros complejos de modo de texto utilizando instrucciones EXISTS
author: Nolan
feature: Reports and Dashboards
exl-id: 106f7c9d-46cc-46c5-ae34-93fd13a36c14
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '2803'
ht-degree: 0%

---

# Creación de filtros complejos de modo de texto utilizando instrucciones EXISTS

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: do not EVER&nbsp;delete this article as long as Text Mode still exists in the system.&nbsp;Google ordered this article to be written and we wrote it with the help of consultants, so the use case is very complex and very hard to understand without this. It is also very much used by many customers)</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;Alina: **~ Replace screen shot of icons when list/ reporting UI changes)</p>
-->

>[!IMPORTANT]
>
>Este artículo requiere una comprensión exhaustiva de la API de Adobe Workfront y de la interfaz de informes en modo de texto. Para obtener información sobre la API de Workfront, consulte [Conceptos básicos de API](../../../wf-api/general/api-basics.md).\
>Para obtener información sobre el uso del modo de texto, consulte [Información general sobre el modo de texto](../../../reports-and-dashboards/reports/text-mode/understand-text-mode.md).

## Descripción general de las relaciones de objetos en Workfront

Todos los objetos están vinculados a otros objetos de la base de datos de Workfront.

Comprender la jerarquía y la interdependencia de los objetos le ayuda a averiguar a qué objetos se puede hacer referencia en los informes.

Para obtener información sobre los objetos que se encuentran en Workfront y sobre su jerarquía y su interdependencia, consulte [Explicación de los objetos en Adobe Workfront](../../../workfront-basics/navigate-workfront/workfront-navigation/understand-objects.md).

Al crear filtros, puede hacer referencia a otros objetos que están conectados al objeto del filtro en un máximo de 2 niveles de relación mediante la interfaz de informes estándar.

Por ejemplo, puede hacer referencia al ID de Portfolio en un filtro de problemas para mostrar solo los problemas de los proyectos asociados a un portafolio determinado mediante la interfaz estándar. En este caso, el portafolio está a dos niveles de distancia de los problemas.

Sin embargo, no puede hacer referencia al propietario del Portfolio en un filtro de problemas usando la interfaz estándar para mostrar solo los problemas de los proyectos asociados con portafolios en los que el propietario es un usuario específico. Debe utilizar el modo de texto para acceder al campo Nombre del propietario del Portfolio, que está a tres niveles de los problemas.

![issue_to_portafolio_owner_right_line_icon.PNG](assets/issue-to-portfolio-owner-sraight-line-icons-350x83.png)

Para obtener una lista completa de los objetos de Workfront, consulte la [Explorador de API](../../../wf-api/general/api-explorer.md).

Para obtener información sobre cómo navegar por el Explorador de API y buscar objetos, consulte [Uso del Explorador de API](../../../wf-api/general/using-api-explorer.md).

Al crear filtros, se deben generar instrucciones complejas en la interfaz de modo de texto para hacer referencia a estos tipos de objetos.

Para obtener información sobre la creación de filtros complejos, consulte la [Descripción general de los filtros complejos de modo de texto que utilizan instrucciones EXISTS](#overview-of-complex-text-mode-filters-that-use-exists-statements) para obtener más información.

## Descripción general de los filtros de modo de texto complejos que utilizan instrucciones EXISTS {#overview-of-complex-text-mode-filters-that-use-exists-statements}

Tenga en cuenta lo siguiente cuando cree filtros que abarquen varios niveles en la jerarquía de objetos o filtre si faltan objetos:

* Debe crear filtros complejos cuando desee hacer referencia a objetos que no estén conectados directamente al objeto de filtro.
* Debe utilizar una instrucción EXISTS para hacer lo siguiente:

   * Cree filtros que abarquen varios niveles.
   * Cree filtros que busquen objetos que faltan.\
      Por ejemplo, al crear un informe de usuario, puede filtrar por usuarios que no hayan registrado la hora durante un período de tiempo determinado.

Tenga en cuenta las siguientes reglas al utilizar las instrucciones EXISTS en un filtro:

* Hay tres objetos a los que puede hacer referencia en un filtro EXISTENTE:

   * El objeto del filtro (objeto original).
   * El objeto cuyo campo desea hacer referencia (objeto de destino).
   * El objeto que conecta los objetos originales y de destino, en caso de que no estén directamente conectados entre sí (objeto de vinculación).

* Los filtros que utilizan EXISTS contienen dos instrucciones independientes vinculadas por un signo igual:

   * La instrucción antes del signo igual hace referencia al objeto al que hace referencia (la vinculación o el objeto de destino).
   * La instrucción que aparece después del signo igual hace referencia al objeto desde el que hace referencia (el objeto original).

* Debe utilizar el código de objeto del objeto de vinculación para conectar las instrucciones.\
   Puede encontrar el código de objeto de todos los objetos en el Explorador de API.\
   Para obtener información sobre el Explorador de API, consulte la [Explorador de API](https://one.workfront.com/s/api-explorer).

* Si falta un objeto de vinculación porque el objeto original y el objeto de destino están conectados entre sí directamente, puede utilizar el código de objeto del objeto de destino en lugar del objeto de vinculación.
* Puede hacer referencia a varios campos (campos de destino) en el mismo objeto (objeto de destino), en cuyo caso debe conectar las líneas que hacen referencia a los campos mediante AND.\
   Para ver un ejemplo del filtrado de más de un campo que pertenece al objeto de destino, consulte la [Ejemplo 4: Filtrar por varios campos: tareas por nombre de propietario del Portfolio y por ID de informe de valoración de alineación del Portfolio](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id) en este artículo.

* El único modificador admitido para una instrucción EXISTS es NOTEXISTS.

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
   <td> <p>Editar acceso a filtros, vistas y grupos</p> <p>Editar acceso a informes, tableros y calendarios para editar filtros en un informe</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administrar permisos en un informe para editar filtros en un informe</p> <p>Administrar permisos en un filtro para editarlo</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear filtros de modo de texto complejos que abarquen varios niveles en la jerarquía de objetos

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***[This information is somewhat duplicated from the section below: Create Text-Mode Filters for Missing Objects])</p>
-->

Puede crear un filtro que haga referencia a objetos en varios niveles de la jerarquía de objetos en la que existe el objeto de filtro. Por ejemplo, puede crear un filtro de problemas para los problemas que se producen en proyectos que no están asociados a un determinado propietario del Portfolio.

Siempre debe utilizar una instrucción EXISTS y la interfaz de modo de texto para crear este filtro.

Para ver ejemplos de filtros, consulte la [Ejemplo 1: Filtrar por problemas por nombre de propietario del Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) en este artículo.

Para crear un filtro que abarque varios niveles en la jerarquía de objetos:

1. Identifique el objeto del filtro. Nos referimos a este objeto como el objeto original.\
   Por ejemplo, Problema.
1. Identifique el campo por el que desea filtrar. Este objeto se denomina Campo de destino que pertenece a un objeto de destino.\
   Por ejemplo, el campo ownerID (campo de destino) que pertenece al Portfolio (objeto de destino).
1. (Condicional) Si el Objeto original (Problema) y el Campo de destino (ID de propietario) no están conectados directamente entre sí, debe encontrar un tercer objeto, un Objeto de vinculación (Proyecto) que los conecte. El objeto Vinculación debe tener al menos un campo al que se haga referencia desde las fichas Campos o Referencias del objeto original (el campo Vinculación se muestra en el objeto original) y también debe tener un campo Vinculación al objeto de destino que se muestra en las fichas Campos o Referencias del objeto Vinculación. El campo Vinculación al objeto de destino que se muestra en el objeto Vinculación (o el campo Vinculación mostrado en el objeto Vinculación) debe coincidir con el campo de destino.\
   Por ejemplo, se hace referencia al ID (proyecto) (campo de vinculación mostrado en el objeto original) desde Problemas (objeto original). (Portfolio) ownerID (Enlace de campo al objeto de destino) se muestra en la ficha Campos del proyecto (Vinculación de objeto). Portfolio ownerID también es un campo del objeto de destino (Portfolio). El campo Vinculación del objeto Vinculación coincide con el campo de Destino.\
   ![portafolio_id_en_el_proyecto_api_object.PNG](assets/portfolio-id-in-the-project-api-object-350x88.png)

1. Con el Explorador de API, identifique la variable **Código de objeto** del objeto de vinculación (proyecto).\
   Por ejemplo, el código de objeto para proyecto es PROJ.\
   ![project_objCode_in_the_API.PNG](assets/project-objcode-in-the-api-350x84.png)

1. Cree un filtro para el objeto original.\
   Por ejemplo, cree un filtro Problema .\
   Para obtener información sobre la creación de filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Haga clic en **Cambiar al modo de texto**.
1. Pegue el siguiente ejemplo de fórmula en la interfaz de modo de texto del nuevo filtro y reemplace el texto sugerido con los objetos y campos correctos:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object>
   EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

   Para ver un ejemplo utilizando los campos identificados anteriormente, consulte la [Ejemplo 1: Filtrar por problemas por nombre de propietario del Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name) en este artículo.

1. Haga clic en **Guardar filtro**.

## Creación de filtros de modo de texto complejos para objetos que faltan

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: **^[This information is somewhat duplicated from the section above: Create Text-Mode Filters that Span Multiple Levels in the Object Hierarchy])</p>
-->

Puede crear un filtro que haga referencia a los objetos que faltan. Por ejemplo, puede crear un filtro de usuario que muestre qué usuarios no han registrado horas en Workfront.

Siempre debe usar un *EXISTE* y la interfaz de modo de texto para crear este filtro.

Para ver ejemplos de filtros para objetos que faltan, consulte las siguientes secciones en este artículo:

* [Ejemplo 2: Filtre para los objetos que faltan: campos personalizados que no aparecen en ningún formulario personalizado](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Ejemplo 3: Filtre para los objetos que faltan: usuarios que no hayan registrado la hora durante un determinado período de tiempo](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)

Para crear un filtro que haga referencia a objetos que faltan:

1. Identifique el objeto del filtro. Nos referimos a este objeto como el objeto original.\
   Por ejemplo, Parámetro o Campo personalizado.
1. Identifique el campo por el que desea filtrar. Este objeto se denomina Campo de destino que pertenece a un objeto de destino.\
   Por ejemplo, el campo categoryID (campo de destino) que pertenece a Category (objeto de destino).
1. Dado que el objeto original (Parámetro) y el campo de destino (categoryID) no están conectados directamente entre sí, debe encontrar un tercer objeto, un objeto de vinculación (un parámetro de categoría) que los conecte. El objeto Vinculación debe tener al menos un campo al que se haga referencia desde las fichas Campos o Referencias del objeto original (el campo Vinculación se muestra en el objeto original) y también debe tener un campo Vinculación al objeto de destino que se muestra en las fichas Campos o Referencias del objeto Vinculación. El campo Vinculación al objeto de destino que se muestra en el objeto Vinculación (o el campo Vinculación mostrado en el objeto Vinculación) debe coincidir con el campo de destino.\
   Por ejemplo, se hace referencia al ID del parámetro de categoría (campo de vinculación mostrado en el objeto original) desde Parameter(Original Object). parameterID (Link Field to the Target Object) se muestra en la ficha Campos del Parámetro de categoría (objeto de vinculación). El campo Vinculación al objeto de destino que se muestra en el objeto Vinculación coincide con el campo de destino.
1. Con el Explorador de API, identifique la variable **Código de objeto** del objeto de vinculación (parámetro de categoría).\
   Por ejemplo, el código de objeto del parámetro de categoría es CTGYPA.\
   ![category_parameter_objcode_in_api.PNG](assets/category-parameter-objcode-in-api-350x79.png)

1. Cree un filtro para el objeto original.\
   Por ejemplo, cree un filtro Parameter .\
   Para obtener información sobre la creación de filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Haga clic en **Cambiar al modo de texto**.
1. (Condicional) Si está filtrando objetos que faltan, pegue el siguiente ejemplo de fórmula en la interfaz de modo de texto del nuevo filtro y reemplace el texto sugerido con los objetos y campos correctos:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   Para ver un ejemplo de los informes en campos personalizados que no están asociados a Forms personalizado, consulte la [Ejemplo 2: Filtre para los objetos que faltan: campos personalizados que no aparecen en ningún formulario personalizado](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms) en este artículo.

1. Haga clic en **Guardar filtro**.

## Ejemplos de filtros de modo de texto que abarcan varios niveles en la jerarquía de objetos

* [Ejemplo 1: Filtrar por problemas por nombre de propietario del Portfolio](#example-1-filter-for-issues-by-portfolio-owner-name)
* [Ejemplo 2: Filtre para los objetos que faltan: campos personalizados que no aparecen en ningún formulario personalizado](#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms)
* [Ejemplo 3: Filtre para los objetos que faltan: usuarios que no hayan registrado la hora durante un determinado período de tiempo](#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time)
* [Ejemplo 4: Filtrar por varios campos: tareas por nombre de propietario del Portfolio y por ID de informe de valoración de alineación del Portfolio](#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id)

### Ejemplo 1: Filtrar por problemas por nombre de propietario del Portfolio {#example-1-filter-for-issues-by-portfolio-owner-name}

Con la interfaz del modo de texto, puede crear un filtro para una lista de problemas para mostrar solo los problemas que están en proyectos asociados con un portafolio cuyo propietario es un usuario específico.

Para filtrar problemas por el nombre del propietario del Portfolio:

1. Cree un filtro de problemas.\
   Para obtener información sobre la creación de filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Haga clic en **Cambiar al modo de texto**.
1. Consulte el siguiente código genérico:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:<Target Object>:<Target Field>=<Your value for the Target Field>
   ```

1. Pegue el siguiente código en la sección **Definir reglas de filtro para el informe** para reemplazar el código genérico anterior:

   <pre>EXISTE:A:$$OBJCODE=PROJ<br>EXISTE:A:ID=FIELD:projectID<br>EXISTE:A:portafolio:ownerID=4d94d7da001699b19edf50de15682221</pre>

   >[!NOTE]
   >
   >* El objeto Original es el objeto del informe: Problema
   >* El objeto Target es Portfolio.
   >* El objeto de vinculación es Project.
   >* El campo de destino y el campo de vinculación al objeto de destino al que se hace referencia desde el objeto de vinculación es ownerID.
   >* El código de objeto del objeto de vinculación aquí es PROJ.
   >* El campo de vinculación que se muestra en el objeto original es projectID y el campo de vinculación es ID.


1. Reemplace el valor del campo de destino (ownerID) en la última instrucción por un ID de usuario de su entorno.
1. Haga clic en **Guardar filtro**.

### Ejemplo 2: Filtre para los objetos que faltan: campos personalizados que no aparecen en ningún formulario personalizado {#example-2-filter-for-missing-objects-custom-fields-that-do-not-appear-in-any-custom-forms}

Con la interfaz del modo de texto, puede crear un filtro para ver los campos personalizados (parámetros) que no están asociados a Forms personalizado (categorías). Este filtro vincula Parámetros a Categorías, que están conectados a través de otro objeto, Parámetro de categoría. Puesto que los dos campos no están conectados directamente entre sí y porque está filtrando por falta de información, debe utilizar una instrucción EXISTS.

>[!IMPORTANT]
>
>Un parámetro es un campo tal como existe en la Biblioteca de campos a la que se hace referencia en un formulario personalizado. Un parámetro de categoría es la versión de un campo que aparece en un formulario específico. Por ejemplo, si el mismo campo aparece en 5 formularios, habrá 1 Parámetro y 5 Parámetros de categoría en la base de datos de Workfront.

Para filtrar campos personalizados que no están asociados a un formulario personalizado:

1. Cree un parámetro o un filtro de campo personalizado.\
   Para obtener información sobre la creación de filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Haga clic en **Cambiar al modo de texto**.
1. Consulte el siguiente código genérico:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Pegue el siguiente código en la sección **Definir reglas de filtro para el informe** para reemplazar el código genérico anterior:

   <pre>EXISTE:A:$$OBJCODE=CTGYPA<br>EXISTE:A:parameterID=FIELD:ID<br>EXISTE:A:$$EXISTSMOD=NOTEXISTS</pre>

   >[!NOTE]
   >
   >* El objeto Original es el objeto del informe: Parámetro.
   >* El objeto de destino es la categoría.
   >* El objeto de vinculación es un parámetro de categoría.
   >* El código de objeto del objeto de vinculación es CTGYPA.
   >* El campo Vinculación al objeto de destino es parameterID porque existe parameterID tanto en la tabla de objetos vinculados como en la tabla de objetos de destino.
   >* El campo de vinculación que se muestra en el objeto original es ID (del parámetro de categoría).


1. Haga clic en **Guardar filtro**.

### Ejemplo 3: Filtre para los objetos que faltan: usuarios que no hayan registrado la hora durante un determinado período de tiempo {#example-3-filter-for-missing-objects-users-who-did-not-log-time-for-a-certain-period-of-time}

Con la interfaz de modo de texto, puede crear un filtro para ver los usuarios que no han registrado la hora durante un período de tiempo determinado. Este filtro vincula a los usuarios con las horas, que están conectados entre sí directamente. Sin embargo, debe utilizar una instrucción EXISTS y la interfaz de modo de texto para poder filtrar por información que falte.

Para filtrar por usuarios que no hayan registrado la hora durante la semana pasada:

1. Crear un filtro de usuario.\
   Para obtener información sobre la creación de filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Haga clic en **Cambiar al modo de texto**.
1. Consulte el siguiente código genérico:

   ```
   EXISTS:A:$$OBJCODE=<Object code of the Linking Object><br>
   ```

   ```
   EXISTS:A:<Linking Field displayed on the Linking Object>=FIELD:<Linking Field displayed on the Original Object><br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

1. Pegue el siguiente código en la sección **Definir reglas de filtro para el informe** para reemplazar el código genérico anterior:

   ```
   EXISTS:A:$$OBJCODE=HOUR<br>EXISTS:A:ownerID=FIELD:ID<br>EXISTS:A:entryDate=$$TODAYb-1w<br>EXISTS:A:entryDate_Range=$$TODAYe-1w<br>EXISTS:A:entryDate_Mod=between<br>EXISTS:A:$$EXISTSMOD=NOTEXISTS
   ```

   >[!NOTE]
   >
   >* El objeto Original es el objeto del informe: Usuario.
   >* El objeto de destino es hora.
   >* En este ejemplo no necesita un objeto de vinculación porque Usuarios y horas están conectados directamente en la base de datos de Workfront.
   >* Como no hay ningún objeto vinculado, debe utilizar el código de objeto del objeto de destino: HORA.
   >* El campo Vinculación al objeto de destino es ownerID (que se muestra en el objeto original; falta el objeto de vinculación).
   >* El campo de vinculación que se muestra en el objeto original es ID (de la hora) (que se muestra en el objeto de destino; falta el objeto de vinculación).
   >* EXISTE:A:La instrucción entryDate hace referencia a campos que definen el objeto de destino (hora) y utilizan la misma sintaxis que en una instrucción de filtro normal. Esto garantiza que solo se muestren los usuarios que no hayan registrado la hora durante un período de tiempo específico, en este caso la semana anterior.
   >* El modificador NOTEXISTS indica que estamos buscando elementos (horas) que no existen para el objeto del informe (Usuarios).


1. Haga clic en **Guardar filtro**.

### Ejemplo 4: Filtrar por varios campos: tareas por nombre de propietario del Portfolio y por ID de informe de valoración de alineación del Portfolio {#example-4-filter-by-multiple-fields-tasks-by-portfolio-owner-name-and-portfolio-alignment-scorecard-id}

Con la interfaz de modo de texto, puede crear un filtro que haga referencia a más de un campo en el objeto de destino. En este caso, las instrucciones de filtro que hacen referencia a los campos de destino deben estar conectadas mediante AND.

Por ejemplo, puede filtrar una lista de tareas para que muestre solo las tareas que cumplen los siguientes criterios:

* Están en un proyecto asociado con un portafolio cuyo propietario es un usuario específico.
* Están en un proyecto asociado a un portafolio cuyos proyectos no están asociados a un informe de valoración de alineación específico.

Para filtrar tareas por nombre de propietario del Portfolio y por ID de informe de valoración de alineación del Portfolio:

1. Crear un filtro de tarea.\
   Para obtener información sobre la creación de filtros, consulte [Información general sobre filtros en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).

1. Haga clic en **Cambiar al modo de texto**.
1. Pegue el siguiente código en la sección **Definir reglas de filtro para el informe** área:
   <pre>EXISTE:A:$$OBJCODE=PROJ<br>EXISTE:A:ID=FIELD:projectID<br>EXISTE:A:portafolio:ownerID=4d80ce5200000528787d57807732a33f<br>Y:A:EXISTE:A:$$EXISTSMOD=NOTEXISTS<br>Y:A:EXISTE:A:$$OBJCODE=PROJ<br>Y:A:EXISTE:A:ID=FIELD:projectID<br>Y:A:EXISTE:A:portafolio:alignmentScoreCardID=4da387b00001cbc732bb259355c33dad</pre>

   >[!NOTE]
   >
   >* El objeto Original es el objeto del filtro: Tarea.
   >* El objeto Target es Portfolio.
   >* El primer campo de destino es ownerID.
   >* El segundo campo de destino es el ID del informe de valoración de alineación.
   >* El objeto de vinculación es Project.
   >* El código de objeto del objeto de vinculación es PROJ.
   >* El campo Vinculación al objeto de destino es el ID (del Portfolio).
   >* El campo de vinculación mostrado en el objeto original es projectID.
   >* Reemplace ownerID por un ID de usuario de su entorno.


1. Haga clic en **Guardar filtro**.
