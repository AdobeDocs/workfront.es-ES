---
title: Editar tipos de registros
description: Puede editar los tipos de registro una vez guardados. Los tipos de registro son los tipos de objetos de Adobe Workfront Planning.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 7d6de742-9657-4286-968c-1fc78ebbb94e
source-git-commit: 1369269bcb64bd32f26603608782dc996b079cb9
workflow-type: tm+mt
source-wordcount: '435'
ht-degree: 1%

---

<!--update the metadata with real information when making this available in TOC and in the left nav
---
title: Edit record types
description: You can edit record types after they have been saved. Record types are the object types of Adobe Workfront Planning.
author: Alina
role: User
feature: Work Management 
topic: Architecture
hidefromtoc: yes
hide: yes
---

-->

# Editar tipos de registros

{{planning-important-intro}}

Los tipos de registro son los tipos de objetos de Adobe Workfront Planning. Puede editar el aspecto de los tipos de registro que usted o cualquier otra persona hayan creado. Para obtener información sobre la creación de tipos de registros de Workfront Planning, consulte [Creación de tipos de registros](../architecture/create-record-types.md).

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
   <p> Adobe Workfront</p> <p>Para conectar los tipos de registros de Adobe Workfront Planning con Experience Manager Assets, debe tener una licencia de Adobe Experience Manager Assets y la instancia de Workfront de su organización debe estar integrada en Adobe Business Platform o Adobe Admin Console.</p> </td>
  </tr>  
 <td role="rowheader"><p>acuerdo con Adobe Workfront</p></td>
   <td>
<p>Su organización debe estar inscrita en la fase de acceso anticipado para Workfront Planning </p>
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
   <td> <p>No hay controles de nivel de acceso para Workfront Planning</p>  
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Permisos</p></td>
   <td> <p>Administración de permisos en un espacio de trabajo</a> </p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Plantilla de diseño</p></td>
   <td> <p>El administrador del grupo o de Workfront debe agregar el área de Planning a la plantilla de diseño. Para obtener más información, consulte <a href="../access/access-overview.md">Acceso a información general</a>. </p>  
</td>
  </tr>

</tbody>
</table>

<!--Maybe enable this at GA - but Planning is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

## Editar tipos de registros

{{step1-to-maestro}}

El espacio de trabajo al que se accedió por última vez debe abrirse de forma predeterminada.

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un área de trabajo existente y seleccione el área de trabajo para la que desea editar los tipos de registros.
1. Pase el ratón sobre la tarjeta de un tipo de registro y haga clic en **Más** menú ![](assets/more-menu.png) en la esquina superior derecha de la tarjeta de tipo de registro, haga clic en **Editar**.

   ![](assets/more-menu-options-from-record-type-card.png)

1. En el **Editar tipo de registro** , actualice la siguiente información:

   * Edite el nombre del tipo de registro si es necesario. <!--did they add a field label for this? -->
   * **Descripción**: edite o agregue una descripción para el tipo de registro con más información sobre él.
   * Edite el color y la forma del icono asociado al tipo de registro. Haga lo siguiente:
      * Seleccione un color para identificar el tipo de registro. Es el color del icono de tipo de registro. Gris está seleccionado de forma predeterminada.
      * Seleccione un icono de la lista o empiece a escribir el nombre de un icono para describir lo que representa y, a continuación, selecciónelo cuando se muestre. Este es el icono del tipo de registro. De forma predeterminada, se selecciona un icono de archivo.

     ![](assets/update-record-type-box.png)

1. Haga clic en **Guardar**.
1. (Opcional) Haga clic en la tarjeta de tipo de registro del área de trabajo para abrir la página del tipo de registro.
1. Haga clic en **Más** a la derecha del nombre del tipo de registro y haga clic en **Editar** para actualizar información sobre el tipo de registro.

   >[!TIP]
   >
   >   Puede cambiar el nombre del tipo de registro en el encabezado.

   ![](assets/more-menu-options-from-record-details-page.png)

   <!--check this screen shot - not sure this is valid ???-->

1. (Opcional) Expanda la flecha hacia abajo a la derecha del nombre de un tipo de registro y seleccione otro tipo de registro para editar.
