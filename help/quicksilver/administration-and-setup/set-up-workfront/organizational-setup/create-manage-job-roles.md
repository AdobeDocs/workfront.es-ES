---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: organization-setup
title: Crear y administrar roles
description: Como [!DNL Adobe Workfront] administrador o usuario con acceso administrativo a las funciones, puede crear funciones que se pueden asignar a usuarios y eliminar funciones predeterminadas que no sean relevantes para su organización.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 664fb2fe-ff7e-4807-9a43-b37e7d5d57eb
source-git-commit: cada5387ddfb710029d06cd38841ecb9c8a6484b
workflow-type: tm+mt
source-wordcount: '1703'
ht-degree: 32%

---

# Crear y administrar funciones de trabajo

<!-- Audited: 1/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

{{highlighted-preview}}

>[!IMPORTANT]
>
>Con la versión 25.11, la moneda de anulación para los roles estaba en desuso en Producción. (La obsolescencia tuvo lugar el 30 de octubre en el entorno de vista previa). En lugar de tener una divisa base y divisas de sustitución, ahora hay una divisa disponible para los roles de trabajo y las tarifas de coste y facturación se definen en esa divisa.

Como administrador de [!DNL Adobe Workfront] o usuario con acceso administrativo a los roles, puede crear roles que se puedan asignar a los usuarios y eliminar los roles predeterminados que no sean relevantes para su organización. Para obtener información acerca del acceso administrativo en [!DNL Workfront], consulte [Conceder acceso administrativo a los usuarios a ciertas áreas](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

>[!TIP]
>
>Las funciones son parte integral de la administración de recursos. Para utilizar las herramientas de planificación de recursos, las funciones necesitan tener asociados un coste y una tasa de facturación. Para obtener más información, consulte [Introducción a la administración de recursos](../../../resource-mgmt/resource-mgmt-overview/get-started-resource-management.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Para crear o editar un rol: Cualquier paquete de flujo de trabajo o Workfront</p>
   <p>Para aplicar atributos de tasa y agregar formularios personalizados a la función: Flujo de trabajo Ultimate</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>[!UICONTROL Standard]</p>
       <p>[!UICONTROL Plan]</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>Acceso administrativo a los roles</td>
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de una función

Para crear una función:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Roles]**.
1. Haga clic en **[!UICONTROL Nuevo rol] <span class="preview">> Crear nuevo rol**.</span>
1. Introduzca información en los campos siguientes:

   * **Nombre**: indique un nombre para el rol. Este es el nombre que se muestra en todas las partes de Workfront donde aparece el campo Rol.

     >[!TIP]
     >
     >El nombre de un rol puede contener hasta 255 caracteres. Sin embargo, los nombres más largos pueden truncarse en determinadas áreas de Workfront.

   * **Descripción**: escriba una descripción para el rol que indique lo que tiene de único.
   * **Está activo**: seleccione **Sí** si desea que el rol esté activo y disponible en cualquier lugar de Workfront para asociarlo a usuarios, elementos de trabajo, etc. Seleccione **No** si desea que el rol se desactive y no esté disponible para asignarlo a usuarios, elementos de trabajo, etc.

     Para obtener información sobre cómo desactivar roles, consulte [Desactivación de funciones](/help/quicksilver/administration-and-setup/set-up-workfront/organizational-setup/deactivate-job-roles.md).

   * **Moneda**: La moneda base se muestra de manera predeterminada. El administrador de Workfront añade la Moneda base en el área de Configuración. Puede cambiar la selección a otra divisa disponible y cambiar la divisa en intervalos de fechas en vigor.

     >[!TIP]
     >
     >En este campo sólo están disponibles las divisas disponibles en el área Tasas de cambio del sistema. Si solo tiene configurada una moneda, solo estará disponible esa moneda.

     Para obtener información sobre cómo configurar la divisa base en Workfront, consulte [Configurar tasas de cambio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

     Para obtener información acerca de cómo cambiar la moneda de un proyecto, vea [Cambiar la moneda del proyecto](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

   * **Tasa de costo**: Es la tasa de costo por hora del rol. Este valor calcula los costes planificados y reales de las tareas y problemas asociados con la función y, en última instancia, los costes planificados y reales de los proyectos. Introduzca el tipo de cambio utilizando la divisa seleccionada.

     Para ver las tarifas de coste efectivas por fecha, haga clic en **Añadir tarifa**. Introduzca el valor del coste/hora para el período de tiempo y asigne una fecha de inicio y una fecha de finalización según sea necesario. La primera tarifa de coste no tendrá una fecha de inicio y la última tarifa de coste no tendrá una fecha de finalización.

     Algunas fechas se añaden automáticamente. Por ejemplo, si la primera tarifa de coste no tiene una fecha de finalización y añade una segunda tarifa de coste con una fecha de inicio del viernes, 01 de mayo de 2025, se añade una fecha de finalización del jueves, 30 de abril de 2025 a la primera tarifa de coste para que no haya huecos.

     Para obtener información acerca de cómo Workfront calcula los costos, vea [Rastrear costos](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >Al editar un rol existente, puede ordenar la lista para ver la fecha de inicio más reciente en la parte superior de la lista de tarifas.

   * **Tarifa de facturación**: Es la tarifa de facturación por hora del rol. Este valor calcula los ingresos planificados y reales de las tareas y los problemas asociados a la función, y, en última instancia, los ingresos planificados y reales de los proyectos. Introduzca el tipo de cambio utilizando la divisa seleccionada.

     Para ver las tarifas de facturación vigentes por fecha, haga clic en **Añadir tarifa**. Introduzca el valor de la facturación/hora para el período de tiempo y asigne una Fecha de inicio y una Fecha de finalización según sea necesario. La primera tarifa de facturación no tendrá fecha de inicio y la última tarifa de facturación no tendrá fecha de finalización.

     Algunas fechas se añaden automáticamente. Por ejemplo, si la primera tarifa de facturación no tiene una fecha de finalización y añade una segunda con una fecha de inicio del viernes, 01 de mayo de 2025, se añade una fecha de finalización del jueves, 30 de abril de 2025 a la primera tarifa de facturación para que no existan huecos.

     Para obtener información sobre cómo Workfront calcula los ingresos, consulte [Información general sobre facturación e ingresos](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >Al editar un rol existente, puede ordenar la lista para ver la fecha de inicio más reciente en la parte superior de la lista de tarifas.

<!-- Remove or hide the billing rate and cost rate bullets on April 16 for GA -->

1. Haga clic en **[!UICONTROL Crear función]**. La función ya está disponible para asignarse a tareas, problemas, aprobaciones o puede compartir plantillas de diseño u otros objetos con ella. Para obtener información acerca de todos los usos de las funciones en [!DNL Workfront], consulte [Información general de la función](../../../administration-and-setup/set-up-workfront/organizational-setup/job-role-overview.md). Para obtener información acerca de cómo eliminar una función, consulte [Eliminar funciones](../../../administration-and-setup/set-up-workfront/organizational-setup/delete-job-roles.md).

<div class="preview">

## Adición de tasas y atributos a un rol

Las tasas de facturación y de costo de un rol se utilizan en los cálculos financieros.

Los atributos de tarifa son compatibles con las áreas de Workfront donde existen tarifas, como roles de trabajo y usuarios. Cuando los atributos se aplican a un rol, sus asignaciones se resuelven automáticamente en las tasas correctas.

Para obtener más información, vea [Definir atributos de tasa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **[!UICONTROL Roles]**.
1. Haga clic en el nombre de un rol existente para editarlo.
1. Para actualizar los detalles del rol, haga clic en **Detalles** en el panel izquierdo.
1. (Opcional) Para adjuntar un formulario personalizado al rol, haga clic en el campo **Agregar formulario personalizado** en la esquina superior derecha de la página Detalles y seleccione un formulario personalizado de la lista que se muestra.

   Para obtener más información sobre cómo adjuntar un formulario personalizado, vea [Añadir un formulario personalizado a un objeto](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

1. Haga clic en [!UICONTROL **Tasas**] en el panel izquierdo.
1. Haga clic en [!UICONTROL **Facturación**] o en [!UICONTROL **Costo**] para seleccionar el tipo de tarifa.
1. Haga clic en [!UICONTROL **Agregar tarifas**] para agregar una nueva tarifa.

   O

   Seleccione una tarifa existente y haga clic en el icono **Editar** ![Editar icono](assets/edit-icon.png) para actualizarlo.

   >[!NOTE]
   >
   >Debido a que cada tasa está asociada a la combinación de la función y los atributos para crear una tasa única, los atributos no se pueden cambiar al editar una tasa.

1. En el cuadro **Nueva tarifa**, seleccione atributos para la tarifa como Agencia, Ubicación o Centro de costo.

   >[!NOTE]
   >
   >Estos atributos se definen por separado y pueden afectar a los cálculos de ingresos y costes. Para obtener más información, vea [Definir atributos de tasa](/help/quicksilver/administration-and-setup/manage-enterprise-operations/define-rate-attributes.md).

1. Seleccione **Divisa** para la tarifa. El administrador de Workfront añade la Moneda base en el área de Configuración. Puede cambiar la selección a otra divisa disponible y cambiar la divisa en intervalos de fechas en vigor.

   >[!TIP]
   >
   >En este campo sólo están disponibles las divisas disponibles en el área Tasas de cambio del sistema. Si solo tiene configurada una moneda, solo estará disponible esa moneda.

   Para obtener información sobre cómo configurar la divisa base en Workfront, consulte [Configurar tasas de cambio](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md).

   Para obtener información acerca de cómo cambiar la moneda de un proyecto, vea [Cambiar la moneda del proyecto](/help/quicksilver/manage-work/projects/project-finances/change-project-currency.md).

1. (Condicional) Para una tarifa de facturación, ingrese **Tarifa de facturación** para este rol.

   Esta es la tarifa de facturación por hora de la función. Este valor calcula los ingresos planificados y reales de las tareas y los problemas asociados a la función, y, en última instancia, los ingresos planificados y reales de los proyectos. Introduzca el tipo de cambio utilizando la divisa seleccionada.

   Si utiliza atributos, los atributos y la función se combinan para definir una tasa única. Por ejemplo, una función de Designer en Nueva York para la Agencia A puede tener una tasa separada de una función de Designer en París para la Agencia B.

   Para ver las tarifas de facturación vigentes por fecha, haga clic en **Añadir tarifa**. Introduzca el valor de la facturación/hora para el período de tiempo y asigne una Fecha de inicio y una Fecha de finalización según sea necesario. La primera tarifa de facturación no tendrá fecha de inicio y la última tarifa de facturación no tendrá fecha de finalización.

   Algunas fechas se añaden automáticamente. Por ejemplo, si la primera tarifa de facturación no tiene una fecha de finalización y agrega una segunda con una fecha de inicio del 1 de mayo, se agrega una fecha de finalización del 30 de abril a la primera tarifa de facturación de modo que no existan brechas.

   Para obtener información sobre cómo Workfront calcula los ingresos, consulte [Información general sobre facturación e ingresos](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

   >[!TIP]
   >
   >Al editar un rol existente, puede ordenar la lista para ver la fecha de inicio más reciente en la parte superior de la lista de tarifas.

1. (Condicional) Para una tasa de costo, escriba la **tasa de costo** para este rol.

   Esta es la tarifa de coste por hora de la función. Este valor calcula los costes planificados y reales de las tareas y problemas asociados con la función y, en última instancia, los costes planificados y reales de los proyectos. Introduzca el tipo de cambio utilizando la divisa seleccionada.

   Si utiliza atributos, los atributos y la función se combinan para definir una tasa única. Por ejemplo, una función de Designer en Nueva York para la Agencia A puede tener una tasa separada de una función de Designer en París para la Agencia B.

   Para ver las tarifas de coste efectivas por fecha, haga clic en **Añadir tarifa**. Introduzca el valor del coste/hora para el período de tiempo y asigne una fecha de inicio y una fecha de finalización según sea necesario. La primera tarifa de coste no tendrá una fecha de inicio y la última tarifa de coste no tendrá una fecha de finalización.

   Algunas fechas se añaden automáticamente. Por ejemplo, si la primera tasa de coste no tiene una fecha de finalización y agrega una segunda tasa de coste con una fecha de inicio del 1 de mayo, se agrega una fecha de finalización del 30 de abril a la primera tasa de coste para que no haya espacios.

   Para obtener información acerca de cómo Workfront calcula los costos, vea [Rastrear costos](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

   >[!TIP]
   >
   >Al editar un rol existente, puede ordenar la lista para ver la fecha de inicio más reciente en la parte superior de la lista de tarifas.

1. Haga clic en [!UICONTROL **Guardar**].

</div>

<!--
   * **Override Currency Cost Rate**: This is the cost per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual costs of tasks and issues associated with the job role.

     Enter the rate in the Override Currency specified above. This also updates the Cost Rate for this job role when using the Base Currency.

     For information about how Workfront calculates cost, see [Track costs](/help/quicksilver/manage-work/projects/project-finances/track-costs.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a cost rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Cost Rate, the cost rate of the job role also updates automatically.

   * **Override Currency Billing Rate**: This is the billing per hour rate of the job role using the selected Override Currency. Workfront uses this value to calculate the planned and the actual revenue of tasks and issues associated with the job role.

      Enter the rate in the Override Currency specified above. This also updates the Billing Rate for this job role when using the Base Currency.

      For information about how Workfront calculates revenue, see [Overview of Billing and Revenue](/help/quicksilver/manage-work/projects/project-finances/billing-and-revenue-overview.md).

     >[!TIP]
     >
     >When updating an existing job role that already has a billing rate associated with it, Workfront calculates the Override Currency rate based on the conversion rate in your system. If you update the Override Currency Billing Rate, the billing rate of the job role also updates automatically.

-->



