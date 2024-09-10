---
user-type: administrator
product-area: system-administration
keywords: KickStart, KickStart, KickStart, KickStart
navigation-topic: use-kick-starts
title: Importación de datos en Workfront mediante una plantilla de KickStart
description: Los Kick-Starts son libros de Excel con formato especial que se pueden rellenar con los datos que se desean importar a Workfront. Adobe Workfront proporciona una plantilla de KickStart que puede utilizar para hacerlo, tal como se explica en el importador de datos de KickStarts.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 25813946-e338-4dd9-b02c-d20fa18c539c
source-git-commit: dc64fef83c2b1e9f8bf9438017155bd47b83ab23
workflow-type: tm+mt
source-wordcount: '2750'
ht-degree: 6%

---

# Importación de datos en Workfront mediante una plantilla de KickStart

<!--Audited: 12/2023-->

Los Kick-Starts son libros de Excel con formato especial que se pueden rellenar con los datos que se desean importar a Workfront. Adobe Workfront proporciona una plantilla de KickStart que puede usar para hacerlo, tal como se explica en [Importador de datos de Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/kick-starts-data-importer.md).

Este proceso se divide en 3 tareas principales:

* En primer lugar, exporte una plantilla de KickStart como archivo de hoja de cálculo
* En segundo lugar, se rellena la hoja de cálculo con los datos
* Por último, importe la hoja de cálculo rellenada en Workfront

Cada uno de estos procedimientos se describe en el orden adecuado en este artículo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p> Nuevo: estándar</p>
   o
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL Administrador del sistema]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Limitaciones

Puede importar una gran cantidad de objetos en Workfront mediante una plantilla de KickStart. Sin embargo, tenga en cuenta las siguientes limitaciones:

* La importación de datos de este modo no actualiza la información de los registros que ya existen en Workfront.
* Solo se pueden importar registros nuevos y su información.
* No importe más de 2000 registros a la vez para garantizar que no se agote el tiempo de espera de la importación

## Exportar una plantilla de KickStart como archivo de hoja de cálculo

Cuando exporta una plantilla de KickStart, recibe un libro de Excel en blanco. Una vez que la hoja de cálculo se haya descargado en el equipo, puede utilizarla para rellenarla con la información y, a continuación, importarla de nuevo a Workfront.

Para exportar una plantilla de KickStart:

{{step-1-to-setup}}

<!--
1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).  -->

1. Haga clic en **Sistema** > **Importar datos (Kick-Starts)**.

