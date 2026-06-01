---
title: Información general sobre espacios de trabajo
description: Un espacio de trabajo es un conjunto de tipos de registros que utiliza un equipo y que representa el ciclo de vida del trabajo del equipo. Puede personalizar por completo los espacios de trabajo en Adobe Workfront Planning para que coincidan con los flujos de trabajo de las unidades organizativas.
feature: Workfront Planning
role: User, Admin
author: Alina
recommendations: noDisplay, noCatalog
exl-id: b80d5ccf-4d22-49f2-89b6-bb9678a353c2
source-git-commit: 4692dc6f7ab840bb43f3788126471425e9f8a396
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 90%

---

# Información general sobre espacios de trabajo

<!--
<span class="preview">The information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>
-->

{{planning-important-intro}}

Un espacio de trabajo es un conjunto de tipos de registros que utiliza una unidad organizativa y representa el ciclo de vida y los procesos de trabajo de la unidad. Puede personalizar por completo los espacios de trabajo en Adobe Workfront Planning.

<!--update screenshot with preview-->

![Cuenta de administrador de página de aterrizaje de espacios de trabajo](assets/workspaces-landing-page-admin-account.png)

## Consideraciones sobre espacios de trabajo

* Puede crear espacios de trabajo para unidades organizativas específicas dentro de su organización, de modo que coincidan con el modo único en que funciona cada unidad.
* Workfront Planning no incluye espacios de trabajo preconfigurados. Debe crearlos de acuerdo con las necesidades de su organización.
* Puede crear espacios de trabajo de las siguientes maneras:

   * Desde cero
   * Mediante una plantilla. Las plantillas contienen un número preconfigurado de tipos de registro y sus campos.
   * Uso de Planning Designer con tecnología de IA. Esta función se encuentra actualmente en Beta.
   * Uso de un paquete de plantillas de varios espacios de trabajo.

  Para obtener más información, consulte [Creación de espacios de trabajo](/help/quicksilver/planning/architecture/create-workspaces.md).

* Los espacios de trabajo son marcos en los que trabajan las unidades organizativas (un equipo, un grupo, un departamento o una división). No se pueden asociar a campos. Solo los tipos de registro dentro de un espacio de trabajo pueden asociarse con campos.

  Para obtener más información, vea [Información general sobre los tipos de registro](/help/quicksilver/planning/architecture/overview-of-record-types.md).
* Según la licencia de Workfront, los espacios de trabajo se muestran en las siguientes pestañas del área de planificación:

   * Para los administradores del sistema, los espacios de trabajo se muestran en las siguientes pestañas:

      * **Espacios de trabajo en los que trabajo**: muestra los espacios de trabajo que ha creado o los que se han compartido con usted.
      * **Otros espacios de trabajo**: muestra todos los demás espacios de trabajo del sistema.

     <!--
      * <span class="preview">**Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.</span> (************TEST THIS WITH SYSTEM ADMINS AND STANDARD USERS**********)
      -->

   * Para el resto de los usuarios, los espacios de trabajo que han creado otros y los que otros han compartido con ellos se muestran en el área Espacios de trabajo.

  <!--

    ******************* If Standard users can see the Sample workspaces, then replace the last bullet with this: 

   * For all other users:

        * (****************what is the name of this tab????*******) Workspaces they created and workspaces others shared with them display in the Workspaces area. 
        * <span class="preview">**Sample workspaces**: Displays built-in examples of best-practice workspaces. You cannot edit the workspaces, record types, or add records, but you can add, edit, and share views with others.</span>
    
    -->

  <!--      
    >[!NOTE]
    >
    ><span class="preview">We recommend to not edit the sample workspaces, but instead to use them as a reference to create your own. Use the multi-workspace template bundle to create workspaces identical to the ones listed in the Sample workspaces tab. For information, see the section "Create multiple workspaces using a best-practice multi-workspace template bundle" in the article [Create workspaces](/help/quicksilver/planning/architecture/create-workspaces.md). </span> 
    -->

* Los tipos de registro que contiene un espacio de trabajo deben reflejar el ciclo de vida laboral y los conceptos de una unidad organizativa.

  Por ejemplo, si los objetos de trabajo de una unidad son campañas, productos y regiones, el espacio de trabajo de esa unidad debe contener los tipos de registro de Campaña, Producto y Región.
* Cuando crea un espacio de trabajo, solo usted tiene permiso para acceder a él y administrarlo. Debe compartirlo con otros usuarios para que puedan colaborar con usted en el mismo espacio.

  Para obtener más información, vea [Uso compartido de un espacio de trabajo](/help/quicksilver/planning/access/share-workspaces.md).

  Los administradores del sistema pueden gestionar todos los espacios de trabajo, incluso los que no hayan creado.

<!--make this live with the GA: * There is no limit for how many workspaces you can create in your environment. However, we recommend not to have too many workspaces, as they could become hard to manage and your workflows might be too fragmented.-->

* Existen límites en cuanto a la cantidad de objetos de espacio de trabajo que se pueden crear en la instancia de Workfront Planning. Para obtener más información, consulte [Información general sobre limitaciones de objetos de Adobe Workfront Planning](/help/quicksilver/planning/general/limitations-overview.md).
