---
title: Creación de jerarquías de Workspace
description: Como administrador de espacio de trabajo, puede crear varias jerarquías de espacio de trabajo entre los tipos de registro en Adobe Workfront Planning. Después de conectar los tipos de registro en un espacio de trabajo y crear una jerarquía, los tipos de registro se conectan entre sí, con un tipo de registro designado como principal y hasta 6 tipos de registro más configurados como secundarios.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: f1e945ca2508fc7ae1feaa5e97677458d175212f
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 4%

---

<!--update the metadata with real information when making this available in TOC and in the left nav:

---
title: Create Workspace Hierarchies
description: You can create multiple workspace hierarchies between the record types in a workspace. 
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
hide: yes 
hidefromtoc: yes 
---

-->

# Crear jerarquías de Workspace

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Como administrador de espacio de trabajo, puede crear varias jerarquías de espacio de trabajo entre tipos de registro en Adobe Workfront Planning.

Una vez que los tipos de registros están conectados en un espacio de trabajo, puede crear una jerarquía que organice esas conexiones. Las jerarquías organizan los tipos de registros y objetos en relaciones principal-secundario y pueden contener hasta cuatro niveles de tipos de objetos.

Si todavía no existe una conexión entre dos tipos de registro, se puede crear a medida que se configura la jerarquía. Una vez definida, la jerarquía establece una ruta estructurada entre los tipos de registros relacionados dentro del espacio de trabajo.

Las jerarquías generarán rutas de exploración para los tipos de registro y sus registros respectivos <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> que se muestran en sus encabezados. De este modo, los usuarios saben dónde se encuentran en la jerarquía en cualquier fase del flujo de trabajo.

Para obtener información general acerca de jerarquías y rutas de exploración, vea [Información general sobre jerarquías y rutas de exploración](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Requisitos de acceso

<!--check the access to see if you oversimplified???-->

+++ Expanda para ver los requisitos de acceso para realizar los pasos de este artículo:  

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
    <tr> 
<tr> 
</tr>   
<tr> 
   <td role="rowheader"><p>Paquete de Adobe Workfront</p></td> 
   <td> 
<ul> 
<li><p>Cualquier Workfront y cualquier paquete de Planning</p></li>
O
<li><p>Cualquier flujo de trabajo y cualquier paquete de Planning</p></li></ul>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en un espacio de trabajo</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de una jerarquía de Workspace

{#step1-to-planning}

1. Haga clic en una tarjeta de Workspace.
1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del área de trabajo y, a continuación, haga clic en **Configuración**.
La sección **Jerarquías** se abre de manera predeterminada.
1. Haga clic en **Nueva jerarquía** en la esquina superior derecha de la página **Jerarquías**.
1. Haga clic en **Agregar objeto** y seleccione un tipo de objeto en el menú desplegable. Va a ser el primer tipo de objeto de la jerarquía. <!--logged bug to correct to "Add object type"-->

   El primer tipo de objeto sólo puede ser un tipo de registro de Planning.

   Los proyectos de Workfront no se pueden seleccionar como principales de otros tipos de objeto en una jerarquía.

1. Haga clic en **Agregar objeto** para agregar un segundo tipo de objeto, que es el primer elemento secundario de la jerarquía, y después seleccione otro tipo de objeto en el menú desplegable.
Cada tipo de objeto adicional se convierte en secundario de los tipos de objeto anteriores.

   ![Nuevo cuadro de jerarquía sin campo seleccionado](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)

1. Haga clic en **Seleccionar campo conectado** para indicar qué campo conecta los dos objetos.
1. (Condicional) Si hay varios campos de conexión, seleccione uno en la lista,

   O

   Haga clic en **Agregar nueva conexión** para agregar un nuevo campo de conexión.

   Esto crea un campo de conexión a partir del tipo de registro que está utilizando como principal y un campo de conexión correspondiente a él desde el tipo de registro que está utilizando como secundario.

   Si está creando una conexión con proyectos de Workfront, no se crea ningún campo en el proyecto.

1. (Condicional) Si no hay campos conectados disponibles, haga clic en **Crear conexión**, agregue una nueva conexión y haga clic en **Guardar**.

1. (Condicional) Si va a agregar una nueva conexión, haga lo siguiente:

   1. Agregue un nombre para el campo conectado en el cuadro **Nombre**.
   1. Seleccione entre los siguientes tipos de conexión:

      * **Varios a varios**
      * **Uno a varios**
      * **Varios a uno**
      * **Uno a uno**

   1. Seleccione uno de los siguientes tipos de apariciones de registros:

      * **Nombre e imagen**
      * **Nombre**
      * **Imagen**

      Para obtener más información, consulte [Conectar tipos de registro](/help/quicksilver/planning/architecture/connect-record-types.md).

   1. Haga clic en **Guardar**.

1. (Condicional) Si el campo **Crear correspondiente en el tipo de registro vinculado** no se seleccionó cuando se creó el campo conectado, se producirá un error y deberá hacer lo siguiente primero: <!--check back on these steps; this is supposed to be seamless, but now you have to abandon creating a hierarchy to do this-->

   1. Haga clic en **Cancelar** en el cuadro **Nueva jerarquía**.
   1. Haga clic en la flecha hacia atrás situada a la izquierda del nombre del espacio de trabajo y, a continuación, haga clic en la tarjeta del tipo de registro que desee elegir como principal.
   1. Abra la vista de tabla del tipo de registro seleccionado en el paso anterior, vaya al campo de conexión con el tipo de objeto que desea utilizar como secundario, pase el ratón sobre el encabezado de la columna y, a continuación, haga clic en el campo **Editar**.
   1. Active la configuración **Crear campo correspondiente en el tipo de registro vinculado** y, a continuación, haga clic en **Guardar**.
   1. Vuelva al área **Configuración** del área de trabajo y haga clic de nuevo en **Nueva jerarquía**; a continuación, siga los pasos para crear una jerarquía.

1. (Opcional) Siga agregando hasta 4 tipos de objetos a las jerarquías siguiendo los pasos anteriores. Puede agregar primero todos los tipos de objetos y, a continuación, agregar los campos de conexión entre ellos.
1. (Opcional) Haga clic en el icono **Quitar** ![Quitar icono](assets/minus-icon.png) para quitar una conexión.
1. Haga clic en **Guardar** para guardar la jerarquía.

   >[!TIP]
   >
   >El botón **Guardar** aparece atenuado si no dispone de todos los campos conectados.

   Ocurren lo siguiente:

   * La jerarquía se agrega a la sección **Jerarquías** del área de trabajo.
   * Los registros que rellenan los campos de conexión muestran todas las conexiones en sus rutas de exploración, cuando va a la página de un registro.
1. (Opcional) Pase el ratón sobre una jerarquía y luego haga clic en el menú **Más**.

   ![Menú Más de jerarquía expandido](assets/hierarchy-more-menu-expanded.png)

1. Haga clic en una de las siguientes opciones:

   * **Editar**: Se abre el cuadro **Editar jerarquía** donde puede realizar cambios.
   * **Eliminar**: Esto elimina la jerarquía de forma permanente. Las jerarquías eliminadas no se pueden recuperar. Los campos de conexión no se eliminan.