1. Seleccione los tipos de información que desea incluir.

   Cada opción seleccionada representa una colección de varias fichas en la hoja de cálculo exportada. Por ejemplo, si selecciona la opción **Informe**, todos los objetos necesarios para crear un informe se incluirán en la hoja de cálculo (vistas, filtros, agrupaciones, informes).

   Puede utilizar todos los tipos de objetos enumerados a continuación para importar datos en Workfront. (La única excepción es la opción Niveles de acceso. La hoja de datos Niveles de acceso de una exportación se proporciona con fines de referencia (le permite asignar un nivel de acceso a una nueva cuenta de usuario por identificador).

   La plantilla para cada uno de los tipos de objeto se puede exportar en los siguientes formatos de archivo y contiene las siguientes hojas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <col> 
    <thead> 
     <tr> 
      <th> <p><strong>Objeto</strong> </p> </th> 
      <th> <p><strong>Exportaciones como</strong> </p> </th> 
      <th> <p><strong>Hojas en la hoja de cálculo exportada</strong> </p> </th> 
     </tr> 
    </thead> 
    <tbody> 
     <tr> 
      <td scope="col"> <p>Panel de control</p> <p>Todos los paneles del sistema están disponibles para exportar. Puede seleccionar hasta 100 paneles específicos en una sola exportación.</p> </td> 
      <td scope="col">Exportaciones como archivo ZIP</td> 
      <td scope="col"> <p>Parámetro</p> <p>Texto descriptivo</p><p>Opción del parámetro</p> <p>Grupo de parámetros</p> <p>Parámetro de categoría</p> <p>Categoría</p> <p>Informe</p> <p>Sección de la ficha de portal</p> <p>Panel de control</p> <p>Preferencias</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Informe</p> <p>Todos los informes del sistema están disponibles para exportar. Puede seleccionar hasta 100 informes específicos en una sola exportación.</p> <p>Kick-Starts no admite filtros de modo de texto. Para que la exportación se realice correctamente, los filtros de creación de informes deben cambiarse al modo Estándar.</p> </td> 
      <td scope="col">Exportaciones como archivo ZIP </td> 
      <td scope="col"> <p scope="col">Parámetro</p> <p scope="col">Texto descriptivo</p> <p scope="col">Opción del parámetro</p> <p scope="col">Grupo de parámetros</p> <p scope="col">Parámetro de categoría</p> <p scope="col">Categoría</p> <p scope="col">Informe</p> <p scope="col">Preferencias</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Aprobación</p> </td> 
      <td scope="col"> <p>Exportaciones como archivo de Excel</p> </td> 
      <td scope="col"> <p>Aprobador de fase</p> <p>Fase de aprobación</p> <p>Aprobación</p> <p>Proceso de aprobación</p> <p>Preferencias</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Datos personalizados</p> </td> 
      <td scope="col"> <p>Exportaciones como archivo de Excel</p> </td> 
      <td scope="col"> <p>Parámetro</p> <p>Texto descriptivo</p>  <p>Opción del parámetro</p> <p>Grupo de parámetros</p> <p>Parámetro de categoría</p> <p>Categoría</p> <p>Preferencias</p> </td> 
     </tr> 
     <tr> 
      <td scope="col"> <p>Tipo de gasto</p> </td> 
      <td scope="col"> <p>Exportaciones como archivo de Excel</p> </td> 
      <td> <p>Tipo de gasto</p> <p>Preferencias</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Tipo de hora</p> </td> 
      <td scope="col"> <p>Exportaciones como archivo de Excel</p> </td> 
      <td> <p>Tipo de hora</p> <p>Preferencias</p> </td> 
     </tr> 
     <tr> 
      <td> <p>Equipo</p> </td> 
      <td scope="col"> <p>Exportaciones como archivo de Excel</p> </td> 
      <td> <p> Miembro del equipo</p> <p>Equipo</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td> <p>Usuario</p> </td> 
      <td> <p>Se exporta como un archivo de Excel. Para ver la lista completa de opciones, haga clic en <strong>Más opciones</strong>.</p> </td> 
      <td> <p>Usuario</p> <p>Preferencias</p> </td> 
     </tr> 
     <tr> 
      <td>Nivel de acceso</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p>Nivel de acceso</p> <p>Preferencias</p> </td> 
     </tr> 
     <tr> 
      <td>Asignación</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p>Asignación</p> <p>Preferencias</p> </td> 
     </tr> 
     <tr> 
      <td>Compañía</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Compañía</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Plantilla de mensaje de correo electrónico</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p>Plantilla de mensaje de correo electrónico</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Gasto</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Gasto'</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Página externa</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Página externa</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Filtro</td> 
      <td>Exportaciones como archivo ZIP</td> 
      <td> <p> Filtro</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Grupo</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Grupo</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Agrupación</td> 
      <td>Exportaciones como archivo ZIP</td> 
      <td> <p> Agrupación</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Hora</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Hora</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Problema</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Problema</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Función</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Función del puesto</p> <p>Preferencias </p> </td> 
     </tr>

   <tr> 
      <td>Ruta de hitos</td> 
      <td> Exportaciones como archivo de Excel</td> 
      <td> <p> Hito</p> <p>Ruta de hitos</p> <p>Preferencias </p> </td> 
     </tr>

   <tr> 
      <td>Nota</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Nota</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Portafolio</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Portafolio</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Proyecto</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Cola</p> <p>Proyecto</p> <p>Regla de enrutamiento</p> <p>Tema de la cola</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Estimación de recursos</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Estimación de recursos</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Riesgo</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Riesgo</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Tipo de riesgo</td> 
      <td> Exportaciones como archivo de Excel</td> 
      <td> <p> Tipo de riesgo</p> <p>Preferencias</p> </td> 
     </tr> 
     <tr> 
      <td>Tarjeta de puntuación</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p>Pregunta de tarjeta de puntuación</p> <p>Opción de tarjeta de puntuación</p> <p>Tarjeta de puntuación</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Tarea</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Tarea</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Plantilla</td> 
      <td> Exportaciones como archivo de Excel</td> 
      <td> <p> Cola</p> <p>Plantilla</p> <p>Regla de enrutamiento</p> <p>Tema de la cola</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Asignación de plantilla</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Asignación de plantilla</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Tarea de plantilla</td> 
      <td>Exportaciones como archivo de Excel</td> 
      <td> <p> Tarea de plantilla</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Hoja de horas</td> 
      <td> Exportaciones como archivo de Excel</td> 
      <td> <p> Perfil de hoja de horas</p> <p>Hoja de horas</p> <p>Preferencias </p> </td> 
     </tr> 
     <tr> 
      <td>Ver </td> 
      <td> <p>Exportaciones como archivo ZIP</p> </td> 
      <td> <p> Ver</p> <p>Preferencias </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Descargar**.
1. Continúe con [Rellene la plantilla de hoja de cálculo con sus datos](#populate-the-spreadsheet-template-with-your-data) para rellenar la hoja de cálculo de plantilla en blanco con su información.

## Rellene la plantilla de hoja de cálculo con los datos {#populate-the-spreadsheet-template-with-your-data}

* [Descripción general de las fichas (hojas de datos) incluidas en la hoja de cálculo](#overview-of-the-tabs-data-sheets-included-in-the-spreadsheet)
* [Importar un registro](#import-a-record)
* [Incluir fechas](#include-dates)
* [Usar caracteres comodín](#use-wildcards)
* [Sustitución de nombres de atributo para ID](#attribute-name-substitution-for-ids)

### Descripción general de las fichas (hojas de datos) incluidas en la hoja de cálculo

>[!TIP]
>
>Para comprender mejor cómo tendrá que dar formato a la información de cada columna al rellenar la plantilla de KickStart, considere la posibilidad de realizar una ejecución de práctica exportando un KickStart con datos de Workfront existentes en los objetos que está intentando importar. Para obtener instrucciones, consulte [Exportar datos de Adobe Workfront mediante Kick-Starts](../../../administration-and-setup/manage-workfront/using-kick-starts/export-data-from-wf-via-kick-starts.md).

Al abrir una plantilla de Kick-Starts en blanco, hay varias pestañas (hojas de datos) disponibles. Dependen de los objetos seleccionados para la descarga. Cada uno representa un objeto en la aplicación, como proyecto, tareas, horas, panel y usuarios:

Al abrir una de estas pestañas, la fila 2 muestra los campos de cada objeto que se puede establecer durante una importación. En un encabezado de columna, después de la palabra &quot;set&quot;, el nombre del campo se muestra tal y como aparece en la base de datos. Estos campos actúan como encabezados de columna.

>[!IMPORTANT]
>
>Para evitar errores, asegúrese de lo siguiente:
>
>* No elimine la primera fila vacía de una hoja de cálculo de inicio rápido.
>* No elimine, modifique ni reorganice estos campos (encabezados de columna) de ninguna manera. Por ejemplo, no cambie el orden ni los nombres.
>* Agregue valores a cada campo que se muestre en negrita en el encabezado de la columna. Estos representan campos obligatorios.
>
>     Sin embargo, si un campo obligatorio contiene un valor predeterminado establecido en las preferencias del sistema, no tiene que rellenarlo.
>
>     Por ejemplo, en la ficha **Proyecto PROJ**, los campos **setCondition** y **setConditionType** pueden dejarse vacíos, pero las columnas **setGroupID** y **setName** no pueden.
>
>* El sistema genera automáticamente ciertos campos, como **setResourceRevenue** y **setEnteredByID**. Si se introducen datos para estos campos en la hoja de cálculo, el proceso de KickStart los sustituirá al cargar la hoja de cálculo.

### Importar un registro  {#import-a-record}

Cada fila de la hoja corresponde a un objeto único.

1. Agregar información en la columna **isNew**:

   * Si el objeto que está importando es nuevo, escriba **TRUE** para importar los datos de la fila. Este valor distingue entre mayúsculas y minúsculas y siempre debe escribirse en mayúsculas
   * Si el objeto ya está en Workfront, escriba **FALSE** en la columna **isNew** para omitir la fila. Este valor distingue entre mayúsculas y minúsculas y siempre debe escribirse en mayúsculas

      * Los registros que ya existen en Workfront no se actualizan.
      * Si ha descargado una plantilla con datos de Workfront, los objetos existentes ya están marcados con **FALSE**.
      * Si ha descargado una plantilla en blanco, no es necesario agregar nuevas filas para los objetos existentes.

1. Agregue información en la columna **ID** de una de las siguientes maneras:

   * Si el objeto que está importando es nuevo (y escribió **TRUE** en la columna **isNew**), escriba cualquier número para el identificador. Este número debe ser único en la hoja de cálculo. Por ejemplo, si importa tres objetos, puede darles el ID de 1, 2 y 3 respectivamente.

   * Si el objeto ya existe en Workfront (y **FALSE** está en la columna **isNew**) y está importando información nueva sobre objetos existentes, el identificador debe ser el GUID alfanumérico que existe en Workfront para ese objeto.

   >[!TIP]
   >
   > Para averiguar el GUID único de un objeto en Workfront, puede crear un informe para ese objeto y agregar la columna ID al informe. El valor de cada objeto de esa columna es el GUID del objeto.

   * Los registros que ya existen en Workfront no se actualizan.
   * Si ha descargado una plantilla con datos, los objetos existentes ya contienen el GUID como ID.
   * Puede importar un nuevo objeto basado en un objeto existente cambiando **FALSE** a **TRUE** en la columna **isNew**, cambiando el identificador y realizando los ajustes de datos necesarios antes de la importación.

   ![ID de muestra para un grupo](assets/kick-start-group-example.png)

   * Al importar un proyecto, debe indicar un ID de grupo.

      * Si el grupo ya existe en Workfront, debe agregar su identificador único al campo **setGroupID** del proyecto.
      * Si el grupo no existe en Workfront, puede agregar la hoja **GROUP Group** al archivo de importación, establecer el campo **isNew** en **TRUE** en la hoja Group e indicar un identificador numérico para el nuevo grupo en la columna **ID**. El campo **setGroupID** del nuevo proyecto debe coincidir con el **ID** numérico del nuevo grupo.

     **Ejemplo:** Para un proyecto, el valor mostrado en la columna **setGroupID** debe ser uno de los siguientes:

      * GUID de un grupo existente en su instancia de Workfront
      * El valor (número) de la columna Id. de la hoja **Grupo de grupo** si está creando un nuevo grupo durante la importación

1. Introduzca valores para los campos obligatorios y cualquier otro campo que desee rellenar durante la importación.
1. (Opcional) Para agregar datos personalizados:

   * Cree una nueva columna para cada campo personalizado que desee incluir en el proceso de importación.
   * Asigne un nombre a cada nueva columna para su campo personalizado correspondiente de la siguiente manera: **DE:[Nombre del campo personalizado tal como aparece en Workfront]**. Por ejemplo, puede crear el siguiente campo personalizado: &quot;DE: Departamentos&quot;.
   * En la columna **setCategoryID**, escriba el GUID del formulario personalizado existente en el que reside este campo personalizado. Este campo es obligatorio al importar datos personalizados.
   * Si necesita agregar varios valores de datos en el campo personalizado (como botones de opción, casillas de verificación o listas), utilice el delimitador de datos personalizados de barra vertical &quot;|&quot; que aparece en la pestaña Preferencias para separar los valores.

     **Ejemplo:** escriba A|D en la columna DE:Departamentos para rellenar los departamentos A y D en el formulario personalizado.

### Incluir fechas  {#include-dates}

Workfront puede procesar la mayoría de los formatos de fecha. Sin embargo, debe asegurarse de que la columna de fecha de la hoja de cálculo tenga el formato de fecha. La importación fallará si la columna tiene el formato general, un número o texto.

>[!TIP]
>
>El formato más popular es el formato MM/DD/AAAA.
>
>Por ejemplo: 10/07/2023.

Workfront también acepta valores de hora como parte de la fecha.

Por ejemplo: 10/07/2022 01:30 o 10/07/2022 1:00 p.m.

Si omite una hora en la fecha, Workfront realiza una de las siguientes acciones:

* Asume que la hora es 12:00 AM. Para ver el resultado de la fecha que espera, la zona horaria del sistema debe coincidir con la del sistema.
* Si se encuentra en un objeto asociado a una programación, el tiempo se difiere a la primera vez que la programación lo permite.

>[!NOTE]
>
>Cuando utilice una marca de tiempo UNIX, debe incluir tres ceros adicionales al final del valor.
>
>Por ejemplo, si la marca de tiempo es 7336899000, debe introducir 7336899000000 en la celda.

### Usar caracteres comodín {#use-wildcards}

Al rellenar la hoja de cálculo de la plantilla de KickStart, puede utilizar los siguientes caracteres comodín:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Comodín</strong> </p> </th> 
   <th> <p><strong>Comportamiento</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>$$TODAY</p> </td> 
   <td> <p>Cuando se usa en un campo <strong>setDate</strong>, este comodín establece la fecha como medianoche del día en que se importa el Kick-Start.</p> <p>Puede modificar el comodín utilizando la sintaxis estándar permitida con el comodín en un filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Si desea que un proyecto comience el lunes de la semana en que se importa, independientemente del día en que realmente realice la importación, puede usar <strong>$$TODAYbw</strong>. Esto establece la fecha planificada de inicio del proyecto como 12:00 a.m. del domingo. Dado que el horario del proyecto probablemente no permita trabajar a esa hora, comenzará a las 9:00 AM del lunes por la mañana.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$NOW</p> </td> 
   <td> <p>Cuando se usa en un campo <strong>setDate</strong>, este comodín establece la fecha según el momento en que se crea el registro durante la importación de KickStart.</p> <p>Puede modificar el comodín utilizando la sintaxis estándar permitida con el comodín en un filtro.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Ejemplo: </b></span></span>Si desea que un proyecto se inicie 3 horas después de importarlo, puede usar <strong>$$NOW+3h</strong>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$USER.ID</p> </td> 
   <td> <p>Cuando se utiliza en <strong>setAssignedToID</strong> u otro campo basado en userID, este comodín asigna el trabajo o asocia de otro modo el registro con el individuo que realiza la importación.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>$$CUSTOMER</p> </td> 
   <td> <p>Este comodín se agregó específicamente para importaciones de usuarios de KickStart. Cuando se crea una cuenta de Workfront, se crea un usuario con el nivel de acceso de administrador del sistema. El nombre de usuario asignado al administrador predeterminado puede utilizarse como prefijo al crear otros usuarios en la cuenta.</p> <p>Dado que los nombres de usuario deben ser únicos en todos los clientes, esto resulta útil cuando tiene varias personas con nombres de usuario muy comunes, como Juan Pérez, que pueden tener un nombre de usuario "jsmith". Al anteponer la asignación de nombre de usuario con el nombre de usuario de administrador predeterminado, garantiza que cada nombre de usuario es único (por ejemplo: <strong>$$CUSTOMER.jsmith</strong>).</p> <p>Sugerencia: Una forma más elegante de asegurarse de que los nombres de usuario sean únicos en todo el sistema es introducir la dirección de correo electrónico del individuo en el campo <strong>setUsername</strong>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sustitución de nombres de atributo para ID  {#attribute-name-substitution-for-ids}

Aunque es recomendable usar identificadores siempre que sea posible, a veces resulta incómodo hacer referencias cruzadas de los identificadores de una hoja a otra al establecer un valor **setAttributeID**. Puede hacer referencia a los valores por nombre simplemente cambiando el encabezado de la columna.

**Ejemplos:**

* **Importación de proyecto**

  Al importar proyectos, establezca el **setGroupID** de los proyectos en la hoja **GROUP Group**, tome nota de los respectivos ID de grupo y péguelos en las celdas correctas (columna **setGroupID**) en la hoja **PROJ Project**.

  Esto es factible cuando se trabaja con solo unos pocos grupos y proyectos, pero si se trabaja con varios de cada uno, no es práctico.

  Para realizar la sustitución de nombres de atributo para el ejemplo descrito anteriormente, cambia el encabezado de columna **setGroupID** a **#setGroupID GROUP name**. A continuación, puede hacer referencia al grupo de cada proyecto por su nombre.

  >[!NOTE]
  >
  >La opción de usar Sustitución de nombre de atributo se limita únicamente a las referencias para los registros existentes. No se puede utilizar la sustitución de nombres para los objetos que se están creando en la misma importación.

* **Importación de usuario**

  Al importar usuarios, rellene **setRoleID** de una lista de funciones en la ficha **FUNCIÓN**.

  Algunos de los identificadores de rol son para registros que ya existen en la cuenta y otros se están creando durante la importación.

  Para los registros de usuario nuevos asignados a funciones existentes, puede utilizar la sustitución de nombres. Para los registros de usuario nuevos asignados a roles recién importados, no puede.

  A continuación se muestra cómo puede utilizar ambos métodos en el mismo archivo de importación:

   * Agregue una columna en la hoja de cálculo a la izquierda de la columna **setRoleID**.
   * Asigne un nombre a la nueva columna **#setRoleID ROLE name**.
   * Para las asignaciones de roles a registros existentes, escriba los nombres de roles en la columna **#setRoleID ROLE name**.

     Para las asignaciones de roles a nuevos registros de roles, introduzca el ID asignado en la hoja ROL Rol en setRoleID.

     ![Identificador de rol para usuarios](assets/set-role-id.png)

## Importar los datos de la hoja de cálculo en Workfront

Después de rellenar la plantilla de Excel con los datos, puede cargar los datos en Workfront.

La importación de KickStart admite los siguientes tipos de archivo:

* Excel (.xls o .xlsx)
* Archivo comprimido (.ZIP) (que contiene solo archivos .xlsx o .xls)

  >[!NOTE]
  >
  >Debe utilizar un archivo .ZIP al importar hojas de cálculo de Excel que hagan referencia a los objetos siguientes:
  >
  >* Informes
  >* Documentos
  >* Avatares
  >* Ver, filtrar o agrupar archivos de propiedades
  >
  >Al utilizar un archivo de importación comprimido, el archivo .ZIP debe tener el mismo nombre que el archivo .xlsx o .xls y todos los archivos deben tener el mismo nivel de estructura (sin carpetas).

Para importar los datos de la hoja de cálculo de plantillas en Workfront:

<!--1. Click the **Main Menu** icon ![](assets/main-menu-icon.png) in the upper-right corner of Adobe Workfront, then click **Setup** ![](assets/gear-icon-settings.png).-->

{{step-1-to-setup}}

1. Haga clic en **Sistema** > **Importar datos (Kick-Starts)**.

1. En la sección **Cargar datos con hoja de cálculo de KickStart**, haga clic en **Elegir archivo**, busque y seleccione la hoja de cálculo rellenada.

1. Haga clic en **Cargar.**

   Si el archivo de Excel tarda más de 5 minutos en cargarse en Workfront, la aplicación agota el tiempo de espera y Workfront no puede cargar el archivo.

   Intente importar los datos en lotes de objetos más pequeños.

1. (Condicional) Si utiliza Workfront Fusion, ahora puede activar los FLO o escenarios.
