---
title: Agregar una página de registros conectados a un registro
description: Puede ver información de registros u objetos conectados agregando una ficha para una página Registros conectados a un registro. Esto agrega los registros conectados en una vista de tabla a la ficha.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 48bfeb3b950ca1149a919aa204d77db6aa501e01
workflow-type: tm+mt
source-wordcount: '1139'
ht-degree: 4%

---


# Agregar una página Registros conectados a un registro

Puede ver información de registros u objetos conectados agregando una ficha para una página Registros conectados a un registro. Esto agrega los registros conectados en una vista de tabla a la ficha.

Tenga en cuenta lo siguiente al agregar una página Registros conectados a un registro:

* Puede agregar una página Registros conectados a un registro después de conectar tipos de registro u objeto al tipo de registro desde la vista de tabla de un tipo de registro.

* Puede agregar una página Registros conectados desde el área de vista previa de un registro o desde la página del registro.

* Las páginas Registros conectados muestran sólo los objetos o registros conectados de un tipo de objeto o registro en una vista de tabla. La página no muestra todos los registros de ese tipo.

* Puede agregar páginas Registros conectados para los siguientes tipos de registros u objetos conectados:

   * Tipos de registros de Workfront Planning
   * Proyectos, programas, portafolios, grupos o compañías de Workfront. Puede ver los objetos de Workfront conectados incluso cuando no tenga permisos para acceder a ellos en Workfront.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo. 

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
<p>Cualquier Workfront y cualquier paquete de Planning</p>
<p>Cualquier flujo de trabajo y cualquier paquete de Planning</p>
<p>Para obtener más información sobre lo que se incluye en cada paquete de Workfront Planning, póngase en contacto con su representante de cuentas de Workfront. </p> 
   </td> 
<tr>
<td> 
   <p> Productos adicionales</p> </td> 
   <td> 
   <p> Además de Adobe Workfront, debe tener lo siguiente si desea agregar una página de registro conectada para objetos de las siguientes aplicaciones:</p>
   <ul><li><p>Licencia de Adobe Experience Manager Assets e integración entre AEM Assets y Workfront para conectar recursos de AEM con tipos de registros de Planning.</p>
   <p>Para obtener más información, consulte <a href="/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/workfront-for-aem-asset-essentials.md">Adobe Workfront para Experience Manager Assets y Assets Essentials: índice de artículo</a>. </p></li>
   <li><p> Licencia de Adobe GenStudio for Performance Marketing para conectar tipos de registros con marcas de GenStudio</p>
   <p>Para obtener más información, consulte <a href="https://experienceleague.adobe.com/es/docs/genstudio-for-performance-marketing/user-guide/get-started">Introducción a Adobe GenStudio for Performance Marketing</a>.</p></li></ul>
   </td> 
  </tr>

<tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Estándar</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader"><p>Permisos de objeto</p></td>
   <td>
   <p>Permisos de contribución o superiores para un espacio de trabajo y tipo de registro </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p> 
  </td>
  </tr>   
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++   


## Agregar una página Registros conectados a un registro

1. Haga clic en el nombre del registro para abrirlo desde cualquier vista de una página de tipo de registro.
1. Haga clic en **Agregar página** en una de las siguientes áreas:

   * Ventana de vista previa del registro
   * La página de detalles del registro, después de hacer clic en el icono **Abrir en ficha nueva** ![Abrir detalles en icono de ficha nueva](assets/open-details-in-a-new-tab-icon.png) en la esquina superior derecha de la página de vista previa.

   Se abre el cuadro **Crear página**.

   ![Agregar página de registros conectados modal](assets/add-connection-view-page-modal.png)

1. Agregue **Nombre de página**, haga clic en **Página de registros conectados** y, a continuación, haga clic en **Crear**.

   Una nueva página de registros conectados se agrega como una nueva ficha a la página del registro.

   Los registros conectados al registro actual se muestran en la vista de tabla.

   >[!TIP]
   >
   >Debe agregar registros conectados en la tabla o en el área Detalles de un registro para poder mostrarlos en una página de registros conectados.

   <!--All fields of the connected record display in the table view of the connected record's tab.-->

   Los cinco primeros campos de los registros conectados se muestran de forma predeterminada. <!--No lookup fields display by default.-->

   ![Vista de tabla conectada a la audiencia con detalles de campaña](assets/audience-connected-table-view-under-campaign-details-page.png)

1. (Opcional) Busque o haga clic en el nombre de un tipo de objeto o registro conectado en la lista.

