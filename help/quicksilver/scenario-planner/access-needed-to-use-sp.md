---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Acceso necesario para utilizar el planificador de escenarios
description: Scenario Planner requiere una licencia independiente de Adobe Workfront y acceso adicional.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 7b61f6d9380365daa614c597ee7755d6d01d915d
workflow-type: tm+mt
source-wordcount: '818'
ht-degree: 0%

---

# Acceso necesario para usar la variable [!DNL Scenario Planner]

La variable [!DNL Scenario Planner] requiere una licencia adicional. Para obtener información sobre la variable [!DNL Workfront Scenario Planner], consulte [La variable [!DNL Scenario Planner] información general](../scenario-planner/scenario-planner-overview.md).

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Sin acceso o permisos correctos, es posible que no pueda ver la variable [!UICONTROL Situaciones] área de[!DNL  Adobe Workfront] ni administrar planes o iniciativas para su organización. La administración de planes e iniciativas incluye su creación, edición y eliminación.

>[!IMPORTANT]
>
>Al acceder [!UICONTROL Situaciones], solo puede ver y administrar los planes que ha creado. Si desea permitir que otros usuarios vean o gestionen los planes que ha creado, debe hacer lo siguiente:
>
>* Enviar un vínculo a su plan a otros usuarios
>* Compartir el plan con otros usuarios
>
>  Para obtener información sobre cómo compartir un plan, consulte [Compartir un plan en [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).
>
>Cuando se desactiva un usuario, sus planes no tienen propietario y no se puede acceder a ellos a menos que se compartan previamente con un vínculo.

## Acceso necesario para ver y usar la variable [!DNL Adobe Workfront Scenario Planner]

Debe asegurarse de que se cumplan todas las condiciones siguientes antes de poder acceder a la variable [!DNL Workfront Scenario Planner]:

<!--drafted for P&P:

* Depending on whether you use the current or the legacy Workfront plans, your organization must have the following:

  * For the current plans:  

    * The [!UICONTROL Ultimate] [!DNL Workfront] plan.

      Or
  
    * The [!UICONTROL Select] or [!UICONTROL Prime] [!DNL Workfront] plan, in addition to purchasing a separate [!DNL Scenario Planner] license.

  * For the legacy plans: (indent the bullets below, before the NOTE)

-->

* Su organización debe adquirir un [!DNL Workfront] [!UICONTROL Empresa] o superior [!DNL Workfront] plan. Para obtener información sobre la variable [!DNL Workfront] planes, consulte [Planes de Workfront](http://workfront.com/plans).
* Su organización debe adquirir un [!DNL Workfront Scenario Planner] licencia, además de [!DNL Workfront] licencia. Póngase en contacto con su [!DNL Workfront] Representante de cuentas para obtener más información [!DNL Workfront Scenario Planner] licencias.

<!--drafted for P&P: 

* Depending on whether you use the current or legacy licenses, your [!DNL Workfront] administrator must assign you a license of any of the following types: 

  * For the current licenses: 
    * [!UICONTROL Standard]
    * [!UICONTROL Light]

  * For the legacy licenses: (re-indent the licenses below and reword the sentence)

-->



* Su [!DNL Workfront] el administrador debe asignarle una licencia de cualquiera de los siguientes [!DNL Workfront] tipos:

   * [!UICONTROL Plan]
   * [!UICONTROL Trabajo]
   * [!UICONTROL Revisar]

   >[!NOTE]
   >
   >Usuarios con un [!UICONTROL Solicitud] o [!UICONTROL Externo] el tipo de licencia no puede acceder a [!DNL Workfront Scenario Planner].

<!--drafted - replace the note above with this at P&P release: 
  * When using the current licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
  * When using the legacy licenses, users with a Request or External license type cannot access the Scenario Planner. -->

* Su [!DNL Workfront] el administrador debe [!UICONTROL Ver] o [!UICONTROL Editar] acceso a [!DNL Scenario Planner] en su nivel de acceso.

   Para obtener información sobre cómo conceder acceso a la variable [!DNL Workfront Scenario Planner], consulte [Conceder acceso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* (Opcional y recomendada) Para ver o actualizar la información financiera de sus planes e iniciativas, su [!DNL Workfront] El administrador también debe conceder acceso a [!UICONTROL Datos financieros] en su nivel de acceso. Para obtener información sobre la concesión de datos financieros en el nivel de acceso, consulte [Concesión de acceso a datos financieros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

   <!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

* Si necesita acceder a planes que no ha creado, un creador del plan debe darle los permisos correctos para su plan para acceder a ellos. Para obtener información sobre los permisos necesarios para acceder a planes e iniciativas que no ha creado, consulte la [Permisos necesarios para acceder a planes e iniciativas](#permissions-needed-to-access-plans-and-initiatives) en este artículo.

## Acceso necesario para ver planes e iniciativas

Además de que su empresa adquiera la licencia correcta para el [!DNL Workfront Scenario Planner], su [!DNL Workfront] el administrador también debe asignarle los siguientes accesos y configuraciones para que pueda ver la [!DNL Workfront Scenario Planner] y la información en este ámbito:

* Un nivel de acceso con al menos [!UICONTROL Ver] acceso a [!DNL Scenario Planner].

   Para obtener información sobre el nivel de acceso a [!DNL Scenario Planner], consulte [Conceder acceso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* Un nivel de acceso con al menos [!UICONTROL Ver] acceso a [!UICONTROL Datos financieros] si necesita ver también información financiera sobre el plan y las iniciativas. Algunos ejemplos de información financiera son presupuestos, costos o tasas de puestos de trabajo.

   Para obtener información sobre la variable [!UICONTROL Datos financieros] nivel de acceso, consulte [Concesión de acceso a datos financieros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

   >[!TIP]
   >
   >[!UICONTROL Solicitantes] y [!UICONTROL Externo] Los usuarios no tienen acceso a la vista del [!DNL Scenario Planner].

* Ver permisos para el plan. Para obtener información sobre los permisos necesarios para acceder a planes e iniciativas que no ha creado, consulte la [Permisos necesarios para acceder a planes e iniciativas](#permissions-needed-to-access-plans-and-initiatives) en este artículo.

## Acceso necesario para administrar planes e iniciativas

Su [!DNL Workfront] el administrador debe asignarle el siguiente acceso para que pueda administrar los planes y su información en la [!DNL Scenario Planner]:

* A [!UICONTROL Plan] o [!UICONTROL Trabajo] tipo de licencia con acceso de edición al [!DNL Scenario Planner] en su nivel de acceso.

   Todos los demás tipos de licencia no tienen acceso para administrar planes.

   Para obtener información sobre cómo conceder acceso a [!DNL Scenario Planner] Desde el nivel de acceso, consulte [Conceder acceso a [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Plan] tipo de licencia con [!UICONTROL Editar] acceso a [!UICONTROL Datos financieros] en el nivel de acceso, si también necesita actualizar información financiera sobre el plan.

   Algunos ejemplos de información financiera que puede editar son [!UICONTROL Presupuesto], [!UICONTROL Beneficio planificado]y [!UICONTROL Costes fijos].

   >[!TIP]
   >
   >Solo [!UICONTROL Plan] los titulares de licencias tienen [!UICONTROL Editar] acceso a [!UICONTROL Datos financieros].

   Para obtener información sobre la variable [!UICONTROL Datos financieros] nivel de acceso, consulte [Concesión de acceso a datos financieros](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Administre permisos para un plan que no haya creado. Para obtener información sobre los permisos necesarios para acceder a planes e iniciativas que no ha creado, consulte la [Permisos necesarios para acceder a planes e iniciativas](#permissions-needed-to-access-plans-and-initiatives) en este artículo.

## Permisos necesarios para acceder a planes e iniciativas

Los niveles de acceso funcionan junto con los permisos en [!DNL Workfront] para darle visibilidad a los planes e iniciativas que no ha creado. Además de tener el nivel de acceso correcto para acceder a la variable [!DNL Scenario Planner], también debe tener los permisos correctos para el plan que desea ver o administrar, si no es el creador de esos planes.

De forma predeterminada, solo tiene acceso a los planes que ha creado. Para ver los planes que otros usuarios han creado, deben compartir sus planes con usted. Para obtener información sobre cómo compartir planes, consulte [Compartir un plan en [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

Si un usuario comparte un vínculo a un plan sin compartir también el plan, puede solicitar permisos para el plan. Para obtener información sobre la solicitud de permisos para planes, consulte [Solicitar acceso a un plan en la [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

