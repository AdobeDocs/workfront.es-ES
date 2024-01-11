---
title: Conectar tipos de registros
description: Una manera de indicar cómo se relacionan los tipos de registros individuales entre sí es conectarlos. Además, puede conectar los tipos de registros de Maestro con los tipos de objetos de otras aplicaciones para mejorar la experiencia de los usuarios y mantener el enfoque en una aplicación.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: ae794ebe-4597-47a4-9ef3-3f4d31cb70c2
source-git-commit: ce015eba8291995eec1611917896a0e797f820cc
workflow-type: tm+mt
source-wordcount: '2051'
ht-degree: 0%

---

<!-----
title: Connect record types
description: A way to indicate how individual record types relate to one another is to connect them. Also, you can connect Maestro record types with object types from other applications to enhance your users' experience and keep their focus in one application.
hidefromtoc: yes
hide: yes
feature: Work management
role: User
author: Alina
--->

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->
<!--************ THIS MIGHT NO LONGER BE A 'RELATIONSHIP' TYPE FIELD, BECAUSE THEY WILL SHOW IT IN THE CONNECTION TAB*****************************-->


# Conectar tipos de registros

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Maestro, que es una nueva oferta de Adobe Workfront.
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes. Debe ser cliente de Workfront para utilizar las funciones de Maestro.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Puede utilizar Adobe Maestro para diseñar espacios de trabajo totalmente personalizables que contengan los tipos de registros necesarios en su organización. Una manera de indicar cómo se relacionan los tipos de registros individuales entre sí es conectarlos. Además, puede conectar los tipos de registros de Maestro con los tipos de objetos de otras aplicaciones para mejorar la experiencia de los usuarios y mantener el enfoque en una aplicación.

Puede conectar lo siguiente:

* Tipos de registros operativos de Maestro entre sí
* taxonomías de Maestro entre sí
* Tipos de registros operativos y taxonomías de Maestro entre sí
* Tipos de registros operativos y taxonomías de Maestro con tipos de objetos de otras aplicaciones.

De este modo, puede mostrar campos del registro vinculado o del tipo de objeto de otro registro Maestro.

En este artículo se describe cómo conectar dos tipos de registro Maestro o un tipo de registro Maestro con un objeto de otra aplicación.

Una vez establecida la conexión entre los tipos de registro u objeto, puede conectar registros individuales entre sí.

Para obtener información acerca de cómo conectar un registro Maestro a un objeto de otra aplicación, vea [Conectar registros](../records/connect-records.md).

Para ver un ejemplo de tipos de registros de conexión, consulte [Ejemplo de conexión de tipos y registros](../architecture/example-connect-record-types-and-records.md).

<!--ensure this last linked article is right; the title and the link should have changed-->

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> <p>Para conectar los tipos de registros de Maestro con Experience Manager Assets, debe tener una licencia de Adobe Experience Manager Assets y la instancia de Workfront de su organización debe estar integrada en Adobe Business Platform o en Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en el programa beta cerrado de Adobe Maestro. Póngase en contacto con el representante de cuentas para obtener más información sobre esta nueva oferta. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>plan de Adobe Workfront</p></td>
   <td>
<p>Cualquiera</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td>
   <td>
   <p>Cualquiera</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>Configuraciones de nivel de acceso</p></td>
   <td> <p>No hay controles de nivel de acceso para Maestro</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador de Workfront o de grupo debe agregar el área de Maestro en la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon
</td>
  </tr>
 </tbody>
</table>

<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->


## Consideraciones sobre la conexión de tipos de registros

Tenga en cuenta lo siguiente:

* Puede conectar las siguientes entidades en Maestro:

   * Dos tipos de registros operativos
   * Dos taxonomías
   * Un tipo de registro operativo y una taxonomía
   * Un tipo de registro operativo o una taxonomía y un tipo de objeto de otra aplicación.

