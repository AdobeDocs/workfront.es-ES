---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: "Ver: Porcentaje de rol de usuario de disponibilidad de FTE"
description: Puede agregar una columna a la vista de una lista de usuarios para mostrar una lista de los roles a los que está asociado el usuario, así como el porcentaje de disponibilidad de FTE para cada rol, tal como se define en el perfil de usuario.
author: Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 66de6c952272f52876f8e912c96d1526575b6f0b
workflow-type: tm+mt
source-wordcount: '297'
ht-degree: 0%

---

# Ver: porcentaje de puesto de usuario con disponibilidad de ETC

<!--Audited: 11/2024-->

Puede agregar una columna a la vista de una lista de usuarios para mostrar una lista de los roles a los que está asociado el usuario, así como el porcentaje de disponibilidad de FTE para cada rol, tal como se define en el perfil de usuario.

Para obtener información acerca de cómo definir el porcentaje de disponibilidad de FTE para los usuarios, vea [Editar el perfil de un usuario](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

![usuario_con_porcentaje_disponibilidad_por_rol.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> <p> Actual: 
   <ul>
   <li>Solicitud para modificar una vista</li> 
   <li>Plan para modificar un informe</li>
   </ul>
     </p>
     <p> Nuevo: 
   <ul>
   <li>Colaborador para modificar una vista</li> 
   <li>Estándar para modificar un informe</li>
   </ul>
     </p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a Informes, Tableros y Calendarios para modificar un informe</p> <p>Editar el acceso a filtros, vistas y agrupaciones para modificar una vista</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administración de permisos de un informe</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Ver porcentaje de puesto de usuario con disponibilidad de ETC

1. Vaya a una lista de usuarios.
1. En el menú desplegable **Vista**, seleccione **Nueva vista**.

1. En el área **Vista previa de columna**, haga clic en **Agregar columna**.

1. Haga clic en el encabezado de la nueva columna y, a continuación, haga clic en **Cambiar al modo de texto** > **Editar modo de texto**.
1. Elimine el texto que encuentre en el cuadro **Editar modo de texto** y reemplácelo por el siguiente código:

   ```
   displayname=Roles Time Percentage
   listdelimiter=
   listmethod=nested(userRoles).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({role},'-',{timePercentage},'%')
   valueformat=HTML
   ```

1. Haga clic en **Listo** y luego en **Guardar vista**.

1. (Opcional) Actualice el nombre de la vista y, a continuación, haga clic en **Guardar vista**.
