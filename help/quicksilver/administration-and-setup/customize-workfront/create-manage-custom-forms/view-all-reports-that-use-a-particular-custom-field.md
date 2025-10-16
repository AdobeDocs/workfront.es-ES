---
title: Ver todos los informes que utilizan un campo personalizado o widget en particular
description: Puede agregar una vista personalizada en el área de Forms personalizado que muestre qué informes están usando un campo o widget personalizado en particular. Esto resulta útil cuando necesita editar o eliminar el campo o widget, porque es posible que ya esté implementado en uno o más informes. Es importante evaluar si esos informes necesitarán ajustes para seguir funcionando correctamente.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: eaafe79b-bdbc-4fb9-b449-23e5a4bc455a
source-git-commit: 15ac51cc13eeb57d2de194a9a6ceec7683acfbe6
workflow-type: tm+mt
source-wordcount: '750'
ht-degree: 7%

---

# Ver todos los informes que utilizan un campo o widget personalizado en particular

Puede agregar una vista personalizada en el área de Forms personalizado que muestre qué informes están usando un campo o widget personalizado en particular. Esto resulta útil cuando necesita editar o eliminar el campo o widget, porque es posible que ya esté implementado en uno o más informes. Es importante evaluar si esos informes necesitarán ajustes para seguir funcionando correctamente.

Para obtener información sobre los campos y widgets personalizados en los formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>Licencia de Adobe Workfront</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> </td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Enumerar los informes que utilizan un campo o widget personalizado en particular

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Formularios personalizados**.
1. Haga clic en **Campos** para mostrar un informe con todos los campos y widgets personalizados de la instancia de Workfront.

1. Haga clic en el menú **Ver** y, a continuación, compruebe si hay vistas personalizadas en la lista que incluyan la columna **Informes** (que no es una columna predeterminada en esta ficha).

   En la columna Informes se puede ver qué informes utilizan cada campo personalizado y widget que se ha agregado a un formulario personalizado del sistema. Es posible que alguien ya haya creado una vista que incluya la columna **Informes**.

1. Si no ve una vista que incluya la columna **Informes**, cree una nueva vista que la incluya:

   1. Haga clic en el menú **Ver** y, a continuación, haga clic en **Nueva vista**.

   1. En la página **Nueva vista** que aparece, en el cuadro cerca de la esquina superior izquierda, reemplace **Nueva vista de parámetro** con un nombre descriptivo para la vista, como *Campos y widgets*.

   1. Haga clic en **Agregar columna** cerca de la esquina inferior derecha.
   1. En el cuadro **Mostrar en esta columna** que aparece cerca de la esquina superior izquierda, empiece a escribir *informe* y, a continuación, seleccione **Informes** cuando aparezca en la lista debajo del cuadro.

   1. (Condicional) Si desea mover la columna **Informes** que acaba de agregar a una posición horizontal diferente, arrastre su encabezado al área **Vista previa de columna** en la parte inferior de la página.

   1. Haga clic en **Listo** y luego haga clic en **Guardar vista**.

1. Haga clic en el menú desplegable **Vista** y, a continuación, seleccione el nombre de la vista personalizada que acaba de crear.
1. En la columna **Nombre**, busque el campo o widget personalizado que planea editar o eliminar y, a continuación, observe la columna **Informes** de esa fila para ver qué informes lo utilizan, si los hay.

   Para encontrar la información de esta columna, Workfront busca los campos y widgets personalizados en todos los filtros, vistas y agrupaciones de informes.

   Si ve un signo más, puede hacer clic en esa línea de texto para mostrar un cuadro con todos los informes adicionales que utilicen el campo o widget.

   >[!NOTE]
   >
   >El tiempo de carga inicial de esta herramienta puede oscilar entre 10 segundos y 2,5 minutos, según la cantidad de datos del sistema.

   >[!TIP]
   >
   >Si no tiene tiempo para investigar los informes que utilizan el campo o widget personalizado, puede hacer clic en Exportar para crear un archivo que los enumere. Podría compartir este archivo con cualquier persona que sea propietaria de un informe que esté utilizando el campo o widget y discutir el cambio que debe producirse, el impacto que podría tener en el informe y lo que debe hacerse para asegurarse de que el informe sigue funcionando correctamente.
   >
   >Esta vista también está disponible en el informe Parámetro:
   >      
   > 1. En el menú principal, haga clic en **Informes**.
   > 1. Cerca de la esquina superior izquierda, haga clic en **Nuevo informe** y, a continuación, haga clic en **Parámetro** en la lista que se muestra.
   > 1. Haga clic en **Agregar columna** cerca de la esquina inferior derecha.
   > 1. En el cuadro **Mostrar en esta columna** que aparece cerca de la esquina superior izquierda, empiece a escribir *informe* y, a continuación, seleccione **Informes** cuando aparezca en la lista debajo del cuadro.
   > 1. (Condicional) Si desea mover la columna **Informes** que acaba de agregar a una posición horizontal diferente, arrastre su encabezado al área **Vista previa de columna** en la parte inferior de la página.
   > 1. Haga clic en **Listo**, luego **Guardar + Cerrar**.
   > 1. Escriba un nombre descriptivo para el informe, tal como *Campos y widgets*.
