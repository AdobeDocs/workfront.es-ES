---
title: Agregar lógica de visualización y saltar lógica a un formulario personalizado con el generador de formularios heredado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede decidir qué secciones de un formulario personalizado se deben mostrar o omitir en función de las opciones que realice un usuario al rellenarlo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '969'
ht-degree: 0%

---

# Agregar lógica de visualización y saltar lógica a un formulario personalizado con el generador de formularios heredado

{{form-designer-default}}

Puede decidir qué secciones de un formulario personalizado se deben mostrar o omitir en función de las opciones que realice un usuario al rellenarlo.

>[!NOTE]
>
>La lógica solo se aplica dentro de un formulario y no se puede basar en selecciones de un formulario diferente.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información acerca de cómo los administradores de Workfront conceden este acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder acceso administrativo a los usuarios a ciertas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber qué configuraciones de plan, tipo de licencia o nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones para utilizar la lógica de visualización y la lógica de omisión

* Para agregar lógica de visualización en un campo personalizado, widget o salto de sección, debe colocarse al menos un campo de opción múltiple (botones de opción, listas desplegables o casillas de verificación) antes de él en el formulario.

  Para obtener información sobre los campos y widgets personalizados en los formularios personalizados, consulte [Agregar un campo personalizado a un formulario personalizado con el generador de formularios heredados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) y [Agregar o editar un widget de recursos en un formulario personalizado con el generador de formularios heredados](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* No se puede agregar lógica de omisión a un widget o salto de sección. Solo puede agregarlo a un campo de opción múltiple (botones de opción, listas desplegables o casillas de verificación).

* Puede agregar lógica de visualización y lógica de omisión a un campo personalizado si se cumplen todas las condiciones siguientes en relación con el campo personalizado:

   * Es un campo de opción múltiple (botones de opción, listas desplegables o casillas de verificación)
   * Va precedido de un campo de opción múltiple
   * Va seguido de otro campo personalizado

* Al copiar formularios con lógica de visualización u lógica de omisión, la lógica se copia en el nuevo formulario personalizado.
* Al editar objetos de forma masiva, todos los campos personalizados se muestran en el cuadro Editar objetos, incluidos los campos omitidos u ocultos.
* Tenga en cuenta lo siguiente al crear una regla de lógica de visualización para un formulario personalizado:

   * De forma predeterminada, los campos personalizados no incluidos en una instrucción de lógica de visualización se muestran en un formulario personalizado.
   * Puede crear instrucciones de lógica de visualización de varios campos.
   * Si se les ha aplicado lógica de visualización a todos los campos debajo de un salto de sección y, como resultado de la lógica, todos ellos están ocultos, toda la sección estará oculta en el formulario personalizado.

## Crear un formulario personalizado de ejemplo con lógica de visualización y omisión

La mejor manera de aprender a agregar lógica de visualización y omisión a un formulario personalizado es a través del ejemplo práctico que se explica en las dos secciones siguientes:

### Mostrar lógica {#display-logic}

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Forms personalizado**.

1. Cree el formulario personalizado de ejemplo:

   1. Haga clic en **Nuevo formulario personalizado** y, a continuación, haga clic en **Proyecto** en la lista desplegable.

   1. En el cuadro **Título del formulario**, escriba **Formulario personalizado de ejemplo: lógica de visualización de aprendizaje y lógica de omisión**.

   1. Haga clic en **Agregar campo** en la esquina superior izquierda.
   1. Agregue un campo desplegable llamado *Campo de problema* haciendo clic en **Menú desplegable** y escribiendo **Campo de problema** en el cuadro **Etiqueta**.

   1. En **Opciones**, agregue las siguientes opciones en los cuadros de texto:

      Investigación necesaria

      No más investigación

   1. Haga clic en **Guardar + Cerrar** en la esquina inferior izquierda.

1. Seleccione el nuevo formulario personalizado de ejemplo **Ejemplo: lógica de visualización de aprendizaje, omita la lógica** y haga clic en **Editar**.

1. Agregue un nuevo campo de texto de una sola línea denominado *Otro estudio* haciendo clic en **Campo de texto de una sola línea** y, a continuación, escribiendo **Otro estudio** en el cuadro **Etiqueta**.

1. Haga clic en **Agregar lógica** cerca de la parte inferior izquierda de la pantalla **Editar formulario personalizado**.

1. En el cuadro que aparece, con la ficha **Lógica de visualización** abierta, configure la lógica para cuándo aparecerá el campo **Otras investigaciones** en el formulario haciendo clic en **Campo de problema** en la primera lista desplegable, **Se necesita investigación** en la segunda lista desplegable y **Seleccionado** en la tercera lista desplegable.
1. Haga clic en **Guardar** para cerrar la ventana de **Lógica de campo** y, a continuación, haga clic en **Listo** en el área de **Configuración de campo**.

   Ahora, cuando alguien seleccione **Se necesita investigación** en la lista desplegable de **Campo de problema**, se mostrará el campo **Otra investigación**.

1. Haga clic en **Vista previa** para asegurarse de que la lógica aparece del modo que desee en el formulario.
1. Haga clic en **Finalizar vista previa** cuando descubra que la lógica funciona según lo esperado.
1. Haga clic en **Guardar y cerrar** en la ventana **Editar formulario personalizado** para guardar el formulario y, a continuación, continúe con [Omitir lógica](#skip-logic) a continuación.

### Omitir lógica {#skip-logic}

La lógica de omisión funciona de manera similar a la lógica de visualización, pero actúa como lo contrario: en lugar de hacer que aparezcan campos de opción múltiple personalizados específicos basados en selecciones específicas, usted determina cuáles deben omitirse, según las selecciones de los usuarios.

Para obtener más información, siga trabajando en el formulario personalizado de ejemplo que creó en la sección [Lógica de visualización](#display-logic) de este artículo:

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Haga clic en **Forms personalizado**.
1. Seleccione el formulario **Formulario personalizado de ejemplo: lógica de visualización de aprendizaje, omita la lógica** que creó en los pasos anteriores y, a continuación, haga clic en **Editar**.

1. Seleccione el campo desplegable que creó denominado *Campo de problema*.
1. Haga clic en el botón **Agregar lógica** en la barra lateral de **Configuración de campo**.

1. En el cuadro **Lógica de campo**, asegúrese de que la ficha **Omitir lógica** esté seleccionada.

1. Establezca la primera lista desplegable en **No más investigaciones** y la segunda lista desplegable en **Seleccionado**.

1. En el menú desplegable **Pasar a**, seleccione **Fin del formulario.**

   Ahora, cuando alguien selecciona **No más investigaciones** en el campo desplegable **Campo de problema**, el formulario se saltará directamente al final del formulario sin mostrar el campo **Otras investigaciones**.

1. Haga clic en **Guardar**.
1. Haga clic en **Vista previa** para asegurarse de que la lógica se aplica como usted lo desea.
1. Haga clic en **Listo** en la parte inferior izquierda del formulario.
