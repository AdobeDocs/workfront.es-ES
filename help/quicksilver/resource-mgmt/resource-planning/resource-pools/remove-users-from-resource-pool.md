---
product-area: resource-management
navigation-topic: resource-pools
title: Quitar usuarios de conjuntos de recursos
description: Aunque no hay límite para la cantidad de usuarios que puede tener en un conjunto de recursos, la lista de usuarios sólo muestra los primeros 2000 usuarios, enumerados alfabéticamente.
author: Lisa
feature: Resource Management
exl-id: b888aa95-8d42-4cc3-8a99-6842435c84d2
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '378'
ht-degree: 1%

---

# Quitar usuarios de conjuntos de recursos

{{preview-and-fast-release-Q424}}

Aunque no hay límite para la cantidad de usuarios que puede tener en un conjunto de recursos, la lista de usuarios sólo muestra los primeros 2000 usuarios, enumerados alfabéticamente.

Se recomienda eliminar los usuarios que se han desactivado o que han movido funciones o departamentos, para garantizar que siempre tenga una lista precisa de los usuarios en todos los conjuntos de recursos.

Para obtener más información acerca de los conjuntos de recursos, vea [Resumen de los conjuntos de recursos](../../../resource-mgmt/resource-planning/resource-pools/work-with-resource-pools.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td><p>Nuevo: Cualquiera</p>
       <p>o</p>
       <p>Actual: Pro o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td><p>Nuevo: estándar</p>
       <p>o</p>
       <p>Actual: plan</p></td>
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Administración de recursos que incluye acceso a Administrar conjuntos de recursos</p> <p>Acceso de visualización o superior a los usuarios</p></td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Quitar usuarios de un conjunto de recursos

Puede quitar usuarios de un conjunto de recursos cuando ya no los necesite en dicho conjunto.

Para eliminar un usuario de un conjunto de recursos:

{{step1-to-resourcing}}

1. Haga clic en **Conjuntos de recursos** en el panel izquierdo.
1. Seleccione un conjunto de recursos y haga clic en **Editar**.
O\
   Haga clic en el nombre de un conjunto de recursos.

1. Empiece a escribir el nombre de un usuario que desee quitar en el campo **Buscar en este conjunto de recursos**.\
   O\
   Empiece a escribir el nombre de una empresa, función de trabajo, equipo o grupo si desea quitar todos los usuarios asociados a esas entidades.

   <span class="preview">Imagen de muestra en el entorno de vista previa:<span>

   ![Quitar usuarios del conjunto de recursos](assets/remove-users-from-resource-pool.png)

   Imagen de muestra en el entorno de producción:
   ![Buscar en el conjunto de recursos](assets/search-inside-new-resource-pool-350x314.png)

1. Haga clic en el icono &quot;x&quot; en el nivel de usuario para eliminar un usuario del conjunto de recursos. Se eliminan de todas las listas en las que aparecen.\
   O\
   Para quitar todos los usuarios asociados con un rol, grupo, equipo o compañía, haga clic en **Quitar** en el rol, grupo, nivel de equipo o nivel de compañía del trabajo. Esto elimina del conjunto de recursos a todos los usuarios asociados a ese rol, grupo, equipo o compañía.

1. Haga clic en **Guardar**.
