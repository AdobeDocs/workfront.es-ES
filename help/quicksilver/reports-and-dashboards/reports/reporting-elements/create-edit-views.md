---
product-area: reporting
navigation-topic: reporting-elements
title: Creación o edición de vistas en Adobe Workfront
description: Puede personalizar el tipo de información que se muestra en la pantalla mediante las vistas. Puede utilizar varios tipos de vistas en Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 8fcd6320-c939-4195-8972-5c31575f78cb
source-git-commit: d98998627ac5161fd12bb2d86f65555550c82a48
workflow-type: tm+mt
source-wordcount: '1721'
ht-degree: 84%

---

# Creación o edición de vistas en Adobe Workfront

<!-- Audited: 11/2024 -->

Puede personalizar el tipo de información que se muestra en la pantalla mediante las vistas. Puede utilizar varios tipos de vistas en Adobe Workfront.

En este artículo se describe cómo crear y editar vistas estándar para listas e informes, y cómo crear vistas de Agile. Para obtener más información, consulte [Información general sobre vistas en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Plan de Adobe Workfront</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Licencia de Adobe Workfront*</strong></td> 
   <td> 
      <p>Nuevo:</p>
         <ul>
         <li><p>Colaborador o superior</p></li>
         </ul>
      <p>Actual:</p>
         <ul>
         <li><p>Solicitud o superior</p></li>
         </ul>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuraciones de nivel de acceso*</strong></td> 
   <td> <p>Acceso de edición a filtros, vistas y agrupaciones</p> <p>Editar el acceso a Informes, Tableros y Calendarios para crear una vista en un informe</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto*</strong></td> 
   <td> <p>Gestionar permisos de un informe para crear o editar una vista en un informe</p> <p>Permisos de administración de una vista para editarla</p>
   </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación o personalización de una vista

El proceso de creación o personalización de una vista varía en función de si está creando o personalizando una vista estándar o una vista de Agile.

* [Crear o personalizar una vista estándar](#create-or-customize-a-standard-view)
* [Crear o personalizar una vista de Agile](#create-or-customize-an-agile-view)

### Creación o personalización de una vista estándar {#create-or-customize-a-standard-view}

Puede crear una nueva vista estándar o personalizar una vista estándar existente que haya creado anteriormente.

1. Haga clic en el menú desplegable **Vista** en cualquier lista donde quiera crear o personalizar una vista.

1. Haga clic en el botón **+ Nueva vista** para crear una vista nueva.
O
Haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png) que aparece al pasar el ratón a la derecha de la vista existente que desee editar.
Se muestra el cuadro de diálogo **Personalizar vista**.

1. En la sección **Vista previa de columna**, realice una de las acciones siguientes:

   * Modifique el valor de cualquier columna haciendo clic en el título de la columna y seleccionando un nuevo campo.
   * Añada una columna haciendo clic en **Añadir columna**, empiece a escribir el nombre de la columna que desea añadir y, a continuación, haga clic en ella cuando aparezca en la lista desplegable.
   * Ajuste el orden en que aparecen las columnas arrastrando el título de la columna a una nueva ubicación.

   * En el área **Configuración de columna**, haga clic en **Resumir esta columna por** y elija cómo desea que se muestren los datos en la columna. Esta opción está disponible para los siguientes tipos de columna:

     <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Campos de fecha</strong></td> 
           <td><ul>
           <li>Máximo</li>
         <li>Mínimo</li>
           </ul></td> 
          </tr> 
          <tr>
           <td role="rowheader"><strong>Campos de moneda</strong></td> 
           <td><ul>
           <li>Cuenta</li>
         <li>Suma</li>
           <li>Promedio</li>
         <li>Máximo</li>
           <li>Mínimo</li>
         </ul></td> 
          </tr> 
         <tr>
           <td role="rowheader"><strong>Campos booleanos y de cadena</strong></td> 
           <td><ul><li>Cuenta</li></ul>
           <p>Nota: Workfront no suele recomendar el resumen de un campo booleano por recuento, ya que el valor siempre será true/false.</p></td> 
          </tr> 
         </tbody> 
        </table>

     >[!NOTE]
     >
     >Las siguientes excepciones se aplican a los objetos principales (por ejemplo, las tareas principales) cuando se resumen los valores de los siguientes campos en las agrupaciones:
     >   
     > * Todos los campos de número y moneda excepto Horas reales (por ejemplo, Costo de mano de obra planificado/ real, Costo de gasto planificado/ real, Costo planificado/ real, Horas planificadas) resumen los valores solo para tareas secundarias y tareas independientes. No resumen los valores de las tareas padre o padre de los padres.
     > * Horas reales resume los valores de las tareas principales e independientes; no resume los números de las tareas principales o secundarias.
     > * Los campos de datos personalizados para valores numéricos y monetarios resumen todas las tareas: padres, hijos, padres de padres y tareas independientes.
     >
     >Para obtener más información acerca del uso de agrupaciones en un informe, consulte el artículo [Información general sobre agrupaciones en Adobe Workfront](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md).

      * (Opcional) Haga clic en **Opciones avanzadas** para especificar la siguiente información para la columna:

        <table style="table-layout:auto"> 
         <col> 
         <col> 
         <tbody> 
          <tr> 
           <td role="rowheader"><strong>Etiqueta personalizada de columna</strong></td> 
           <td><p>Especifique una etiqueta personalizada para la columna. Esta etiqueta reemplaza la etiqueta predeterminada. Se recomienda utilizar solo caracteres UTF-8 para evitar problemas de compatibilidad.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Formato de campo</strong></td> 
           <td>Seleccione el formato en el que desea que se muestren los valores de los campos de la columna.</td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Mostrar esta columna en panel de control</strong></td> 
           <td><p>Seleccione esta opción para mostrar esta columna en un panel de control cuando el informe se muestre en paralelo con otro informe. Cuando esta opción no está seleccionada, esta columna no se muestra al ver el informe en un panel en el que los informes se muestran uno al lado del otro.</p></td> 
          </tr> 
          <tr> 
           <td role="rowheader"><strong>Reglas de columna</strong></td> 
           <td><p>Haga clic en <strong>+ Agregar una regla para esta columna</strong> para definir una regla para la columna. Después de añadir una regla, puede definir estilos de campo y de texto para ver cómo se muestran los campos que coinciden con esa regla. Haga clic en <strong>Añadir regla</strong> después de haber terminado de definir la regla.</p></td> 
          </tr> 
         </tbody> 
        </table>

        Para obtener más información acerca del formato condicional de vistas en los informes, consulte el artículo [Usar formato condicional en el modo de texto](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

1. (Condicional) Si ha hecho clic en **Opciones avanzadas**, haga clic en **Listo**.

1. Haga clic en **Guardar vista** para crear una vista nueva o para reemplazar la vista actual con los cambios.\
   O\
   Haga clic en **Guardar como nueva vista** para guardar los cambios como una vista nueva.

   >[!TIP]
   >
   >**Guardar como nueva vista** es la única opción disponible al personalizar una vista integrada de Workfront.

   Su acceso dicta cómo se guarda la vista. Si ha creado la vista originalmente, puede guardar los cambios; de lo contrario, se le pedirá que guarde una versión. Tenga en cuenta que los cambios que realice en la vista afectan a los usuarios con los que se ha compartido la vista.

### Crear o personalizar una vista de Agile {#create-or-customize-an-agile-view}

Puede crear una vista de Agile o personalizar una existente que haya creado anteriormente.

>[!IMPORTANT]
>
>Las vistas de Agile solo están disponibles cuando se visualiza un proyecto.

Para obtener más información acerca de las vistas de Agile, consulte el artículo [Administrar un proyecto en la vista de Agile](../../../manage-work/projects/manage-projects/manage-projects-in-agile-view.md).

>[!NOTE]
>
>Este procedimiento solo se aplica a la vista de Agile heredada, no a la vista de tablero de un proyecto.

Para crear o personalizar una vista de Agile, haga lo siguiente:

1. Vaya a la lista de tareas de un proyecto.
1. Haga clic en el icono **Tablero** ![Icono Tablero](assets/board-icon-for-agile-view.png) y, a continuación, haga clic en **Utilizar el legado de Agile** en la vista del tablero.

1. (Condicional) Para personalizar una vista de Agile existente, haga lo siguiente:

   1. Haga clic en el menú desplegable **Vista** y, a continuación, seleccione la vista de Agile que desee personalizar.\
      No se puede personalizar la vista de Agile predeterminada.

   1. Vuelva a hacer clic en el menú desplegable **Vista** y, a continuación, haga clic en **Personalizar vista**.\
      ![Personalizar vista](assets/view-agile-customize.png)

1. (Condicional) Para crear una nueva vista de Agile, haga clic en **Nueva vista**.\
   Se muestra el cuadro de diálogo **Personalizar vista de Agile**.

1. En el cuadro de diálogo **Personalizar vista de Agile**, especifique un nombre para esta.\
   Se recomienda incluir la palabra “Agile” en el nombre de la vista para que los usuarios sepan que se trata de una vista de Agile.\
   Este nombre se muestra en el menú desplegable **Vista** al seleccionar una vista.

1. Defina las columnas de estado para mostrar en el tablero de historia en la vista de Agile. Estos son los estados de tareas definidos por el administrador de Workfront, tal como se describe en [Crear o editar un estado](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md).

   Solo los estados del sistema están disponibles para su uso en el tablero de historia de Agile. Si un estado solo está disponible para un grupo individual al que pertenece, el estado no estará disponible en el tablero de historia de Agile. Además, las tareas que se encuentran en un estado que solo está disponible para un grupo personalizado no son visibles cuando se visualiza el proyecto en una vista de Agile.

   Los usuarios pueden mover historias entre estas columnas de estado en el tablero de historias de Agile.\
   Cuando vaya a definir columnas de estado, puede hacer lo siguiente:

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
      <td>Haga clic en el icono (x) de la columna que desee quitar.<br>No puede quitar el estado "Nuevo" a menos que se haya añadido un estado personalizado a la vista y que ese estado personalizado sea igual a "Nuevo".<br>Para obtener información sobre la creación de un estado personalizado, consulte <a href="../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-or-edit-a-status.md" class="MCXref xref">Crear o editar un estado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Añadir columnas de estado:</strong> </td> 
      <td> <p>Haga clic en el icono de <strong>Más</strong> y, a continuación, seleccione el estado que desee añadir.<br>Se muestran todos los estados predeterminados del sistema, así como todos los estados personalizados que se han compartido con usted.<br>Puede configurar hasta 10 estados para mostrar.</p></td> 
     </tr> 
    </tbody> 
   </table>

   <!--
        <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE FOR ADD STATUS COLUMNS: research this and add: [! What if the status has been shared with me or a group I'm in (so I can see it here), but the status hasn't been shared with another user who also has access to a project where I later apply this view? Can that user still see this status on the project?]) </p>
       -->

1. En el área **Asociar el color de tarjeta con**, seleccione una de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col>
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>Historia:</strong> </td> 
      <td>Cualquier subtarea coincide con el color de la tarea principal, de modo que los colores de todas las historias de cualquier carril especificado son los mismos.<br>Los colores se asignan aleatoriamente a las tareas cuando se crean si la tarea no tiene subtareas o no tiene una tarea principal.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Forma libre:</strong> </td> 
      <td> Todas las tarjetas se muestran en azul de forma predeterminada hasta que un usuario cambie el color manualmente, tal como se describe en el artículo <a href="../../../agile/use-scrum-in-an-agile-team/scrum-board/categorize-stories-by-color.md" class="MCXref xref">Clasificar las historias por el color en el tablero de Scrum</a>. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Prioridad:</strong> </td> 
      <td> <p> Los colores se asocian a la prioridad de la historia de la siguiente manera:</p> 
       <ul> 
        <li>Alta = Rojo</li> 
        <li>Media = Amarillo</li> 
        <li>Baja = Verde<br>Si el administrador de Workfront ha configurado prioridades personalizadas para su sistema Workfront, la prioridad más alta es de color rojo, la segunda más alta es amarilla y las restantes son verdes.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>Propietario de la tarea:</strong> </td> 
      <td> Todas las historias con la misma persona principal asignada son del mismo color.<br>La persona asignada principal es el usuario que se asignó por primera vez a la tarea. </td> 
     </tr> 
    </tbody> 
   </table>

1. En el área **Campos adicionales**, haga clic en **Agregar campo** y, a continuación, seleccione el campo que desee agregar a las tarjetas de historia. (Son los mismos campos que puede añadir al crear, personalizar una vista o crear columnas para un informe).\
   Repita este proceso para añadir hasta tres campos adicionales a las tarjetas de la historia.\
   Cuando se añaden campos a las tarjetas de historia, los campos se muestran cuando se rellena el campo y son de solo lectura.

   De forma predeterminada, los siguientes tipos de datos se muestran en la tarjeta de la historia:

   * Nombre de la historia con un vínculo directamente a la tarea
   * El nombre del proyecto con un vínculo directamente al proyecto\
     Este vínculo solo se muestra cuando se utiliza la vista de Agile en una iteración; no se muestra cuando se utiliza una vista de Agile en un proyecto.
   * La descripción de la tarea
   * Compromiso actual
   * Vea y edite el porcentaje completado ajustando el porcentaje completado en sí o ajustando el número de puntos u horas que se han completado
   * Usuarios asignados

   Se pueden mostrar datos adicionales (incluidos datos personalizados) en las tarjetas de historias. Es posible que desee mostrar campos adicionales en las tarjetas de historias por varios motivos. Por ejemplo, es posible que desee mostrar el identificador del cliente si está trabajando en historias para varios clientes dentro del proyecto o puede que desee mostrar la fecha de inicio de la tarea.

1. Haga clic en **Guardar**.\
   Su acceso dicta cómo se guarda la vista. Si ha creado la vista originalmente, puede guardar los cambios; de lo contrario, se le pedirá que guarde una versión. Tenga en cuenta que los cambios que realice en la vista afectan a los usuarios con los que se ha compartido la vista.

1. (Opcional) Haga clic en el icono de **Lista** para regresar a la lista de tareas.
