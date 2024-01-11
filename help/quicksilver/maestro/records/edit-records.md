---
title: Edición de registros
description: Puede editar la información de los registros en Adobe Maestro. Debe crear tipos de registros antes de empezar a crear y editar registros.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 981b8e44-b548-4f94-bf89-5f5dec3a6166
source-git-commit: 1ae60512c337d778939ef6c48fd2eda8b279dcce
workflow-type: tm+mt
source-wordcount: '875'
ht-degree: 1%

---

<!--update the metadata with real information when making this avilable in TOC and in the left nav-->

# Edición de registros

>[!IMPORTANT]
>
>La información de este artículo hace referencia a Adobe Maestro, que es una nueva oferta de Adobe Workfront.
>
>En la actualidad, Adobe Maestro forma parte de un programa beta abierto a un número limitado de clientes. Debe ser cliente de Workfront para utilizar las funciones de Maestro.
>
>Póngase en contacto con su representante de cuentas para obtener más información acerca de cómo unirse al programa beta de Maestro.
>
>Para obtener más información, consulte [Introducción a Adobe Maestro](../maestro-overview.md).

Puede editar la información de los registros en Adobe Maestro. Debe crear tipos de registros antes de empezar a crear y editar registros.
Para obtener más información, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

&lt;!— mencione aquí que los campos de la vista Detalles son los mismos que los de la vista de tabla — este artículo está vinculado desde Administrar vistas de registros a hacer referencia a esta información—>

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
   <p> Adobe Workfront</p> </td>
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
   <td> <p>No hay controles de acceso para Maestro </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Permisos de contribución o superiores en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador de Workfront o de grupo debe agregar el área de Maestro en la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

## Consideraciones acerca de la edición de registros

* Puede editar los registros que usted u otro usuario hayan creado. <!--will change with access levels-->
* No se pueden editar campos vinculados desde otros registros o campos que contengan cálculos.
* Si los registros que muestra están vinculados a otros registros, la nueva información de los registros que está modificando se reflejará en los registros vinculados.
* No puede editar registros de forma masiva. <!--this will probably change-->
* Las direcciones URL se reconocen como vínculos en tipos de campo de texto de una sola línea solo cuando comienzan con lo siguiente: http://, https://, ftp:// o www. .
* Puede utilizar las siguientes opciones de formato de texto enriquecido al editar un campo de tipo párrafo:

   * Negrita
   * Cursiva
   * Subrayado
   * Añadir un vínculo
   * Agregar una lista con viñetas
   * Añadir una lista numerada

## Edición de registros

Puede editar un registro desde las siguientes áreas:

* [Desde la página Detalles de un registro](#edit-a-record-from-the-records-details-page)
* [Desde la vista de tabla de un tipo de registro](#edit-a-record-from-the-record-type-table-view)

### Editar un registro desde la página de detalles del registro

{{step1-to-maestro}}

El espacio de trabajo al que se accede por última vez se abre.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del nombre del área de trabajo para seleccionar el área de trabajo cuyos registros desea actualizar.
1. Realice una de las siguientes acciones:

   * En la vista Tabla, haga clic en el nombre de un registro.
   * En la vista Tabla, pase el ratón sobre el nombre de un registro y haga clic en **Más** menú ![](assets/more-menu.png), luego haga clic en **Ver**

     ![](assets/contextual-menu-for-record-row.png)
   * En una vista Línea de tiempo, haga clic en una barra de registros.

   El registro **Detalles** se abre la página.

1. Haga clic en **Más** menú ![](assets/more-menu.png) a la derecha del nombre del registro y haga clic en **Editar**

   O

   Haga clic dentro de cualquier campo editable de la página Detalles para editar la información.

   ![](assets/more-menu-options-from-record-details-page.png) <!--ensure the options have not changed or been renamed-->

1. Clic **Guardar cambios**. <!--logged a bug for this - this needs to be "Save"-->

### Editar un registro desde la vista de tabla de un tipo de registro

{#step1-to-maestro}

Se abre el espacio de trabajo al que accedió por última vez.

1. (Opcional) Haga clic en la flecha hacia abajo situada a la derecha del nombre del área de trabajo para seleccionar el área de trabajo cuyos registros desea actualizar.
1. Haga clic en una tarjeta de tipo de registro.

   Se abre la página de tipo de registro.
1. (Condicional) Desde el **Ver** menú desplegable en la esquina superior derecha de la tabla, seleccione un **Tabla** vista. Esta debe ser la vista predeterminada, a menos que haya visto el tipo de registro en la vista de escala de tiempo cuando accedió por última vez.

   Los registros asociados al tipo de registro seleccionado se muestran en la vista de tabla.
1. Haga clic dentro de la fila de un registro para empezar a editar la información sobre el registro en línea.

   ![](assets/edit-record-paragraph-field-with-formatting-table-view.png)
1. Prensa **Entrar** en el teclado o haga clic fuera de una fila para guardar los cambios. Los cambios se guardan automáticamente. Un indicador Guardado aparece brevemente en la esquina superior derecha de la vista de tabla para mostrar que los cambios se han guardado.

   >[!NOTE]
   >
   >  No puede editar la información de los siguientes campos, ya que son de solo lectura y Workfront los actualiza automáticamente:
   >  
   >  * Campos vinculados que se crean conectando tipos de registro. Para obtener más información, consulte [Conectar tipos de registros](../architecture/connect-record-types.md).
   >  * Campos de los siguientes tipos: Creado por, Fecha de creación, Última modificación por, Fecha de última modificación


1. (Opcional) Copie uno o varios valores existentes de un campo, péguelos en un campo del mismo tipo en otro registro y haga clic en **Entrar** en el teclado para guardar los cambios.

   >[!NOTE]
   >
   >Tenga en cuenta lo siguiente:
   >
   >* No puede copiar información de otro origen que no sea un campo Maestro del mismo tipo que el campo en el que pega la información.
   >
   >* No se pueden copiar y pegar valores de campo en el área de Detalles de un registro. Esta funcionalidad solo se admite en la vista de tabla de un tipo de registro.
   >* No puede copiar y pegar valores de campo para los siguientes tipos de campo:
   >
   >
   >    * Campos vinculados que se crean conectando tipos de registro. Puede copiar y pegar campos de registro vinculados. Para obtener más información, consulte [Conectar tipos de registros](../architecture/connect-record-types.md).
   >    * Campos de los siguientes tipos: Creado por, Fecha de creación, Última modificación por, Fecha de última modificación

1. (Opcional) Utilice los siguientes métodos abreviados del teclado para deshacer o rehacer la edición o copiar y pegar la información de los registros:

   * **Deshacer**: CTRL/CMD + Z
   * **Rehacer**: CTRL/CMD + Mayús + Z