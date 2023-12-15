---
product-area: projects;user-management
keywords: adjuntar, aplicar
navigation-topic: work-with-custom-forms
title: Agregar un formulario personalizado a un objeto
description: Puede agregar un formulario personalizado existente a cualquiera de los objetos enumerados a continuación. Un formulario personalizado contiene campos personalizados en los que se puede almacenar información sobre el objeto.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 4e3cafafb121371249fb73f2f001477bdbad2d77
workflow-type: tm+mt
source-wordcount: '850'
ht-degree: 2%

---

# Agregar un formulario personalizado a un objeto

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Puede agregar un formulario personalizado existente a cualquiera de los objetos enumerados a continuación. Un formulario personalizado contiene campos personalizados en los que se puede almacenar información sobre el objeto.

* Proyectos (incluidos casos comerciales)
* Tareas
* Problemas
* Compañías
* Portafolios
* Programas
* Documentos
* Usuarios
* Iteraciones
* Gastos
* Registros de facturación

Puede agregar un formulario personalizado solo a los tipos de objetos para los que se creó el formulario.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar las acciones descritas en este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Licencia de Adobe Workfront*</td> 
  <td> <p>Nuevo: Colaborador o superior </p>
 <p>o</p> 
<p>Actual: Solicitud o superior </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar el acceso a los objetos para los que administra formularios personalizados</p> <p><b>NOTA</b></p>

Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos al objeto para el que desea adjuntar un formulario personalizado.</p> <p>Ver o permisos superiores del formulario personalizado, con permiso para <b>Adjuntar a datos personalizados</b> objetos (proyectos, tareas y problemas). Para obtener más información, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Compartir un formulario personalizado</a>.</p> <p>Importante: Si no tiene una licencia de planificación con acceso administrativo a Forms personalizado, debe tener permisos específicos para ver al menos el formulario personalizado, como se describe en <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Compartir un formulario personalizado</a>. Se le deben otorgar estos permisos incluso si el formulario es visible en todo el sistema. </p> <p>Para obtener información sobre cómo solicitar acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitud de acceso a objetos</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con su administrador de Workfront.

## Requisitos previos

El administrador de Workfront o un usuario con una licencia de planificación y acceso administrativo a los formularios personalizados deben crear formularios personalizados en su entorno para poder agregarlos a los objetos. Para obtener más información, consulte [Crear o editar un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Agregar un formulario personalizado a un objeto

Puede agregar un formulario personalizado a un objeto de dos formas:

* [Agregar un formulario personalizado a un objeto editando el objeto](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Agregar un formulario personalizado a un objeto desde el área de Detalles](#add-a-custom-form-to-an-object-from-the-details-area)

### Agregar un formulario personalizado a un objeto editando el objeto {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Vaya al objeto donde desea agregar el formulario personalizado.
1. Haga clic en **Más** menú ![](assets/more-icon.png), luego haga clic en **Editar** ![](assets/edit-icon.png).
1. Clic **Forms personalizado** > **Añadir Forms**, luego seleccione hasta 10 formularios en el menú desplegable.

1. (Opcional) Actualice la información de los campos editables del formulario personalizado.

   Debe actualizar todos los campos obligatorios en los formularios que agregue.

1. Haga clic en **Guardar**.

### Agregar un formulario personalizado a un objeto desde el área de Detalles {#add-a-custom-form-to-an-object-from-the-details-area}

1. Vaya al objeto donde desea agregar el formulario personalizado.
1. Haga clic en **`<Object type>`Detalles** en el panel izquierdo. Por ejemplo, haga clic en **Detalles del proyecto** para agregar formularios personalizados a un proyecto o **Detalles del problema** para agregar formularios personalizados a un problema.
1. Haga clic en **Añadir formulario personalizado** en la esquina superior derecha, seleccione hasta 10 formularios personalizados en la lista que se muestra.

   Si el formulario contiene campos obligatorios (marcados con un asterisco rojo), no tiene que completarlos en este momento.

   Los formularios seleccionados se adjuntan automáticamente al objeto.

1. (Opcional) Actualice la información en los campos personalizados del formulario y, a continuación, haga clic en **Guardar cambios**.

## Varios formularios personalizados en un objeto

Se pueden agregar hasta 10 formularios personalizados a un objeto determinado, lo que permite poner los campos a disposición de algunos usuarios y no de otros, o satisfacer mejor los requisitos de formulario de varios proyectos.

**Ejemplo:** Si un proyecto existente ya tiene un formulario personalizado y se necesitan más campos personalizados para este proyecto, que existen en otro formulario personalizado, puede agregar un segundo formulario al proyecto con los campos adicionales, en lugar de agregar los campos al formulario personalizado existente.

## Agregar un formulario personalizado a varios objetos de forma masiva

Puede agregar formularios personalizados a varios objetos seleccionándolos en una lista.

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>Agregar formularios personalizados a objetos es idéntico para todos los objetos, excepto para los proyectos.
>
>Para obtener información sobre cómo agregar formularios personalizados a proyectos de forma masiva, consulte el artículo [Editar proyectos](../../manage-work/projects/manage-projects/edit-projects.md).


1. Navegue hasta una lista de objetos.
1. Seleccione varios objetos de la lista.

1. Haga clic en **Más** menú ![](assets/more-icon.png), luego haga clic en **Editar** icono  ![](assets/edit-icon.png).

   O

   Haga clic en **Editar** icono ![](assets/edit-icon.png) al principio de la lista.
1. Clic **Forms personalizado** en el panel izquierdo.
1. en el **Realización de una selección** , seleccione el formulario que desea asociar con todos los objetos seleccionados.

   >[!NOTE]
   >
   >Si no encuentra el formulario en el menú desplegable, significa que al menos uno de los objetos ya tiene el formulario asociado. Determine qué objeto es y elimínelo de la selección antes de agregar el formulario a los objetos restantes.


1. Haga clic en **Guardar cambios**.

   Si el formulario contiene campos obligatorios (marcados con un asterisco rojo), no tiene que completarlos en este momento.
