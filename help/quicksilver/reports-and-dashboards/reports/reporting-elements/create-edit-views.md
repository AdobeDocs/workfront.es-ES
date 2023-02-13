---
product-area: reporting
navigation-topic: reporting-elements
title: Crear o editar vistas en Adobe Workfront
description: Puede personalizar el tipo de información que muestra en la pantalla mediante vistas. Puede utilizar varios tipos de vistas en Adobe Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: 442e0b8fde9e4acaa2686ccd292fb003f72be623
workflow-type: tm+mt
source-wordcount: '1748'
ht-degree: 1%

---

# Crear o editar vistas en Adobe Workfront

Puede personalizar el tipo de información que muestra en la pantalla mediante vistas. Puede utilizar varios tipos de vistas en Adobe Workfront.

En este artículo se describe cómo crear y editar vistas estándar para listas e informes, y cómo crear vistas ágiles. Para obtener más información, consulte [Información general sobre las vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan de Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a filtros, vistas y grupos</p> <p>Editar acceso a informes, tableros y calendarios para crear una vista en un informe</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administrar permisos para un informe para crear o editar una vista en un informe</p> <p>Administrar permisos en una vista para editarla</p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear o personalizar una vista

El proceso para crear o personalizar una vista varía en función de si se está creando o personalizando una vista estándar o una vista ágil.

* [Crear o personalizar una vista estándar](#create-or-customize-a-standard-view)
* [Creación o personalización de una vista Águila](#create-or-customize-an-agile-view)

### Crear o personalizar una vista estándar {#create-or-customize-a-standard-view}

Puede crear una nueva vista estándar o personalizar una vista estándar existente que haya creado anteriormente.

1. Haga clic en el **Ver** menú desplegable de cualquier lista en la que desee crear o personalizar una vista.
1. (Opcional) Para personalizar una vista existente, seleccione la vista estándar que desee personalizar.\
   Las vistas estándar están disponibles en cualquier tipo de lista de Workfront, como un informe, una lista de proyectos o una lista de tareas.
1. Haga clic en el **Ver** menú desplegable y haga clic en **Personalizar vista** o **Nueva vista**.\
   La variable **Personalizar vista** se abre.

1. En el **Vista previa de columna** , realice una de las acciones siguientes:

   * Modifique el valor de cualquier columna haciendo clic en el título de la columna y seleccionando a continuación un nuevo campo.
   * Agregue una columna haciendo clic en **Agregar columna**, empiece a escribir el nombre de la columna que desea agregar y, a continuación, haga clic en ella cuando aparezca en la lista desplegable.
   * Ajuste el orden en que aparecen las columnas arrastrando el título de la columna a una nueva ubicación.

      * (Opcional) En la **Configuración de columna** , haga clic en el **Resumir esta columna por** lista desplegable y, a continuación, seleccione una de las opciones disponibles para resumir la información. Al elegir esta opción, la información de la columna se agrega en las agrupaciones del informe.\
         Para los campos de fecha, puede resumir los valores con las siguientes opciones:

         * Máximo
         * Mínimo

         Para los campos de número y moneda, puede resumir los valores con las siguientes opciones:

         * Cuenta
         * Suma
         * Promedio
         * Máximo
         * Mínimo

         >[!NOTE]
         >
         >Las siguientes excepciones se aplican a los objetos principales (por ejemplo, tareas principales) cuando se agregan valores para los siguientes campos en agrupaciones:
         >   
         >   * Todos los campos de número y moneda excepto Horario real (por ejemplo, Coste laboral planeado/real, Coste planeado/real, Coste planeado/real, Horario planificado) agregan solamente los valores para las tareas secundarias y las tareas independientes. No acumulan los valores para las tareas principales o los principales de los padres.
         >   * Las horas reales agregan los valores para las tareas principales y las tareas independientes; no agregan los números para los elementos principales de las tareas principales o las tareas secundarias.
         >   * Los campos de datos personalizados para valores numéricos y monetarios agregan todas las tareas: padres, hijos, padres de padres y tareas independientes.


         Para obtener más información sobre el uso de agrupaciones en un informe, consulte el artículo [Información general sobre las agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Opcional) Haga clic en **Opciones avanzadas** para especificar la siguiente información para la columna:

         <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Etiqueta personalizada de columna</strong></td> 
           <td><p>Especifique una etiqueta personalizada para la columna. Esta etiqueta reemplaza la etiqueta predeterminada.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Formato de campo</strong></td> 
           <td>Seleccione el formato en el que desea que se muestren los valores para los campos de la columna .</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Mostrar esta columna en panel</strong></td> 
           <td><p>Seleccione esta opción para mostrar esta columna en un tablero, cuando el informe se muestre en paralelo con otro informe. Cuando se anula la selección de esta opción, esta columna no se muestra al ver el informe en un tablero en el que los informes se muestran uno al lado del otro.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Reglas de columna</strong></td> 
           <td><p>Haga clic en <strong>Agregar una regla para esta columna</strong> para definir una regla para la columna. Después de agregar una regla, puede definir los estilos de campo y texto para ver cómo se muestran los campos que coinciden con esa regla. Haga clic en <strong>Agregar regla</strong> una vez que haya terminado de definir la regla.</p></td> 
          </tr> 
         </tbody> 
        </table>

         Para obtener más información sobre el formato condicional de las vistas en los informes, consulte el artículo [Utilizar el formato condicional en modo de texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).



1. (Condicional) Si ha hecho clic en **Opciones avanzadas**, haga clic en **Listo**.

1. Haga clic en **Guardar vista** para crear una vista nueva o reemplazar la vista actual con los cambios.\
   O\
   Haga clic en **Guardar como vista nueva** para guardar los cambios como una vista nueva.

   >[!TIP]
   >
   >La variable **Guardar como vista nueva** es la única opción disponible al personalizar una vista integrada de Workfront.

   El acceso dicta cómo se guarda la vista. Si creó la vista originalmente, puede guardar los cambios; de lo contrario, se le pedirá que guarde una versión. Tenga en cuenta que los cambios que realice en la vista afectarán a los usuarios con los que se ha compartido la vista.

### Creación o personalización de una vista Águila {#create-or-customize-an-agile-view}

Se puede crear una nueva vista Águila o personalizar una vista Águila existente que haya creado anteriormente.

>[!IMPORTANT]
>
>Las vistas ágiles solo están disponibles cuando se visualiza un proyecto.

Para obtener más información sobre las vistas de Agile, consulte el artículo [Administrar un proyecto en la vista Águila](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: [! The information in the following steps is more or less duplicated in "Creating and Managing Agile Teams."])</p>
-->

Para crear o personalizar una vista Agile:

1. Vaya a la lista de tareas de un proyecto.
1. Haga clic en el **Guión gráfico Agile** icono ![](assets/agile-storyboard-nwe.png).

1. (Condicional) Para personalizar una vista Agile existente:

   1. Haga clic en el **Ver** menú desplegable y, a continuación, seleccione la vista Águila que desee personalizar.\
      No se puede personalizar la vista Agile predeterminada.

   1. Haga clic en el **Ver** menú desplegable de nuevo y, a continuación, haga clic en **Personalizar vista**.\
      ![](assets/view-agile-customize.png)

1. (Condicional) Para crear una nueva vista Águila, haga clic en **Nueva vista**.\
   La variable **Personalizar vista Ágica** se abre.

1. En el **Personalizar vista Ágica** , especifique un nombre para la vista Águila.\
   Le recomendamos que incluya la palabra &quot;Águila&quot; en el nombre de la vista, de modo que los usuarios sepan que se trata de una vista Águila.\
   Este nombre se muestra en la sección **Ver** menú desplegable al seleccionar una vista.

1. Defina las columnas de estado que se mostrarán en el tablero de artículos en la vista ágil. Estos son los estados de tareas definidos por el administrador de Workfront, tal como se describe en [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Solo los estados del sistema están disponibles para su uso en el tablero de historias Agile. Si un estado solo está disponible para un grupo individual del que es miembro, el estado no está disponible en el tablero de artículos ágil. Además, las tareas que están en un estado que solo está disponible para un grupo personalizado no son visibles al ver el proyecto en una vista Águila.

   Los usuarios pueden mover artículos entre estas columnas de estado en el tablero de artículos Agile.\
   Al definir columnas de estado, puede hacer lo siguiente:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Reordenar columnas de estado:</strong> </td> 
      <td> Arrastre una columna de estado al orden en el que desea que aparezca.<br><img src="assets/agile-project-reorderstatuses-350x141.png" alt="" style="width: 350;height: 141;"></td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Quitar columnas de estado:</strong> </td> 
      <td>Haga clic en el icono (x) de la columna que desee eliminar.<br>No se puede quitar el estado "Nuevo" a menos que se haya agregado un estado personalizado a la vista y que dicho estado personalizado equivalga a "Nuevo".<br>Para obtener información sobre cómo crear un estado personalizado, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Crear o editar un estado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Agregar columnas de estado:</strong> </td> 
      <td> <p>Haga clic en el <strong>Más</strong> y, a continuación, seleccione el estado que desee añadir.<br>Se muestran todos los estados predeterminados del sistema, así como cualquier estado personalizado que se haya compartido con usted.<br>Se pueden configurar hasta 10 estados para mostrar.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. En el **Asociar color de tarjeta a** , seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Historia:</strong> </td> 
      <td>Cualquier subtarea coincide con el color de la tarea principal, de modo que los colores de todas las historias en una línea de baño determinada sean los mismos.<br>Los colores se asignan aleatoriamente a tareas cuando se crean si la tarea no tiene ninguna subtarea o no tiene una tarea principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Forma libre:</strong> </td> 
      <td> De forma predeterminada, todas las tarjetas se muestran como azules hasta que un usuario cambia el color manualmente, tal como se describe en el artículo <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorizar artículos por color en el tablero Anulación</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridad:</strong> </td> 
      <td> <p> Los colores están asociados a la prioridad del artículo de la siguiente manera:</p> 
       <ul> 
        <li>Alto = Rojo</li> 
        <li>Medio = Amarillo</li> 
        <li>Bajo = Verde<br>Si el administrador de Workfront ha configurado prioridades personalizadas para su sistema Workfront, la prioridad más alta es roja, la segunda más alta es amarilla y las demás son verdes.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Propietario de tarea:</strong> </td> 
      <td> Todos los artículos con el mismo usuario asignado principal son del mismo color.<br>El usuario asignado principal es el usuario que se asignó primero a la tarea. </td> 
     </tr> 
    </tbody> 
   </table>

1. En el **Águila** en la sección **Campos adicionales** área, haga clic en **Agregar campo** y, a continuación, seleccione el campo que desee añadir a las tarjetas de artículo. (Son los mismos campos que se pueden añadir al crear una vista o crear columnas para un informe).\
   Repita este proceso para agregar hasta tres campos adicionales a las tarjetas de artículo.\
   Cuando se agregan campos a las tarjetas de artículo, los campos son de solo vista y se muestran solo cuando se rellena el campo.

   De forma predeterminada, se muestran los siguientes tipos de datos en la tarjeta de artículo:

   * Nombre del artículo con un vínculo directamente a la tarea
   * El nombre del proyecto con un vínculo directo al proyecto\
      Este vínculo solo se muestra al utilizar la vista ágil en una iteración; no se muestra al utilizar una vista Águila en un proyecto.
   * La descripción de la tarea
   * Compromiso actual
   * Ver y editar el porcentaje completado ajustando el porcentaje completado por sí mismo o ajustando el número de puntos u horas completadas
   * Usuarios asignados

   Puede mostrar datos adicionales (incluidos datos personalizados) en tarjetas de artículos. Es posible que desee mostrar campos adicionales en las tarjetas de artículo por varios motivos. Por ejemplo, es posible que desee mostrar el ID de cliente si está trabajando en artículos para varios clientes dentro del proyecto o que desee mostrar la Fecha de inicio de la tarea.

1. Haga clic en **Guardar**.\
   El acceso dicta cómo se guarda la vista. Si creó la vista originalmente, puede guardar los cambios; de lo contrario, se le pedirá que guarde una versión. Tenga en cuenta que los cambios que realice en la vista afectarán a los usuarios con los que se ha compartido la vista.

1. (Opcional) Haga clic en el **Vista de lista** icono ![](assets/list-view-in-agile-view-for-tasks.png) para volver a la lista de tareas.