* Puede conectar los siguientes objetos desde las siguientes aplicaciones con los tipos de registros de Maestro:

   * Adobe Workfront:

      * Proyectos
      * Portafolios
      * Programas
      * Compañías
      * Grupos

   * Adobe Experience Manager Assets:

      * Imágenes
      * Carpetas

     >[!IMPORTANT]
     >
     >Debe tener una licencia de Adobe Experience Manager Assets y la instancia de Workfront de su organización debe estar integrada en Adobe Business Platform o Adobe Admin Console para conectar los registros de Maestro a Adobe Experience Manager Assets.
     >
     >Si tiene alguna pregunta acerca de la incorporación a Adobe Admin Console, consulte la [Preguntas frecuentes sobre Adobe Unified Experience](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/unified-experience-faq.md).

* Después de conectar un tipo de registro con otro tipo de registro o con un tipo de objeto de otra aplicación, existen los siguientes escenarios:

   * **Cuando conecta dos tipos de registros**: se crea un campo de registro vinculado en el tipo de registro desde el que se conecta. Se crea un campo de registro vinculado similar en el tipo de registro al que se conecta.

     Por ejemplo, si conecta el tipo de registro &quot;Campaña&quot; con el tipo de registro &quot;Producto&quot;, se crea un campo de registro vinculado denominado &quot;Producto vinculado&quot; en el tipo de registro de Campaña y se crea un tipo de registro vinculado denominado automáticamente &quot;Campaña&quot; en el tipo de registro de Producto.

   * **Cuando conecta un tipo de registro con un tipo de objeto de otra aplicación**: se crea un campo de registro vinculado en el tipo de registro desde el que se conecta. No se crea automáticamente ningún campo de registro vinculado en el objeto de aplicación de terceros.

     Sólo se crea un nuevo tipo de registro Maestro para el objeto de aplicación de terceros cuando los objetos reales están conectados a los registros Maestro.

     Para obtener más información, consulte [Conectar registros](../records/connect-records.md).

   * **Cuando se agregan campos de búsqueda desde el registro u objeto al que se conecta**: los campos vinculados se agregan al registro desde el que se está conectando y muestran los campos de búsqueda que seleccionó para pasar del registro vinculado a los registros desde los que está vinculando. Los campos de registro siempre son de solo lectura y se rellenan automáticamente con los valores del objeto de terceros.

     Por ejemplo, si conecta el tipo de registro Maestro &quot;Campaña&quot; con un proyecto de Workfront y selecciona traer el campo Fecha planificada de finalización del proyecto al registro Maestro, se crea automáticamente un campo vinculado denominado Fecha planificada de finalización (desde Project) para el registro desde el que está vinculando.

* Los campos de registro vinculados van precedidos de un icono de relación ![](assets/relationship-field-icon.png).

  Los campos vinculados van precedidos de un icono que identifica el tipo de campo. Por ejemplo, los iconos que indican que un campo es un número, un párrafo o una fecha.

* Después de crear registros individuales para un tipo de registro, puede seleccionar los registros a los que se conecta desde el campo tipo de registro vinculado. Para obtener más información, consulte [Conectar registros](../records/connect-records.md).

## Conectar tipos de registros

<!--when changes here, also update the article for "Connect records"-->

{{step1-to-maestro}}

El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo desde la que desea conectar los tipos de registros.
1. Haga clic en la tarjeta de un tipo de registro para abrir la página del tipo de registro.
1. Haga clic en **+** en la esquina superior derecha de la vista de tabla y, a continuación, haga clic en el icono **Nueva conexión** pestaña.

   ![](assets/new-connection-tab-with-workfront-aem-options.png)

1. En el **Tipo de registro** , busque un tipo de registro o seleccione una de las siguientes opciones: <!--is the field name spelled right? lowercase "t"?-->

   * Otro tipo de registro operativo o una taxonomía del espacio de trabajo seleccionado

     >[!TIP]
     >
     >Solo están disponibles para la conexión los tipos de registro y las taxonomías del espacio de trabajo seleccionado.
     > 
     >Si no hay otros tipos de registro en el espacio de trabajo seleccionado, el nombre del espacio de trabajo no se muestra.

   * A **Proyecto, Portfolio, Programa, Empresa**, o **Grupo** desde el **Tipos de objetos Workfront** sección.
   * **Experience Manager Assets** desde el **Aplicaciones de Adobe** sección.

   ![](assets/new-connection-tab-fields-with-another-record-selected.png)


