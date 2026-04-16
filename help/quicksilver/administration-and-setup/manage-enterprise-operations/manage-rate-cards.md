---
user-type: administrator
product-area: system-administration;setup
navigation-topic: manage-rate-cards
title: Administrar tarjetas de tarifas
description: Una tarjeta de tarifas representa el acuerdo contractual con su cliente en el que se definen las tarifas por hora para los roles que completarán el trabajo. En una tarjeta de tarifas, puede definir varias tarifas de facturación por rol, según los atributos.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 3972f498-c461-4535-82c6-ad1b60d3ed86
source-git-commit: c27dd9d972b89af09c0865a0e878f1665416c80e
workflow-type: tm+mt
source-wordcount: '1337'
ht-degree: 14%

---

# Administrar tarjetas de tarifas

Una tarjeta de tarifas representa el acuerdo contractual con su cliente en el que se definen las tarifas por hora para los roles que completarán el trabajo. En una tarjeta de tarifas, puede definir varias tarifas de facturación por rol, según atributos como agencia, ubicación o centro de coste. Los atributos de tarifa únicos se configuran en el área Configuración. Para obtener más información, vea [Definir atributos de tasa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

Por ejemplo, podría tener una función de Designer con sede en París para la Agencia A, otra Designer con sede en París para la Agencia B y una tercera Designer con sede en Nueva York no asignada a una agencia, cada una con diferentes tarifas de facturación. Sin embargo, los atributos no son necesarios para las funciones del puesto en una tarjeta de tasas. Los atributos sirven como herramientas para establecer tasas más granulares. Una tarifa de facturación en una tarjeta de tarifas también puede ser efectiva por fecha, de manera que la tarifa comience y termine en fechas especificadas.

También puede bloquear las tarifas en una tarjeta de tarifas para evitar que se anulen en el nivel de proyecto o tarea. Las tarifas bloqueadas son las más altas de la jerarquía de tarifas de facturación, excepto para las tarifas conservadas de un proyecto. Para obtener más información, consulte [Información general sobre la jerarquía de ingresos y costos](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td>Workflow Ultimate</td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td>[!UICONTROL Standard]</td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Editar acceso a [!UICONTROL Rate Cards]</td> 
  </tr> 
  <tr> 
   <td>Permisos de objeto</td> 
   <td>Para editar una tarjeta de tarifas compartida con usted, debe tener permisos de administración en la tarjeta de tarifas.</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Añadir una tarjeta de tarifas

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifas**].
1. Haz clic en [!UICONTROL **Nueva tarjeta de tarifa**] y luego haz clic en [!UICONTROL **Crear nueva tarjeta de tarifa**].
1. Escriba un nombre y una descripción para la tarjeta de tarifas en el cuadro [!UICONTROL **Nueva tarjeta de tarifas**].

   El nombre debe ser único.

   ![Nuevo cuadro de diálogo de tarjeta de tarifa](assets/new-rate-card-dialog.png)

1. (Opcional) Seleccione un [!UICONTROL **Grupo**] para la tarjeta de tarifas. Esta es la agencia que define la tarjeta de tarifas.
1. (Opcional) Seleccione una [!UICONTROL **Compañía**] para la tarjeta de tarifas. Este es el cliente para el que se contratan las tarifas.

   >[!NOTE]
   >
   >El Grupo y la Empresa no solo se utilizan en los detalles de la tarjeta de tarifas, sino también como filtros al adjuntar una tarjeta de tarifas a un proyecto.

1. Haga clic en **Crear**.

   Aparecerá la pantalla Tarjeta de tarifas > Funciones del puesto y tarifas.

1. Haga clic en [!UICONTROL **Agregar rol**].
1. En el cuadro [!UICONTROL **Nueva tarifa de facturación**], seleccione un [!UICONTROL **Rol**] para definir tarifas de facturación para.

   ![Nuevo cuadro de diálogo de tarifa de facturación](assets/new-job-role-rate-on-rate-card.png)

1. (Opcional) Seleccione atributos para la tasa de facturación como Agencia, Ubicación o Centro de Coste.

   >[!NOTE]
   >
   >Estos atributos se definen por separado y pueden afectar a los cálculos de ingresos y costes. Para obtener más información, vea [Definir atributos de tasa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

1. Seleccione una [!UICONTROL **Moneda**] para la tarifa de facturación.
1. (Opcional) Escriba un [!UICONTROL **alias de rol**] para el rol.

   Si el nombre de alias que escribe no existe, puede agregarlo.

   Cuando la tarjeta de tasas se adjunta a un proyecto, el alias aparece en información como asignaciones de marcador de posición, gastos e informes, en lugar del nombre de rol interno.

   >[!NOTE]
   >
   >* Solo puede existir un alias para cada combinación de rol y atributo dentro de una sola tarjeta de tarifa.
   >* Un alias debe actualizarse en la tarjeta de tarifas y no se puede editar en un proyecto.

1. En el campo [!UICONTROL **Tarifa de facturación**], introduzca la tarifa de facturación para este rol y sus atributos.
1. (Opcional) Seleccione [!UICONTROL **Tasa de bloqueo**] para bloquear esta tasa y no permitir que se cambie en el nivel de proyecto o tarea. Puede desbloquearlo más tarde si es necesario.
1. (Opcional) Haga clic en [!UICONTROL **Agregar tarifa vigente por fecha**] para aplicar fechas efectivas a la tarifa de facturación.
1. (Opcional) Haga clic de nuevo en [!UICONTROL **Agregar tarifa vigente por fecha**] para agregar más tarifas de facturación con fechas efectivas para este rol y sus atributos.
1. (Condicional) Si agrega más de una tarifa de facturación para este rol, introduzca la siguiente información:

   * [!UICONTROL **Tarifa de facturación**]: Valor de la tarifa de facturación para el período de tiempo.
   * [!UICONTROL **Fecha de inicio**]: La fecha en la que comienza la tarifa.
   * [!UICONTROL **Fecha de finalización**]: fecha en la que finaliza la tarifa.

     La primera tarifa de facturación no es necesaria para tener una fecha de inicio y la última tarifa de facturación no es necesaria para tener una fecha de finalización. Se permiten espacios entre las fechas de tarifa, pero no fechas superpuestas. Durante un espacio, se utilizan otras áreas de la jerarquía de tarifas de facturación para determinar la tasa de facturación, según el tipo de ingresos de una tarea. Para obtener más información, consulte [Información general sobre la jerarquía de ingresos y costos](/help/quicksilver/manage-work/projects/project-finances/overview-revenue-cost-hierarchy.md).

1. Haga clic en [!UICONTROL **Guardar**].
1. (Opcional) Para agregar otra tarifa de facturación, ya sea para el mismo rol con atributos diferentes o para un rol separado, haga clic en [!UICONTROL **Agregar rol**].

   Las tarifas de cada rol se añaden a la tarjeta de tarifas a medida que las crea. La tarifa vigente actualmente, basada en las fechas, se indica con un icono ![Icono de tarifa actual](assets/current-rate-icon.png).

   ![Tarjeta de tarifa con tarifas mostradas](assets/rates-on-rate-card.png)

## Editar detalles y tarifas de la tarjeta de tarifas

{{step-1-to-setup}}

1. El panel de navegación izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifas**].
1. Para editar una tarjeta de tarifa existente, haga clic en el nombre de la tarjeta de tarifa en la lista Tarjetas de tarifa.
1. Para actualizar los detalles de la tarjeta de tarifas, haga clic en [!UICONTROL **Detalles**] en el panel izquierdo.
1. (Opcional) Para adjuntar un formulario personalizado a la tarjeta de tarifas, haga clic en el campo [!UICONTROL **Agregar formulario personalizado**] en la esquina superior derecha de la página Detalles y seleccione un formulario personalizado de la lista que se muestra.

   Para obtener más información sobre cómo adjuntar un formulario personalizado, vea [Añadir un formulario personalizado a un objeto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Haga clic en [!UICONTROL **Guardar cambios**] después de editar los detalles de la tarjeta de tarifas.
1. Haga clic en [!UICONTROL **Funciones y tarifas del puesto**] en el panel izquierdo para editar las tarifas de facturación.
1. Para editar una tarifa, selecciona la casilla de verificación que está junto a la tarifa y haz clic en [!UICONTROL **Editar**] en la barra de acciones de la parte inferior de la pantalla.

   Para obtener más información acerca de la barra de acciones, vea [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

   >[!NOTE]
   >
   >Dado que cada tasa está asociada a la combinación de la función y los atributos para crear una tasa única, la función y los atributos no se pueden cambiar al editar una tasa.

1. Para eliminar una tarifa de facturación de la tarjeta de tarifas, selecciona la casilla junto a la tarifa y haz clic en [!UICONTROL **Eliminar**] en la barra de acciones.
1. Para bloquear una tarifa, selecciona la casilla de verificación situada junto a la tarifa y haz clic en [!UICONTROL **Bloquear**] en la barra de acciones.

   Las tarifas bloqueadas no se pueden cambiar en el nivel de proyecto o tarea. Aparece un icono de candado junto a las tarifas bloqueadas en la lista.

   También puede desbloquear una velocidad bloqueada desde la barra de acciones.

1. Para ajustar las tasas en un porcentaje, siga estos pasos:

   1. Seleccione todas las tarifas que desee ajustar en la pantalla Tarjeta de tarifas > Funciones del puesto y tarifas.

      Puede elegir una o varias tarifas. Todos se ajustarán en el mismo porcentaje.

   1. Haga clic en [!UICONTROL **Ajustar tasas**] en la barra de acciones.
   1. En el cuadro [!UICONTROL **Ajustar las tasas de rol**], elija si desea que el ajuste de tasa se produzca durante el período de tiempo seleccionado (las fechas en vigor existentes) o un intervalo de fecha personalizado que defina.

      ![Ajustar tarifas de rol](assets/adjust-job-role-rates-dialog.png)

   1. Introduzca el valor de ajuste de los tipos.

      Este valor se aplica como porcentaje. Por ejemplo, si introduce 10, las tasas seleccionadas aumentarán un 10 %.

   1. Haga clic en [!UICONTROL **Actualizar tarifas**].
   1. Haga clic en [!UICONTROL **Actualizar**] en el mensaje de confirmación.

      Las tasas seleccionadas se incrementan en función del porcentaje.

## Importar una tarjeta de tarifas

Consulte el artículo [Importar tarjetas de tarifa desde una plantilla](/help/quicksilver/administration-and-setup/manage-enterprise-operations/import-rate-cards.md).

## Copiar una tarjeta de tarifas

{{step-1-to-setup}}

1. El panel de navegación izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifas**].
1. Seleccione la casilla de verificación situada junto a la tarjeta de tarifas de la lista y haga clic en el icono **Copiar** ![Copiar icono](assets/copy-icon.png).
1. Escriba un nombre para la nueva tarjeta de tarifas en el cuadro [!UICONTROL **Copiar tarjeta de tarifas**]. A continuación, haga clic en [!UICONTROL **Crear**].

   Se guardará la nueva tarjeta de tarifas. Edite los detalles de la tarjeta de tarifas, las funciones y las tarifas, según sea necesario.

## Eliminar una tarjeta de tarifas

{{step-1-to-setup}}

1. En el panel de navegación izquierdo, haga clic en [!UICONTROL **Tarjetas de tarifas**].
1. Seleccione la casilla de verificación situada junto a la tarjeta de tarifas de la lista y haga clic en el icono **Eliminar** ![Eliminar icono](assets/delete.png).

   >[!NOTE]
   >
   >Una tarjeta de tarifas adjunta se eliminará del proyecto.

