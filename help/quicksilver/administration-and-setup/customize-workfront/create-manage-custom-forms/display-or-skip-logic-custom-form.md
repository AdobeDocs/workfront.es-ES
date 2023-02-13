---
title: Agregar lógica de visualización y de omisión de lógica a un formulario personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede decidir qué secciones de un formulario personalizado deben mostrarse o omitirse en función de las opciones que elija un usuario al rellenarlo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: 59e3b958dd81f2f068bc06c3fe439de0084f9ce4
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 0%

---

# Agregar lógica de visualización y de omisión de lógica a un formulario personalizado

Puede decidir qué secciones de un formulario personalizado deben mostrarse o omitirse en función de las opciones que elija un usuario al rellenarlo.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Consideraciones sobre el uso de la lógica de visualización y la lógica de omisión

* Para agregar lógica de visualización en un campo personalizado, widget o salto de sección, se debe colocar al menos un campo de opción múltiple (botones de opción, menú desplegable o casillas de verificación) antes de colocarlo en el formulario.

   Para obtener información sobre los campos personalizados y las utilidades de los formularios personalizados, consulte [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) y [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* No se puede agregar la lógica de omisión a un widget o a un salto de sección. Solo se puede agregar a un campo de opción múltiple (botones de opción, desplegables o casillas de verificación).

* Puede agregar lógica de visualización y de omisión a un campo personalizado. Todo lo siguiente es verdadero sobre el campo personalizado:

   * Se trata de un campo de opción múltiple (botones de opción, menú desplegable o casillas de verificación)
   * Está precedido por un campo de opción múltiple
   * Le sigue otro campo personalizado

* Al copiar formularios con lógica de visualización o de omisión, la lógica se copia en el nuevo formulario personalizado.
* Tenga en cuenta lo siguiente al crear una regla de lógica de visualización para un formulario personalizado

   * Los campos personalizados no incluidos en una instrucción de lógica de visualización se muestran en un formulario personalizado de forma predeterminada.
   * Puede crear instrucciones de lógica de visualización de varios campos.

* Al editar objetos de forma masiva, todos los campos personalizados se muestran en el cuadro Editar objetos , incluidos los campos omitidos u ocultos.

## Crear un formulario personalizado de ejemplo con lógica de visualización y omisión

La mejor manera de aprender a agregar lógica de visualización y omisión a un formulario personalizado es mediante el ejemplo práctico explicado en las dos secciones siguientes:

* [Mostrar lógica](#display-logic)
* [Omitir lógica](#skip-logic)

### Mostrar lógica {#display-logic}

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Forms personalizado** ![](assets/custom-forms-icon.png).

1. Cree el formulario personalizado de ejemplo:

   1. Haga clic en **Nuevo formulario personalizado** y haga clic en **Proyecto** en la lista desplegable .

   1. En el **Título del formulario** cuadro, tipo **Formulario personalizado de ejemplo: aprendizaje de la lógica de visualización y la lógica de omisión**.

   1. Haga clic en **Agregar un campo** en la esquina superior izquierda.
   1. Añada un campo desplegable llamado *Campo de problema* haciendo clic en **Lista desplegable** y, a continuación, escriba **Campo Problema** en el **Etiqueta** en la ventana

   1. En **Opciones**, agregue las siguientes opciones en los cuadros de texto:

      Investigación necesaria

      No más investigación

   1. Haga clic en **Guardar + Cerrar** en la esquina inferior izquierda.

1. Seleccione el nuevo **Formulario personalizado de ejemplo: aprendizaje de la lógica de visualización y la lógica de omisión** formulario personalizado y, a continuación, haga clic en **Editar**.

1. Agregue un nuevo campo de texto de una sola línea llamado *Otras investigaciones* haciendo clic en **Campo de texto de una sola línea** y, a continuación, escriba **Otras investigaciones** en el **Etiqueta** en la ventana

1. Haga clic en **Agregar lógica** cerca del lado inferior izquierdo del **Editar formulario personalizado** en el Navegador.

1. En el cuadro que aparece, con la variable **Mostrar lógica** abra la pestaña , configure la lógica de cuándo se abre la **Otras investigaciones** aparecerá en el formulario haciendo clic en **Campo Problema** en la primera lista desplegable, **Investigación necesaria** en la segunda lista desplegable, y **Seleccionado** en la tercera lista desplegable.
1. Haga clic en **Guardar** para cerrar el **Lógica del campo** y, a continuación, haga clic en **Listo** en el **Configuración de campos** .

   Ahora, cuando alguien selecciona **Investigación necesaria** en el **Campo Problema** lista desplegable, **Otras investigaciones** se muestra el campo .

1. Haga clic en **Vista previa** para asegurarse de que la lógica aparece del modo deseado en el formulario.
1. Haga clic en **Finalizar vista previa** cuando encuentre que la lógica funciona según lo esperado.
1. Haga clic en **Guardar + Cerrar** en el **Editar formulario personalizado** para guardar el formulario y, a continuación, continúe con [Omitir lógica](#skip-logic) más abajo.

### Omitir lógica {#skip-logic}

La lógica Skip funciona de forma similar a la lógica de visualización, pero actúa de forma inversa: en lugar de hacer que aparezcan campos personalizados específicos de opción múltiple basados en selecciones específicas, se determinan cuáles se deben omitir en función de las selecciones de los usuarios.

Para obtener más información, siga trabajando en el formulario personalizado de ejemplo que ha creado en la sección [Mostrar lógica](#display-logic) en este artículo:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Forms personalizado**.
1. Seleccione el formulario **Formulario personalizado de ejemplo: aprendizaje de la lógica de visualización y la lógica de omisión** que ha creado en los pasos anteriores y, a continuación, haga clic en **Editar**.

1. Seleccione el campo desplegable que ha creado con el nombre *Campo Problema*.
1. Haga clic en el **Agregar lógica** en el **Configuración de campos** barra lateral.

1. En el **Lógica del campo** asegúrese de que la variable **Omitir lógica** está seleccionada.

1. Defina la primera lista desplegable como **No más investigación** y la segunda lista desplegable a **Seleccionado**.

1. En el **A Continuación, Pasar A** desplegable, seleccione **Fin del formulario.**

   Ahora, cuando alguien selecciona **No más investigación** en el **Campo Problema** campo desplegable, el formulario se saltará directamente al final del formulario sin mostrar la variable **Otras investigaciones** campo .

1. Haga clic en **Guardar**.
1. Haga clic en **Vista previa**  para asegurarse de que la lógica se aplica de la manera que desea.
1. Haga clic en **Listo** en la parte inferior izquierda del formulario.
