---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Acceso necesario para utilizar el Scenario Planner
description: El planificador de escenarios requiere una licencia independiente de Adobe Workfront y acceso adicional.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: f0f6c2bee98c6cebf8ea9e18bf34262f3c1d6e3a
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 0%

---

# Se necesita acceso para usar [!DNL Scenario Planner]

[!DNL Scenario Planner] requiere una licencia adicional. Para obtener información acerca de [!DNL Workfront Scenario Planner], vea [La [!DNL Scenario Planner] descripción general](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Sin el acceso o los permisos correctos, es posible que no pueda ver el área de [!UICONTROL Escenarios] de[!DNL  Adobe Workfront] ni administrar planes o iniciativas para su organización. La administración de planes e iniciativas incluye su creación, edición y eliminación.

>[!IMPORTANT]
>
>Al acceder a [!UICONTROL Escenarios], solo puede ver y administrar los planes que ha creado. Si desea permitir que otros usuarios vean o administren los planes que ha creado, debe hacer lo siguiente:
>
>* Envíe un vínculo a su plan a otros usuarios
>* Compartir el plan con otros usuarios
>
>  Para obtener información acerca de cómo compartir un plan, vea [Compartir un plan en [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>Cuando se desactiva un usuario, sus planes no tienen propietario y no se puede acceder a él a menos que se comparta previamente con un vínculo.

## Acceso necesario para ver y utilizar [!DNL Adobe Workfront Scenario Planner]

Debe asegurarse de que se cumplen todas las condiciones siguientes para poder tener acceso a [!DNL Workfront Scenario Planner]:

1. Su organización debe tener uno de los planes de Workfront que se describen a continuación.

   Dependiendo de si utiliza el plan de Workfront nuevo o el actual, su organización debe tener uno de los siguientes:

   * Para los nuevos planes, su organización debe tener uno de los siguientes:

      * El plan [!UICONTROL Ultimate] [!DNL Workfront]. El Scenario Planner está incluido en el plan Ultimate.

        O

      * El plan [!UICONTROL Select] o [!UICONTROL Prime] [!DNL Workfront], además de comprar una licencia de [!DNL Scenario Planner] por separado.

   * Para los planes actuales de Workfront, su organización debe tener los dos elementos siguientes:

      * Su organización debe adquirir un plan [!DNL Workfront] [!UICONTROL Empresa] o superior [!DNL Workfront]. Para obtener información sobre los planes [!DNL Workfront], consulte [Planes de Workfront](https://workfront.com/plans).

      * Su organización debe adquirir una licencia de [!DNL Workfront Scenario Planner], además de una licencia de [!DNL Workfront]. Póngase en contacto con su representante de cuentas de [!DNL Workfront] para obtener más información sobre las licencias de [!DNL Workfront Scenario Planner].

1. Debe tener una de las licencias de Workfront que se describen a continuación.

   Dependiendo de si usa las licencias nuevas o las actuales, el administrador de [!DNL Workfront] debe asignarle una licencia de cualquiera de los siguientes tipos:

   * Para las nuevas licencias:
      * [!UICONTROL Estándar]
      * [!UICONTROL Claro]

   * Para las licencias actuales:

      * [!UICONTROL Plan]
      * [!UICONTROL Trabajo]
      * [!UICONTROL Revisar]

   >[!NOTE]
   > 
   >* Al usar las licencias nuevas, los usuarios con un tipo de licencia [!UICONTROL Contributor] o [!UICONTROL External] no pueden obtener acceso a [!DNL Scenario Planner].
   >
   >* Al utilizar las licencias actuales, los usuarios con un tipo de licencia de Solicitud o Externa no pueden acceder al Scenario Planner.

1. El administrador de [!DNL Workfront] debe darle acceso de [!UICONTROL Ver] o [!UICONTROL Editar] a [!DNL Scenario Planner] en su nivel de acceso.

   Para obtener información acerca de cómo conceder acceso a [!DNL Workfront Scenario Planner], vea [Conceder acceso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Opcional y recomendada) Para ver o actualizar la información financiera de sus planes e iniciativas, el administrador de [!DNL Workfront] también debe otorgarle acceso a [!UICONTROL Datos financieros] en su nivel de acceso. Para obtener información sobre la concesión de datos financieros en su nivel de acceso, consulte [Conceder acceso a datos financieros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

1. (Opcional) Si necesita acceder a planes que no ha creado, un creador de planes debe darle los permisos correctos sobre su plan para acceder a ellos. Para obtener información sobre los permisos necesarios para acceder a planes e iniciativas que no has creado, consulta la sección [Permisos necesarios para acceder a planes e iniciativas](#permissions-needed-to-access-plans-and-initiatives) en este artículo.

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

## Acceso necesario para ver planes e iniciativas

Además de que su compañía adquiera la licencia correcta para [!DNL Workfront Scenario Planner], su administrador de [!DNL Workfront] debe asignarle también el siguiente acceso y configuración para que pueda ver [!DNL Workfront Scenario Planner] y la información de esta área:

* Un nivel de acceso con al menos [!UICONTROL Ver] acceso a [!DNL Scenario Planner].

  Para obtener información acerca del nivel de acceso a [!DNL Scenario Planner], vea [Conceder acceso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Un nivel de acceso con al menos [!UICONTROL Ver] acceso a [!UICONTROL Datos financieros] si también necesitas ver información financiera sobre el plan y las iniciativas. Algunos ejemplos de información financiera son los presupuestos, los costes o las tasas de función.

  Para obtener información sobre el nivel de acceso de [!UICONTROL Datos financieros], consulte [Conceder acceso a datos financieros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >Los usuarios de [!UICONTROL Requestors] y [!UICONTROL External] no tienen acceso para ver [!DNL Scenario Planner].

* Ver permisos del plan. Para obtener información sobre los permisos necesarios para acceder a planes e iniciativas que no has creado, consulta la sección [Permisos necesarios para acceder a planes e iniciativas](#permissions-needed-to-access-plans-and-initiatives) en este artículo.

## Acceso necesario para administrar planes e iniciativas

El administrador de [!DNL Workfront] debe asignarle el siguiente acceso para que pueda administrar planes y su información en [!DNL Scenario Planner]:

* Un tipo de licencia de [!UICONTROL Plan] o [!UICONTROL Trabajo] con acceso de edición para [!DNL Scenario Planner] en su nivel de acceso.

  Todos los demás tipos de licencia no tienen acceso para administrar planes.

  Para obtener información sobre la concesión de acceso a [!DNL Scenario Planner] desde el nivel de acceso, vea [Conceder acceso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Un tipo de licencia de [!UICONTROL Plan] con acceso de [!UICONTROL Editar] para [!UICONTROL datos financieros] en su nivel de acceso, si también necesita actualizar la información financiera sobre el plan.

  Algunos ejemplos de información financiera que puede editar son [!UICONTROL Presupuesto], [!UICONTROL Beneficio planificado] y [!UICONTROL Costos fijos].

  >[!TIP]
  >
  >Solo los titulares de la licencia de [!UICONTROL Plan] tienen acceso de [!UICONTROL Editar] a [!UICONTROL Datos financieros].

  Para obtener información sobre el nivel de acceso de [!UICONTROL Datos financieros], consulte [Conceder acceso a datos financieros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Administre permisos a un plan que no haya creado. Para obtener información sobre los permisos necesarios para acceder a planes e iniciativas que no has creado, consulta la sección [Permisos necesarios para acceder a planes e iniciativas](#permissions-needed-to-access-plans-and-initiatives) en este artículo.

## Permisos necesarios para acceder a planes e iniciativas

Los niveles de acceso trabajan junto con los permisos en [!DNL Workfront] para darle visibilidad a los planes e iniciativas que no ha creado. Además de tener el nivel de acceso correcto para acceder a [!DNL Scenario Planner], también debe tener los permisos correctos para el plan que desea ver o administrar, si no es el creador de esos planes.

De forma predeterminada, solo tiene acceso a los planes que ha creado. Para ver los planes que otros usuarios han creado, deben compartir sus planes con usted. Para obtener información acerca de cómo compartir planes, vea [Compartir un plan en [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

Si un usuario comparte un vínculo a un plan sin compartirlo también, puede solicitar permisos para el plan. Para obtener información sobre cómo solicitar permisos para planes, consulte [Solicitar acceso a un plan en [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

