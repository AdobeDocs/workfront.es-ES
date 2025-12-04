---
title: Creación de jerarquías de Workspace
description: Como administrador de espacio de trabajo, puede crear varias jerarquías de espacio de trabajo entre los tipos de registro en Adobe Workfront Planning. Después de conectar los tipos de registro en un espacio de trabajo y crear una jerarquía, los tipos de registro se conectan entre sí, con un tipo de registro designado como principal y hasta 6 tipos de registro más configurados como secundarios.
hide: true
hidefromtoc: true
exl-id: 2f83c427-4439-499d-a0b2-fc8630552cae
source-git-commit: ff9371b639e7684a94c08b8cd6293b632fac9edf
workflow-type: tm+mt
source-wordcount: '248'
ht-degree: 10%

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

Después de conectar los tipos de registro en un espacio de trabajo y crear una jerarquía, los tipos de registro se conectan entre sí, con un tipo de registro designado como principal y hasta 6 tipos de registro más configurados como secundarios. <!--asking Robert how many we can have in one hierarchy; I think 7 total but not sure-->

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
