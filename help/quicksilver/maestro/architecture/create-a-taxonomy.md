---
title: Crear tipos de registros de taxonomía
description: Las taxonomías son un tipo de tipos de registros reutilizables que capturan atributos sobre un tipo de registro operativo en Adobe Workfront Maestro.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: e90a3ebe-fc02-4cce-8472-1ca5004ddde8
source-git-commit: 5681b540bceddaae85116b632e968d94761eec0d
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 0%

---

<!--udpate the metadata with real information when making this avilable in TOC and in the left nav-->

# Crear tipos de registros de taxonomía

{{maestro-important-intro}}

Los tipos de registros de taxonomía capturan atributos sobre tipos de registros operativos en Adobe Maestro.

Por ejemplo, Campaign puede ser un tipo de registro operativo. Las siguientes son taxonomías que capturan atributos sobre el tipo de registro de campaña: Región, Audiencia, País.

Para obtener más información acerca de los tipos de registros de Maestro, vea [Información general sobre los tipos de registros y las taxonomías](../architecture/overview-of-record-types-and-taxonomies.md).

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

## Consideraciones sobre la creación de taxonomías

* Debe crear un espacio de trabajo para poder crear tipos de registros de taxonomía en el espacio de trabajo.

  Para obtener información sobre los espacios de trabajo, consulte [Creación de espacios de trabajo](../architecture/create-workspaces.md).
* Puede crear un tipo de registro de taxonomía realizando una de las siguientes acciones:
   * Se crean automáticamente al crear un espacio de trabajo con una plantilla. Para obtener más información, consulte [Creación de espacios de trabajo](../architecture/create-workspaces.md).
   * Créelas manualmente, desde cero.

* Todos los tipos de registros de taxonomía recién creados incluyen los siguientes campos:

   * Nombre <!--if there won't be any more fields, consider rephrasing this-->

  Además, puede agregar campos personalizados a las taxonomías. Para obtener más información, consulte [Creación de campos](../fields/create-fields.md).

  >[!NOTE]
  >
  >    Los tipos de registro de taxonomía creados al utilizar una plantilla de espacio de trabajo tienen campos adicionales.

## Creación de un tipo de registro de taxonomía

Crear tipos de registros de taxonomía es similar a crear tipos de registros operativos desde cero o desde una plantilla de espacio de trabajo.

Para obtener más información, consulte la sección &quot;Crear un tipo de registro desde cero&quot; en el artículo [Creación de tipos de registros](../architecture/create-record-types.md).

Para obtener información sobre la creación automática de taxonomías al crear un espacio de trabajo a partir de una plantilla, consulte [Creación de espacios de trabajo](../architecture/create-workspaces.md).
