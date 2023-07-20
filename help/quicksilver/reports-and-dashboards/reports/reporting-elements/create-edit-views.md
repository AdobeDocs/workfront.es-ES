---
product-area: reporting
navigation-topic: reporting-elements
title: Creación o edición de vistas en Adobe Workfront
description: Puede personalizar el tipo de información que se muestra en la pantalla mediante las vistas. Puede utilizar varios tipos de vistas en Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: a4ccd48956fedbafc04ce19198592efdad49e5a3
workflow-type: tm+mt
source-wordcount: '1777'
ht-degree: 1%

---

# Creación o edición de vistas en Adobe Workfront

Puede personalizar el tipo de información que se muestra en la pantalla mediante las vistas. Puede utilizar varios tipos de vistas en Adobe Workfront.

En este artículo se describe cómo crear y editar vistas estándar para listas e informes, y cómo crear vistas de Agile. Para obtener más información, consulte [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>plan Adobe Workfront*</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Editar acceso a filtros, vistas y agrupaciones</p> <p>Editar el acceso a Informes, Tableros y Calendarios para crear una vista en un informe</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Administración de permisos de un informe para crear o editar una vista de un informe</p> <p>Administrar permisos a una vista para editarla</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Creación o personalización de una vista

El proceso de creación o personalización de una vista varía en función de si está creando o personalizando una vista estándar o una vista Agile.

* [Creación o personalización de una vista estándar](#create-or-customize-a-standard-view)
* [Creación o personalización de una vista de Agile](#create-or-customize-an-agile-view)

### Creación o personalización de una vista estándar {#create-or-customize-a-standard-view}

Puede crear una nueva vista estándar o personalizar una vista estándar existente que haya creado anteriormente.

1. Haga clic en **Ver** menú desplegable de cualquier lista en la que desee crear o personalizar una vista.
1. (Opcional) Para personalizar una vista existente, seleccione la vista estándar que desee personalizar.\
   Las vistas estándar están disponibles en cualquier tipo de lista de Workfront, como un informe, una lista de proyectos o una lista de tareas.
1. Haga clic en **Ver** y, a continuación, haga clic en **Personalizar vista** o **Nueva vista**.\
   El **Personalizar vista** aparece el cuadro de diálogo.

1. En el **Previsualización de columna** , realice una de las siguientes acciones:

   * Modifique el valor de cualquier columna haciendo clic en el título de la columna y seleccionando un nuevo campo.
   * Añada una columna haciendo clic en **Agregar columna**, empiece a escribir el nombre de la columna que desea agregar y, a continuación, haga clic en ella cuando aparezca en la lista desplegable.
   * Ajuste el orden en que aparecen las columnas arrastrando el título de la columna a una nueva ubicación.

      * (Opcional) En el **Configuración de columna** , haga clic en el **Resumir esta columna por** y, a continuación, seleccione una de las opciones disponibles para resumir la información. Al elegir esta opción, la información de la columna se agrega a las agrupaciones del informe.\
        Para los campos de fecha, puede resumir los valores mediante las siguientes opciones:

         * Máximo
         * Mínimo

        Para los campos de número y moneda, puede resumir los valores mediante las siguientes opciones:

         * Cuenta
         * Suma
         * Promedio
         * Máximo
         * Mínimo

        >[!NOTE]
        >
        >Las siguientes excepciones se aplican a los objetos principales (por ejemplo, las tareas principales) cuando se agregan valores para los siguientes campos en agrupaciones:
        >   
        >   * Todos los campos de número y moneda excepto Horas reales (por ejemplo, Costo de mano de obra planificado/ real, Costo de gasto planificado/ real, Costo planificado/ real, Horas planificadas) agregan solo los valores de las tareas secundarias y las tareas independientes. No acumulan los valores de las tareas principales o principales de los elementos principales.
        >   * Las horas reales acumulan los valores de las tareas principales e independientes; no acumulan los números de las tareas principales o secundarias.
        >   * Los campos de datos personalizados para valores numéricos y monetarios acumulan todas las tareas: principales, secundarios, principales de principales y tareas independientes.
        >   
        >

        Para obtener más información sobre el uso de agrupaciones en un informe, consulte el artículo [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

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
           <td>Seleccione el formato en el que desea que se muestren los valores de los campos de la columna.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Mostrar esta columna en panel</strong></td> 
           <td><p>Seleccione esta opción para mostrar esta columna en un panel cuando el informe se muestre en paralelo con otro informe. Cuando esta opción no está seleccionada, esta columna no se muestra al ver el informe en un panel en el que los informes se muestran uno al lado del otro.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Reglas de columna</strong></td> 
           <td><p>Clic <strong>Agregar una regla para esta columna</strong> para definir una regla para la columna. Después de agregar una regla, puede definir estilos de campo y de texto para ver cómo se muestran los campos que coinciden con esa regla. Clic <strong>Agregar regla</strong> una vez que haya terminado de definir la regla.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Para obtener más información sobre el formato condicional de vistas en los informes, consulte el artículo [Uso del formato condicional en el modo Texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Condicional) Si hizo clic en **Opciones avanzadas**, haga clic en **Listo**.

1. Clic **Guardar vista** para crear una vista nueva o para reemplazar la vista actual con los cambios.\
   O\
   Clic **Guardar como nueva vista** para guardar los cambios como una nueva vista.

   >[!TIP]
   >
   >El **Guardar como nueva vista** es la única opción disponible al personalizar una vista integrada de Workfront.

   Su acceso dicta cómo se guarda la vista. Si creó la vista originalmente, puede guardar los cambios; de lo contrario, se le pedirá que guarde una versión. Tenga en cuenta que los cambios que realice en la vista afectan a los usuarios con los que se ha compartido la vista.

### Creación o personalización de una vista de Agile {#create-or-customize-an-agile-view}

Puede crear una nueva vista de Agile o personalizar una vista de Agile existente que haya creado anteriormente.

>[!IMPORTANT]
>
>Las vistas de Agile solo están disponibles cuando se visualiza un proyecto.

Para obtener más información sobre las vistas de Agile, consulte el artículo [Administrar un proyecto en la vista de Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

>[!NOTE]
>
>Este procedimiento solo se aplica a la vista de Agile heredada, no a la vista de tablero de un proyecto.

Para crear o personalizar una vista de Agile:

1. Ir a la lista de tareas de un proyecto.
1. Haga clic en **Tablero** icono ![Icono de tablero](assets/board-icon-for-agile-view.png)y haga clic en **Usar Agile heredado** en la vista del tablero.

1. (Condicional) Para personalizar una vista de Agile existente:

   1. Haga clic en **Ver** menú desplegable y, a continuación, seleccione la vista de Agile que desee personalizar.\
      No se puede personalizar la vista de Agile predeterminada.

   1. Haga clic en **Ver** menú desplegable de nuevo y haga clic en **Personalizar vista**.\
      ![](assets/view-agile-customize.png)

1. (Condicional) Para crear una nueva vista de Agile, haga clic en **Nueva vista**.\
   El **Personalizar vista de Agile** aparece el cuadro de diálogo.

1. En el **Personalizar vista de Agile** , especifique un nombre para la vista de Agile.\
   Se recomienda incluir la palabra &quot;Agile&quot; en el nombre de la vista para que los usuarios sepan que se trata de una vista Agile.\
   Este nombre se muestra en la variable **Ver** menú desplegable al seleccionar una vista.

1. Defina las columnas de estado para mostrar en el guion gráfico en la vista Agile. Estos son los estados de tareas definidos por el administrador de Workfront, tal como se describe en [Creación o edición de un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Solo los estados del sistema están disponibles para su uso en el panel de historia de Agile. Si un estado solo está disponible para un grupo individual al que pertenece, el estado no estará disponible en el panel de historias Agile. Además, las tareas que están en un estado que solo está disponible para un grupo personalizado no están visibles al ver el proyecto en una vista de Agile.

   Los usuarios pueden mover historias entre estas columnas de estado en el panel de historias de Agile.\
   Al definir las columnas de estado, puede hacer lo siguiente:

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
      <td>Haga clic en el icono (x) de la columna que desee eliminar.<br>No puede quitar el estado "Nuevo" a menos que se haya agregado un estado personalizado a la vista y ese estado personalizado sea igual a "Nuevo".<br>Para obtener información sobre cómo crear un estado personalizado, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Creación o edición de un estado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Agregar columnas de estado:</strong> </td> 
      <td> <p>Haga clic en <strong>Plus</strong> y, a continuación, seleccione el estado que desee añadir.<br>Se muestran todos los estados predeterminados del sistema, así como todos los estados personalizados que se han compartido con usted.<br>Puede configurar hasta 10 estados para mostrarlos.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. En el **Asociar el color de la tarjeta con** , seleccione entre las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Historia:</strong> </td> 
      <td>Cualquier subtarea coincide con el color de la tarea principal, de modo que los colores de todas las historias de cualquier carril de baño dado son los mismos.<br>Los colores se asignan aleatoriamente a las tareas cuando se crean si la tarea no tiene subtareas o no tiene una tarea principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Forma libre:</strong> </td> 
      <td> Todas las tarjetas se muestran en azul de forma predeterminada hasta que un usuario cambia el color manualmente, tal como se describe en el artículo <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Categorizar historias por color en el panel Scrum</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridad:</strong> </td> 
      <td> <p> Los colores se asocian a la prioridad del artículo de la siguiente manera:</p> 
       <ul> 
        <li>Alto = Rojo</li> 
        <li>Medio = Amarillo</li> 
        <li>Baja = Verde<br>Si el administrador de Workfront ha configurado prioridades personalizadas para su sistema de Workfront, la prioridad más alta es roja, la segunda es amarilla y las restantes son verdes.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Propietario de tarea:</strong> </td> 
      <td> Todas las historias con el mismo usuario principal asignado son del mismo color.<br>El usuario asignado principal es el usuario que se asignó por primera vez a la tarea. </td> 
     </tr> 
    </tbody> 
   </table>

1. En el **Agile** , en la sección **Campos adicionales** , haga clic en **Añadir campo**, luego seleccione el campo que desee agregar a las tarjetas de historia. (Son los mismos campos que puede agregar al crear, personalizar una vista o crear columnas para un informe).\
   Repita este proceso para agregar hasta tres campos adicionales a las tarjetas de historia.\
   Cuando se agregan campos a las tarjetas de historia, los campos son de sólo lectura y sólo se muestran cuando se rellena el campo.

   De forma predeterminada, los siguientes tipos de datos se muestran en la tarjeta de historia:

   * Nombre de la historia con un vínculo directamente a la tarea
   * El nombre del proyecto con un vínculo directamente al proyecto\
     Este vínculo solo se muestra cuando se utiliza la vista Agile en una iteración; no se muestra cuando se utiliza una vista Agile en un proyecto.
   * Descripción de la tarea
   * Compromisos actuales
   * Vea y edite el porcentaje completado ajustando el porcentaje completado en sí o ajustando el número de puntos u horas que se han completado
   * Usuarios asignados

   Puede mostrar datos adicionales (incluidos datos personalizados) en tarjetas de historia. Es posible que desee mostrar campos adicionales en las tarjetas de historia por varios motivos. Por ejemplo, es posible que desee mostrar el ID de cliente si está trabajando en historias para varios clientes dentro del proyecto o puede que desee mostrar la fecha de inicio de la tarea.

1. Haga clic en **Guardar**.\
   Su acceso dicta cómo se guarda la vista. Si creó la vista originalmente, puede guardar los cambios; de lo contrario, se le pedirá que guarde una versión. Tenga en cuenta que los cambios que realice en la vista afectan a los usuarios con los que se ha compartido la vista.

1. (Opcional) Haga clic en **Lista** para volver a la lista de tareas.
