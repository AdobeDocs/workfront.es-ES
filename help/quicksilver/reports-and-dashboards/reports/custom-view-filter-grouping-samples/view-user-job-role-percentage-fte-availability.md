---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 'Ver: usuario Puesto de trabajo Porcentaje de disponibilidad de FTE'
description: Puede agregar una columna al vista de una usuario lista para mostrar un lista de los roles de trabajo con los que está asociado el usuario, así como el porcentaje de disponibilidad de FTE para cada función de trabajo, según se define en el usuario perfil.
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

# Ver: porcentaje de puesto de usuario con disponibilidad de ETC

Puede agregar una columna a la vista de una lista de usuarios para mostrar una lista de los roles a los que está asociado el usuario, así como el porcentaje de disponibilidad de FTE para cada rol, tal como se define en el perfil de usuario.

Para obtener información acerca de cómo definir el porcentaje de disponibilidad de FTE para los usuarios, vea [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![usuario_con_porcentaje_avivialidad_por_función.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Systems Plan Workfront*</td> 
   <td> <p>Cualquier</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Systems Licencia Workfront*</td> 
   <td> <p>Solicitud de modificación de un vista </p>
   <p>plan modificar un informe</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> <p><b>NOTA</b>

Si aún no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">Permisos de objetos</td> 
   <td> <p>Administrar permisos para un informe</p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, tipo de licencia o acceso tiene, comuníquese con el administrador de Workfront.

## Puesto de trabajo Ver usuario Porcentaje de disponibilidad de FTE.

1. Vaya a un lista de usuarios.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. En el área **Vista previa de columna**, haga clic en **Agregar columna**.

1. Haga clic en el encabezado de la nueva columna y, a continuación, haga clic en **Cambiar al modo de texto**.
1. Pase el ratón sobre el área Modo de texto y haga clic en Haga clic **para editar el texto**.
1. Quitar el texto que encuentra en el **cuadro Modo de** texto y sustitúyalo por el siguiente código:
   <pre>displayname=Porcentaje de<br>tiempo de los roles listdelimiter=<p><br>listmethod=nested(userRoles).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>

1. Haga clic en Guardar **y, a continuación**, en **Guardar Ver**.

1. (Opcional) Especifique un nombre para el vista y haga clic en **Guardar Ver**.
