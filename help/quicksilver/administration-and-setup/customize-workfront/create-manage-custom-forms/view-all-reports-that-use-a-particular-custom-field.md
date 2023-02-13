---
title: Ver todos los informes que utilizan un widget o campo personalizado en particular
description: Puede agregar una vista personalizada en el área Forms personalizada que muestre qué informes están usando un widget o campo personalizado en particular. Esto resulta útil cuando necesita editar o eliminar el campo o la utilidad, ya que puede que ya esté implementado en uno o más informes. Es importante evaluar si esos informes necesitarán ajustes para seguir funcionando correctamente.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 5d36c2c959dbfd00920eaf0a16409102b99de042
workflow-type: tm+mt
source-wordcount: '817'
ht-degree: 0%

---

# Ver todos los informes que utilizan un widget o campo personalizado en particular

Puede agregar una vista personalizada en el área Forms personalizada que muestre qué informes están usando un widget o campo personalizado en particular. Esto resulta útil cuando necesita editar o eliminar el campo o la utilidad, ya que puede que ya esté implementado en uno o más informes. Es importante evaluar si esos informes necesitarán ajustes para seguir funcionando correctamente.

Para obtener información sobre los campos personalizados y las utilidades de los formularios personalizados, consulte [Añadir un campo personalizado a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) y [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## Lista de los informes que utilizan un widget o campo personalizado en particular

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Abra el **Campos** para mostrar un informe con todos los campos y utilidades personalizados de la instancia de Workfront.

   ![](assets/fields-tab.png)

1. Haga clic en el **Ver** menú desplegable en el encabezado de la parte superior de la lista y, a continuación, compruebe si hay vistas personalizadas en la lista que incluyan la variable **Informes** (que no es una columna predeterminada de esta pestaña).

   En la columna Informes puede ver qué informes utilizan cada campo y utilidad personalizados que se han agregado a un formulario personalizado del sistema. Es posible que alguien ya haya creado una vista que incluya el **Informes** para abrir el Navegador.

1. Si no ve una vista que incluya la variable **Informes** , cree una nueva vista que la incluya:

   1. Haga clic en el **Ver** menú desplegable y haga clic en **Nueva vista**.

   1. En el **Nueva vista** que aparece, en el cuadro situado cerca de la esquina superior izquierda, sustituya **Nueva vista de parámetro** con un nombre descriptivo para la vista, como *Campos y utilidades*.

   1. Haga clic en **Agregar columna** cerca de la esquina inferior derecha.
   1. En el **Mostrar en esta columna** que aparece cerca de la esquina superior izquierda, empiece a escribir *informe* y, a continuación, seleccione **Informes** cuando aparezca en la lista debajo del cuadro.

   1. (Condicional) Si desea mover la variable **Informes** que acaba de agregar a una posición horizontal diferente, arrastre su encabezado en la **Vista previa de columna** en la parte inferior de la página.

   1. Haga clic en **Listo** y haga clic en **Guardar vista**.

1. Haga clic en el **Ver** menú desplegable y, a continuación, seleccione el nombre de la vista personalizada que acaba de crear.
1. En el **Nombre** , busque el campo personalizado o el widget que desea editar o eliminar y, a continuación, consulte la **Informes** para ver qué informes lo utilizan, si los hay.

   Para encontrar la información de esta columna, Workfront busca los campos personalizados y las utilidades en todos los filtros de informe, vistas y agrupaciones.

   Si ve un signo de suma, puede hacer clic en esa línea de texto para mostrar un cuadro con todos los informes adicionales que utilizan el campo o la utilidad.

   >[!NOTE]
   >
   >El tiempo de carga inicial de esta herramienta puede tardar entre 10 segundos y 2,5 minutos, dependiendo de la cantidad de datos del sistema.

   >[!TIP]
   >
   >Si no tiene tiempo para investigar los informes que utilizan el campo o la utilidad personalizados, puede hacer clic en Exportar para crear un archivo que los enumere. Puede compartir este archivo con cualquier persona que posea un informe que utilice el campo o la utilidad y discutir el cambio que debe producirse, el impacto que podría tener en el informe y lo que debe hacerse para asegurarse de que el informe siga funcionando correctamente.
   >
   >Esta vista también está disponible en un informe de parámetros:
   >      
   > 1. En el menú principal, haga clic en **Informes**.
   > 1. Cerca de la esquina superior izquierda, haga clic en **Nuevo informe** y haga clic en **Parámetro** en la lista que se muestra.
   > 1. Haga clic en **Agregar columna** cerca de la esquina inferior derecha.
   > 1. En el **Mostrar en esta columna** que aparece cerca de la esquina superior izquierda, empiece a escribir *informe* y, a continuación, seleccione **Informes** cuando aparezca en la lista debajo del cuadro.
   > 1. (Condicional) Si desea mover la variable **Informes** que acaba de agregar a una posición horizontal diferente, arrastre su encabezado en la **Vista previa de columna** en la parte inferior de la página.
   > 1. Haga clic en **Listo** y haga clic en **Guardar y cerrar**.
   > 1. Escriba un nombre descriptivo para el informe, como *Campos y utilidades*.