1. Actualice la siguiente información:

   * **Nombre**: Nombre del campo conectado, tal como aparecerá en la vista de tabla o en la página Detalles del tipo de registro original. Esto crea la columna de registro vinculado en la vista de tabla del tipo de registro original o el campo de registro vinculado para los registros originales. <!--ensure they updated this; and update the screen shot: it used to be "Label"-->

   >[!TIP]
   >
   >Se recomienda incluir el nombre del registro al que se está vinculando en el nombre del campo de registro conectado para capturar de qué tipo de registro proviene el nuevo campo. El nombre del registro vinculado no es visible en el nuevo campo de registro vinculado o en sus campos vinculados.

   * **Descripción**: Información adicional sobre el campo de registro conectado. La descripción de un campo se muestra cuando pasa el ratón sobre la columna del campo de una tabla.
   * **Permitir varios registros**: seleccione esta opción para indicar que permite que los usuarios puedan agregar varios registros cuando el campo de tipo de registro vinculado aparece en los registros originales. Esta opción está seleccionada de forma predeterminada.
   * **Seleccionar campos de búsqueda**: seleccione esta opción para agregar campos del tipo de registro seleccionado. Esta opción está seleccionada de forma predeterminada.

1. (Condicional y opcional) Si ha seleccionado conectar un objeto de Workfront, seleccione un **Formulario personalizado** desde el **Vincular solo proyectos que cumplan estos criterios** sección. <!--this needs to be updated for each object when they fix this UI.--> Sólo los objetos que tienen los formularios personalizados seleccionados adjuntos pueden vincularse al tipo de registro Maestro seleccionado. Puede seleccionar varios formularios.

   ![](assets/workfront-project-connection-selection.png)

1. (Condicional) Si ha seleccionado conectarse a Experience Manager Assets, seleccione un repositorio en la **repositorio del Experience Manager** menú desplegable en el **Vincular recursos del siguiente repositorio** sección. Este campo es obligatorio. En este campo solo se muestran los repositorios a los que tiene acceso en Experience Manager Assets.

   ![](assets/aem-assets-connection-selection.png)

1. Haga clic en **Crear**.

1. (Condicional) Si seleccionó la variable **Seleccionar campo de búsqueda** configuración, la **Agregar campos de búsqueda** se abre el cuadro.

   Haga clic en **+** para añadir campos desde el **Campos no seleccionados** área.

   O

   Haga clic en **-** para eliminar campos de la **Campos seleccionados** área

   ![](assets/add-lookup-fields-for-another-maestro-record-type-box.png)


1. (Opcional) Haga clic en **Omitir** y no agregue ningún campo del registro u objeto vinculado. El **Nombre** del registro vinculado es el único campo visible en la vista de tabla del registro original.

1. (Opcional y condicional) Si selecciona vincular un campo de número, moneda, porcentaje o tipo de fecha, seleccione también un valor de acumulador. Los valores de los campos vinculados se muestran separados por comas o como un valor agregado según el agregador que elija, cuando los usuarios seleccionen más de un registro vinculado en el campo de registro vinculado.

   ![](assets/aggregator-drop-down-for-number-linked-field.png)

   >[!NOTE]
   >
   > Los acumuladores no están disponibles al conectar tipos de registros a Experience Manager Assets.

   Seleccione una de las siguientes opciones:

   * **Ninguno**: Muestra los valores procedentes de varios registros separados por comas. Esta es la selección predeterminada.
   * **MAX**: Muestra el valor más alto de todos los valores procedentes de varios registros seleccionados en el campo de registro vinculado.
   * **MIN**: Muestra el valor más bajo de todos los valores procedentes de varios registros seleccionados en el campo de registro vinculado.
   * **SUM**: Muestra el total de todos los valores procedentes de varios registros seleccionados en el campo de registro vinculado.
   * **AVG**: Muestra el promedio de todos los valores procedentes de varios registros seleccionados en el campo de registro vinculado.

   >[!NOTE]
   >
   >Por ejemplo, puede vincular el registro de producto (registro vinculado) desde el registro de campaña (registro original) y asignarle el nombre &quot;Campo de producto&quot;. También puede vincular el campo Presupuesto del registro de producto del registro de campaña y llamarlo &quot;Presupuesto de producto&quot;. Si se le permite seleccionar varios registros en el &quot;Campo de producto&quot;, puede seleccionar el Producto 1 con un presupuesto de 120 000 $ y el Producto 2 con un presupuesto de 100 000 $. Puede ver la siguiente información de presupuesto en el campo vinculado desde el registro original, en función del agregador que elija:
   >
   >* **Ninguno**: 120 000 $, 100 000 $
   >* **MAX**: 120 000 $
   >* **MIN**: 100 000 $
   >* **SUM**: 220 000 $
   >* **AVG**: 110 000 $
   >

