---
title: Agregar lógica de visualización y saltar lógica a un formulario personalizado con el generador de formularios heredado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede decidir qué secciones de un formulario personalizado se deben mostrar o omitir en función de las opciones que realice un usuario al rellenarlo.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c687c4a8-a99d-4ac0-b785-5bfe503a7e2c
source-git-commit: 7835b5f9b5903e19b03cb7e25bfae37c9739f064
workflow-type: tm+mt
source-wordcount: '917'
ht-degree: 0%

---

# Agregar lógica de visualización y saltar lógica a un formulario personalizado con el generador de formularios heredado

Puede decidir qué secciones de un formulario personalizado se deben mostrar o omitir en función de las opciones que realice un usuario al rellenarlo.

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
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber qué configuraciones de plan, tipo de licencia o nivel de acceso tiene, póngase en contacto con su administrador de Workfront.

## Consideraciones para utilizar la lógica de visualización y la lógica de omisión

* Para agregar lógica de visualización en un campo personalizado, widget o salto de sección, debe colocarse al menos un campo de opción múltiple (botones de opción, lista desplegable o casillas de verificación) antes de él en el formulario.

   Para obtener información sobre los campos y widgets personalizados en los formularios personalizados, consulte [Agregar un campo personalizado a un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) y [Agregar o editar un widget de recursos en un formulario personalizado con el generador de formularios heredado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

* No se puede agregar lógica de omisión a un widget o salto de sección. Solo puede agregarlo a un campo de opción múltiple (botones de opción, listas desplegables o casillas de verificación).

* Puede agregar lógica de visualización y lógica de omisión a un campo personalizado. Todo lo siguiente es verdadero en relación con el campo personalizado:

   * Es un campo de opción múltiple (botones de opción, listas desplegables o casillas de verificación)
   * Va precedido de un campo de opción múltiple
   * Va seguido de otro campo personalizado

* Al copiar formularios con lógica de visualización u lógica de omisión, la lógica se copia en el nuevo formulario personalizado.
* Tenga en cuenta lo siguiente al crear una regla de lógica de visualización para un formulario personalizado

   * De forma predeterminada, los campos personalizados no incluidos en una instrucción de lógica de visualización se muestran en un formulario personalizado.
   * Puede crear instrucciones de lógica de visualización de varios campos.

* Al editar objetos de forma masiva, todos los campos personalizados se muestran en el cuadro Editar objetos, incluidos los campos omitidos u ocultos.

## Crear un formulario personalizado de ejemplo con lógica de visualización y omisión

La mejor manera de aprender a agregar lógica de visualización y omisión a un formulario personalizado es a través del ejemplo práctico que se explica en las dos secciones siguientes:

* [Mostrar lógica](#display-logic)
* [Omitir lógica](#skip-logic)

### Mostrar lógica {#display-logic}

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Forms personalizado** ![](assets/custom-forms-icon.png).

1. Cree el formulario personalizado de ejemplo:

   1. Clic **Nuevo formulario personalizado**, luego haga clic en **Proyecto** en la lista desplegable.

   1. En el **Título del formulario** cuadro, tipo **Formulario personalizado de ejemplo: lógica de visualización de aprendizaje y lógica de omisión**.

   1. Clic **Añadir un campo** en la esquina superior izquierda.
   1. Añada un campo desplegable llamado *Campo de problema* haciendo clic en **Desplegable** y, a continuación, escriba **Campo de problema** en el **Etiqueta** cuadro.

   1. En **Opciones**, agregue las siguientes opciones en los cuadros de texto:

      Investigación necesaria

      No más investigación

   1. Clic **Guardar + Cerrar** en la esquina inferior izquierda.

1. Seleccione el nuevo **Formulario personalizado de ejemplo: lógica de visualización de aprendizaje y lógica de omisión** formulario personalizado y haga clic en **Editar**.

1. Agregue un nuevo campo de texto de una sola línea llamado *Otras investigaciones* haciendo clic en **Campo de texto de línea única** y, a continuación, escriba **Otras investigaciones** en el **Etiqueta** cuadro.

1. Clic **Agregar lógica** cerca del lado inferior izquierdo del **Editar formulario personalizado** pantalla.

1. En el cuadro que aparece, con la etiqueta **Lógica de visualización** Abra la pestaña, configure la lógica para cuando el **Otras investigaciones** aparecerá en el formulario al hacer clic en **Campo de problema** en la primera lista desplegable, **Investigación necesaria** en la segunda lista desplegable, y **Seleccionado** en la tercera lista desplegable.
1. Clic **Guardar** para cerrar el **Lógica de campo** y haga clic en **Listo** en el **Configuración de campo** área.

   Ahora, cuando alguien selecciona **Investigación necesaria** en el **Campo de problema** desplegable, la variable **Otras investigaciones** se mostrará el campo.

1. Clic **Previsualizar** para asegurarse de que la lógica aparece del modo que desea en el formulario.
1. Clic **Finalizar previsualización** cuando descubra que la lógica funciona según lo esperado.
1. Clic **Guardar + Cerrar** en el **Editar formulario personalizado** para guardar el formulario y, a continuación, continúe en [Omitir lógica](#skip-logic) más abajo.

### Omitir lógica {#skip-logic}

La lógica de omisión funciona de manera similar a la lógica de visualización, pero actúa como lo contrario: en lugar de hacer que aparezcan campos de opción múltiple personalizados específicos basados en selecciones específicas, usted determina cuáles deben omitirse, según las selecciones de los usuarios.

Para obtener más información, siga trabajando en el formulario personalizado de ejemplo que ha creado en la sección [Mostrar lógica](#display-logic) en este artículo:

1. Haga clic en **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Clic **Forms personalizado**.
1. Selección del formulario **Formulario personalizado de ejemplo: lógica de visualización de aprendizaje y lógica de omisión** que creó en los pasos anteriores y haga clic en **Editar**.

1. Seleccione el campo desplegable que ha creado denominado *Campo de problema*.
1. Haga clic en **Agregar lógica** botón en el **Configuración de campo** barra lateral.

1. En el **Lógica de campo** , asegúrese de que la **Omitir lógica** está seleccionada.

1. Establezca la primera lista desplegable en **No más investigación** y la segunda lista desplegable a **Seleccionado**.

1. En el **Entonces Saltar A** menú desplegable, seleccione **Fin del formulario.**

   Ahora, cuando alguien selecciona **No más investigación** en el **Campo de problema** , el formulario se saltará directamente al final del formulario sin mostrar el campo de **Otras investigaciones** field.

1. Haga clic en **Guardar**.
1. Clic **Previsualizar**  para asegurarse de que la lógica se aplica de la manera que desee.
1. Clic **Listo** en la parte inferior izquierda del formulario.
