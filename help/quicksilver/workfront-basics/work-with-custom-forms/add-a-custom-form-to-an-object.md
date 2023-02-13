---
product-area: projects;user-management
keywords: adjuntar,aplicar
navigation-topic: work-with-custom-forms
title: Adición de un formulario personalizado a un objeto
description: Puede agregar un formulario personalizado existente a cualquiera de los objetos que se enumeran a continuación. Un formulario personalizado contiene campos personalizados en los que se puede almacenar información sobre el objeto.
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '816'
ht-degree: 1%

---

# Adición de un formulario personalizado a un objeto

Puede agregar un formulario personalizado existente a cualquiera de los objetos que se enumeran a continuación. Un formulario personalizado contiene campos personalizados en los que se puede almacenar información sobre el objeto.

* Proyectos (incluidos casos empresariales)
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

Puede agregar un formulario personalizado solamente a los tipos de objetos para los que se creó el formulario.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar las acciones descritas en este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a los objetos para los que se administran formularios personalizados</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p>Administre permisos al objeto para el que desea adjuntar un formulario personalizado.</p> <p>Ver o permisos superiores del formulario personalizado, con permiso para <b>Adjuntar a datos personalizados</b> objetos (proyectos, tareas y problemas). Para obtener más información, consulte <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Compartir un formulario personalizado</a>.</p> <p>Importante: Si no tiene una licencia de Plan con acceso administrativo a Forms personalizado, debe tener permisos específicos para ver al menos el formulario personalizado, tal como se describe en <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Compartir un formulario personalizado</a>. Estos permisos deben concederse incluso si el formulario es visible en todo el sistema. </p> <p>Para obtener información sobre la solicitud de acceso adicional, consulte <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Solicitar acceso a objetos </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Requisito previo

El administrador de Workfront o un usuario con una licencia de Plan y acceso administrativo a formularios personalizados deben crear formularios personalizados en su entorno para poder agregarlos a los objetos. Para obtener más información, consulte [Crear o editar un formulario personalizado](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## Adición de un formulario personalizado a un objeto

Puede agregar un formulario personalizado a un objeto de dos maneras:

* [Agregar un formulario personalizado a un objeto editando el objeto](#add-a-custom-form-to-an-object-by-editing-the-object)
* [Agregar un formulario personalizado a un objeto desde el área Detalles](#add-a-custom-form-to-an-object-from-the-details-area)

### Agregar un formulario personalizado a un objeto editando el objeto {#add-a-custom-form-to-an-object-by-editing-the-object}

1. Vaya al objeto en el que desea agregar el formulario personalizado.
1. Haga clic en el **Más** menú ![](assets/more-icon.png)y haga clic en **Editar** ![](assets/edit-icon.png).
1. Haga clic en **Forms personalizado** > **Añadir Forms** y, a continuación, seleccione hasta 10 formularios en el menú desplegable.

1. (Opcional) Actualice la información en los campos editables del formulario personalizado.

   Debe actualizar todos los campos obligatorios en los formularios que agregue.

1. Haga clic en **Guardar**.

### Agregar un formulario personalizado a un objeto desde el área Detalles {#add-a-custom-form-to-an-object-from-the-details-area}

1. Vaya al objeto en el que desea agregar el formulario personalizado.
1. Haga clic en el **`<Object type>`Detalles** en el panel izquierdo. Por ejemplo, haga clic en **Detalles del proyecto** para agregar formularios personalizados a un proyecto o **Detalles del problema** para agregar formularios personalizados a un problema.
1. Haga clic en el **Agregar formulario personalizado** en la esquina superior derecha y, a continuación, seleccione hasta 10 formularios personalizados de la lista que se muestra.

   Si el formulario contiene campos obligatorios (marcados con un asterisco rojo), no es necesario completarlos en este momento.

   Los formularios seleccionados se adjuntan automáticamente al objeto.

1. (Opcional) Actualice la información en los campos personalizados del formulario y haga clic en **Guardar cambios**.

## Varios formularios personalizados en un objeto

Puede agregar hasta 10 formularios personalizados en un objeto determinado, lo que le permite poner los campos a disposición de algunos usuarios y no de otros, o permitirle cumplir mejor los requisitos de formulario de varios proyectos.

**Ejemplo:** Si un proyecto existente ya tiene un formulario personalizado y se necesitan más campos personalizados que existan en otro formulario personalizado, puede agregar un segundo formulario al proyecto con los campos adicionales en lugar de agregar los campos al formulario personalizado existente, si esos campos son necesarios solo para este proyecto.

## Agregar un formulario personalizado a varios objetos de forma masiva

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit is released for NWE) </p>
-->

Para agregar formularios personalizados a varios objetos, selecciónelos en una lista.

1. Vaya a una lista de objetos.
1. Seleccione varios objetos de la lista.

1. Haga clic en el **Más** menú ![](assets/more-icon.png)y, a continuación, haga clic en el botón **Editar** icono  ![](assets/edit-icon.png)o haga clic en el botón **Editar** icono ![](assets/edit-icon.png).
1. Haga clic en **Forms personalizado** en el panel izquierdo.
1. En el **Realización de una selección** menú desplegable, seleccione el formulario que desee asociar a todos los objetos seleccionados.

   >[!NOTE]
   >
   >Si no encuentra el formulario en el menú desplegable, significa que al menos uno de los objetos tiene el formulario ya asociado. Determine qué objeto es y elimínelo de la selección antes de agregar el formulario a los objetos restantes.

1. Haga clic en **Guardar cambios**.

   Si el formulario contiene campos obligatorios (marcados con un asterisco rojo), no es necesario completarlos en este momento.