1. (Opcional y condicional) En la vista de tabla de la página de registros conectados, realice una de las siguientes acciones cuando visualice registros de Planning conectados o cualquier objeto de Workfront excepto los proyectos: <!--or AEM Assets--> <!--AEM is not available yet?? see note below-->

   * Haga clic en el nombre de un registro. Se abre la página del registro en una nueva ficha.

   * Haga clic en **Conectar** en la parte inferior de la vista de tabla para conectar más registros y, a continuación, haga clic fuera del cuadro de conexión para cerrarlo. Los registros nuevos se agregan automáticamente a la tabla.

     Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
   * Edite cualquier información de los registros conectados en línea en la vista de tabla.

   * Pase el ratón sobre el nombre de un registro conectado y luego haga clic en el menú **Más** ![Menú Más](assets/more-menu.png)

     O

     Seleccione uno de los registros y, a continuación, haga clic en una de las siguientes opciones de la barra azul situada en la parte inferior de la lista:

      * **Ver** para abrir la página de registros en una nueva pestaña
      * **Copiar vínculo** para copiar un vínculo a la página de registro
      * **Editar miniatura** para abrir el cuadro **Grabar miniatura** y editar la imagen en miniatura del registro
      * **Duplicate** para duplicar el registro conectado. El registro duplicado también está conectado al registro actual.
      * **Inserte un registro por encima o por debajo de** para agregar nuevos registros al tipo de registro conectado. Los registros nuevos agregados aquí también están conectados al registro actual. Esta opción no está disponible en la barra azul al seleccionar un registro de la tabla.
      * **Eliminar** para eliminar el registro. Al eliminar un registro conectado, se elimina de su tipo de registro y de cualquier lugar donde esté conectado.

     Para obtener información acerca de cómo editar registros en la vista de tabla, vea [Editar registros](/help/quicksilver/planning/records/edit-records.md).

     >[!TIP]
     >
     >Puede seleccionar más de un registro u objeto para eliminarlos.

   * Edite en línea cualquiera de los registros de Planning de la tabla de la página Registros conectados.

     El resto de los objetos de Workfront se muestran en una vista de tabla de solo lectura y no se pueden editar.

1. (Opcional y condicional) En la vista de tabla de la página de registros conectados, realice una de las siguientes acciones cuando visualice proyectos de Workfront conectados:

   * Haga clic en **Conectar registros** en la esquina superior derecha de la página de registros conectada para conectar proyectos existentes.

   Para obtener más información, consulte [Conectar registros](/help/quicksilver/planning/records/connect-records.md).
   * Editar en línea la información del proyecto en la tabla.
   * Haga clic en **Nueva fila** para crear un proyecto sin plantilla. El nuevo proyecto se conecta inmediatamente al registro actual.

     Para obtener más información, vea [Crear objetos de Workfront desde Workfront Planning a medida que los conecta a registros](/help/quicksilver/planning/records/create-workfront-objects-from-workfront-planning.md)
   * Pase el ratón sobre un proyecto y haga clic en el menú **Más** [Menú más](assets/more-menu.png)

     O

     Seleccione uno o varios proyectos, observe la barra azul en la parte inferior de la lista y, a continuación, haga clic en uno de los siguientes:

      * **Eliminar** para eliminar el proyecto. Al eliminar un proyecto, se desconecta del registro y se mueve a la papelera de reciclaje de Workfront.
      * **Desconectar** para desconectar el proyecto del registro. Al desconectar un proyecto, éste y todos los valores de sus campos de búsqueda se eliminan del registro actual.

1. (Opcional) Haga doble clic en el nombre de la ficha **Página de registros conectados**

   O

   Pase el ratón sobre el nombre de la ficha, luego haga clic en **Más** ![Menú más](assets/more-menu.png), luego haga clic en **Cambiar nombre** para cambiar el nombre a la nueva ficha Vista conectada.
1. (Opcional) Utilice cualquiera de los siguientes elementos de vista en la barra de herramientas de una página de registro conectada para administrar la vista de tabla:

   * Filtros
   * Ordenar
   * Agrupación
   * Campos, para mostrar, ocultar o reorganizar campos
   * Altura de la fila
   * Buscar

   Para obtener más información, consulte [Administrar la vista de tabla](/help/quicksilver/planning/views/manage-the-table-view.md).

   >[!NOTE]
   >
   >No puede crear, editar ni eliminar campos en la vista de tabla de la ficha de un registro conectado.

1. (Opcional) Pase el ratón sobre el nombre de la ficha de la página Registros conectados, haga clic en **Más** ![Menú más](assets/more-menu.png) y, a continuación, haga clic en **Eliminar** para quitar a la ficha.