1. (Opcional) Utilice la variable **búsqueda** icono ![](assets/search-icon.png) para buscar un campo.

1. Clic **Añadir campos** para guardar los cambios.

   Se añaden los elementos siguientes:

   * Campo de registro vinculado que muestra los registros del tipo de registro vinculado, después de agregarlos manualmente. El nombre del campo de registro vinculado es el nombre seleccionado en el paso 5. <!--accurate-->

   * Campo o campos vinculados que muestran información de los campos del tipo de registro vinculado después de agregar manualmente los registros en el campo de registro vinculado. Los campos vinculados se crean únicamente cuando **Seleccionar campos de búsqueda** La configuración se selecciona al crear la conexión. Los campos vinculados reciben un nombre según este patrón:

     `<Name of the original field on the linked record> (from <Name of your linked field>)`

   * Cuando se vinculan tipos de registros de Maestro, también se agrega un campo de registro vinculado en el tipo de registro al que se está vinculando El nombre del campo de registro vinculado en el tipo de registro vinculado es el nombre del tipo de registro desde el que se establece el vínculo.

     Por ejemplo, si vincula el tipo de registro &quot;Producto&quot; desde el tipo de registro &quot;Campaña&quot; y asigna al campo conectado de la campaña el nombre &quot;Producto vinculado&quot;, se crea un campo de registro vinculado &quot;Campaña&quot; para el tipo de registro Producto.

1. (Opcional) Desde el tipo de registro original o la vista de tabla del tipo de registro vinculado, haga clic en la flecha hacia abajo en el encabezado de los campos de registro vinculados y, a continuación, haga clic en una de las siguientes opciones:

   * **Editar campo**: solo puede actualizar el **Nombre** y el **Descripción** información del campo.
   * **Editar campos de búsqueda**: agregue o quite cualquiera de los campos del registro vinculado.

   ![](assets/edit-field-and-lookup-fields-drop-down-menu-in-table-column.png)

   Para agregar o quitar campos de búsqueda, siga las instrucciones de los pasos 9-13 anteriores. <!--ensure these step numbers stay accurate-->

   >[!NOTE]
   >
   > No se pueden agregar los campos de búsqueda del registro vinculado al tipo de registro vinculado que indica un objeto en una aplicación de terceros.
   >
   > Por ejemplo, no puede agregar el campo de búsqueda de un objeto Maestro &quot;Campaign&quot; desde el campo de registro vinculado &quot;Campaign&quot; que se muestra en el tipo de registro de Proyecto Maestro al vincularlo a proyectos de Workfront.


1. (Opcional) Haga clic en la flecha hacia abajo en el encabezado del campo de registro vinculado desde el tipo de registro desde el que está vinculando y, a continuación, haga clic en **Eliminar**.

   El campo de registro y cualquier campo de búsqueda vinculado adicional se eliminan, y los campos y su información no se pueden recuperar.

   >[!TIP]
   >
   >    El campo de registro vinculado del tipo de registro al que está vinculando no se elimina. <!-- is this still accurate?! -->
