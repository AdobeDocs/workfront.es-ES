---
title: Creación de jerarquías de Workspace
description: Como administrador de espacio de trabajo, puede crear varias jerarquías de espacio de trabajo entre los tipos de registro en Adobe Workfront Planning. Después de conectar los tipos de registro en un espacio de trabajo y crear una jerarquía, los tipos de registro se conectan entre sí, con un tipo de registro designado como principal y hasta 6 tipos de registro más configurados como secundarios.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: 6aba4316228a320cf33e419249a64b3cf56e8f39
workflow-type: tm+mt
source-wordcount: '662'
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

Como administrador de espacio de trabajo, puede crear varias jerarquías de espacio de trabajo entre los tipos de registro en Adobe Workfront Planning.


Una vez que los tipos de registros están conectados en un espacio de trabajo, puede crear una jerarquía que organice esas conexiones. Las jerarquías organizan los tipos de registros en relaciones principal-secundario y pueden contener hasta cuatro niveles de tipos de objetos.

Si todavía no existe una conexión entre dos tipos de registro, se puede crear a medida que se configura la jerarquía. Una vez definida, la jerarquía establece una ruta estructurada entre los tipos de registros relacionados dentro del espacio de trabajo.

Las jerarquías generarán rutas de exploración para los tipos de registros y los registros <!--ensure this is the case: does the breadcrumb show for both the RT and the record??--> que se muestran en sus encabezados. De este modo, los usuarios saben dónde se encuentran en la jerarquía en cualquier fase del flujo de trabajo.

Para obtener información general acerca de jerarquías y rutas de exploración, vea [Información general sobre jerarquías y rutas de exploración](/help/quicksilver/planning/architecture/hierarchy-and-breadcrumb-overview.md).

## Requisitos de acceso

<!--check the access to see if you oversimplified???-->

<!--Update the TOC for this to publish-->

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
1. Haga clic en **Agregar objeto** y seleccione un objeto en el menú desplegable. Va a ser el primer objeto principal de la jerarquía.
El primer elemento principal sólo puede ser un tipo de registro de Planning. Los proyectos de Workfront no se pueden seleccionar como principales de otros tipos de objeto en una jerarquía.
1. Haga clic en **Agregar objeto** para agregar un segundo objeto, que es el primer elemento secundario de la jerarquía, y luego seleccione otro objeto en el menú desplegable.
   ![Nuevo cuadro de jerarquía sin campo seleccionado](assets/new-hierarchy-modal-without-connecte-fielf-selected.png)
1. Haga clic en **Seleccionar campo conectado** para indicar qué campo conecta los dos objetos.
1. (Condicional) Si existe un campo conectado entre los dos tipos de objeto, selecciónelo en la lista. De lo contrario, haga clic en **Agregar nueva conexión**.

   >[!WARNING]
   >
   >Si el **campo Crear correspondiente en el tipo de registro vinculado** no se seleccionó cuando se creó el campo conectado, debe editar primero el campo para poder continuar.

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
Para obtener más información, vea [Conectar tipos de registros](/help/quicksilver/planning/architecture/connect-record-types.md).
   1. Haga clic en **Guardar**.
1. (Opcional) Siga agregando hasta 4 tipos de objetos a las jerarquías siguiendo los pasos anteriores. Puede agregar primero todos los tipos de objetos y, a continuación, agregar los campos de conexión entre ellos.
1. (Opcional) Haga clic en el icono **Quitar** ![Quitar icono](assets/minus-icon.png) para quitar una conexión.
1. Haga clic en **Guardar** para guardar la jerarquía.

   >[!TIP]
   >
   >El botón **Guardar** aparece atenuado si no dispone de todos los campos conectados.

   Ocurren lo siguiente:

   * La jerarquía se agrega a la sección **Jerarquías** del área de trabajo.
   * Los registros que rellenan los campos de conexión muestran todas las conexiones en sus rutas de exploración, cuando va a la página de un registro.
1. (Opcional) Pase el ratón sobre una jerarquía, haga clic en el menú **Más** y, a continuación, haga clic en una de las siguientes opciones:

   * **Editar**: Se abre el cuadro **Editar jerarquía** donde puede realizar cambios.
   * **Eliminar**: Esto elimina la jerarquía de forma permanente. Las jerarquías eliminadas no se pueden recuperar. Los campos de conexión no se eliminan.





