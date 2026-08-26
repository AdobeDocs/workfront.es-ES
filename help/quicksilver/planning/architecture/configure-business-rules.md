---
title: Configurar reglas de negocio de tipo de registro
description: Puede configurar reglas empresariales de tipo de registro que definan cómo se administran los registros de ese tipo en Adobe Workfront Planning.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
source-git-commit: 159b845c7b755117197d18f8474c01d4b19d53b8
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 14%

---


# Configurar reglas empresariales de tipo de registro

{{planning-important-intro}}

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the release to Preview, the same features are also available monthly in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

Puede configurar reglas empresariales de tipo de registro que definan cómo se administran los registros de ese tipo en Adobe Workfront Planning.

## Requisitos de acceso

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
<li><p>Cualquier Workfront o flujo de trabajo con un paquete de Planning</p></li>
O
<li><p>Cualquier paquete de Planning cuando se adquiere como producto independiente</p></li></ul>
   </td> </tr>
  <tr> 
   <td role="rowheader"><p>Licencia de Adobe Workfront</p></td> 
   <td><p>Workflow Standard</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Licencia de planificación de Adobe</p></td> 
   <td><p>Estándar de planificación</p>
   </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>Configuración de nivel de acceso</p></td> 
   <td> <p>Debe agregar un tipo de licencia de flujo de trabajo y de Planning al nivel de acceso cuando tenga un flujo de trabajo y un paquete de Planning a la vez</p>   
</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Permisos de objeto</p></td> 
   <td>   <p>Administración de permisos en un espacio de trabajo y en un tipo de registro</p>  
   <p>Los administradores del sistema tienen permisos para todos los espacios de trabajo, incluidos los que no crearon</p>  </td> 
  </tr>  
</tbody> 
</table>

Para obtener más información acerca de los requisitos de acceso de Workfront, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Consideraciones al configurar reglas empresariales

* Puede configurar reglas para cuándo se pueden editar o eliminar registros.
* No se pueden configurar reglas para cuándo se crean los registros. Todas las personas con permisos de administración en el tipo de registro pueden crear registros.
* Puede crear una condición para la regla de negocio que haga referencia a todos los tipos de campo excepto a los siguientes:
  * Campos de fórmula
  * Campos de búsqueda
  * Campos de referencia

## Configurar reglas empresariales

1. Vaya a un tipo de registro.
1. Haga clic en el menú **Más** ![Menú más](assets/more-menu.png) que se encuentra a la derecha del nombre del tipo de registro y, a continuación, haga clic en Reglas de negocio.



