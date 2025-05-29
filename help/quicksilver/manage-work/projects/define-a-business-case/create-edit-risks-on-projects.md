---
product-area: projects
navigation-topic: business-case-and-scorecards
title: Crear y editar riesgos en proyectos
description: Los riesgos son eventos posibles o factores que impiden que un proyecto finalice a tiempo o dentro del presupuesto. Puede registrar los riesgos del proyecto como parte de la creación del caso empresarial de un proyecto o utilizando la pestaña Riesgos. Puede agregar riesgos a proyectos y plantillas. No es posible asociar riesgos con tareas o problemas.
author: Alina
feature: Work Management
exl-id: 6125c477-c0d8-43b4-88d8-35b0c2412468
source-git-commit: 78b4724ca8d5df15ed76e9e882179e3cb127282c
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 64%

---

# Crear y editar riesgos en proyectos

<!--Audited: 01/2025-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers after a week from the Preview release. </span>   

<span class="preview">For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md). </span>-->

Los riesgos son eventos posibles o factores que impiden que un proyecto finalice a tiempo o dentro del presupuesto. Puede registrar los riesgos como parte de la creación del caso empresarial de un proyecto o utilizando la pestaña Riesgos.

Solo puede crear riesgos en proyectos o plantillas. No es posible asociar riesgos con tareas o problemas.

Los riesgos pueden estar asociados con el coste, pero el coste de riesgos real no afecta al coste real del proyecto.

>[!NOTE]
>
>Este artículo define los riesgos asociados con el proyecto tal como los define en el caso comercial del proyecto o como los agrega en la pestaña Riesgos del proyecto.
>
>Para obtener información sobre el campo Riesgo que está disponible al editar un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Plan de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Nuevo: estándar </p>
   <p>Actual: plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Editar acceso a Proyectos y datos financieros</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p> Permisos de administración que incluyen Administrar finanzas en el proyecto para el que desea crear o editar riesgos </p> </td> 
  </tr> 
 </tbody> 
</table>

*Para obtener información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear y editar riesgos en el caso empresarial

Puede crear riesgos como parte de la planificación del caso empresarial de un proyecto. Posteriormente, puede editarlos en el caso empresarial, cuando se produzcan cambios en su probabilidad, plan de mitigación o coste, por ejemplo. Para obtener información sobre cómo crear un caso empresarial, consulte [Crear un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

El administrador de Workfront o el administrador de grupos debe habilitar la sección **Riesgos** en su caso empresarial en el área Preferencias del proyecto para poder verla en el nivel de proyecto en la sección Caso empresarial. Para obtener información sobre cómo establecer las preferencias del proyecto, consulte [Configurar las preferencias de proyecto en todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

En el caso empresarial, el proceso de creación y de edición de riesgos es idéntico.

Para crear o editar un riesgo en el caso empresarial:

1. Vaya al proyecto para el que desea crear riesgos.
1. Haga clic en **Caso empresarial** en el panel de la izquierda.
1. En la sección **Riesgos**, haga clic en **Editar riesgos**.
1. Introduzca o edite la siguiente información:

   * **Descripción:** describa el riesgo.

   * **Coste potencial**: indique el coste estimado en caso de producirse el riesgo.

   * **Probabilidad**: indique la probabilidad de que el riesgo se manifieste como un valor porcentual.

   * **Tipo**: indique a qué categoría pertenece el riesgo.
   * **Plan de mitigación**: actualice la descripción del plan para mitigar el riesgo.

   * **Coste de mitigación**: indique el coste del plan de mitigación que se debe establecer para evitar que se produzca el riesgo.

   ![Riesgos](assets/crp1-350x117.png)

1. (Opcional) Haga clic en **Añadir otro riesgo** para añadir riesgos adicionales.
1. Haga clic en **Guardar**.

## Crear y editar riesgos en el área Riesgos

Además de crear y editar riesgos en el caso empresarial, puede hacerlo en la sección **Riesgos** de un proyecto.

Puede crear y editar riesgos en la sección Riesgos de un proyecto o una plantilla. Crear riesgos para plantillas es idéntico a crear riesgos para proyectos.

### Creación de riesgos en el área Riesgos {#create-risks-in-the-risks-area}

1. Vaya al proyecto para el que quiera crear riesgos.
1. Haga clic en **Riesgos** en el panel izquierdo.

   ![Sección Riesgos de la tarea](assets/risks-section-on-project-2022.png)

1. Haga clic en **Comenzar a agregar riesgos** y cree riesgos editando en línea su información. **Descripción** es un campo obligatorio

   O

   Haga clic en **Nuevo riesgo**.

   Se abre el cuadro **Nuevo riesgo**.

   ![Nuevo cuadro de riesgo](assets/new-risk-box.png)

1. (Condicional) Si agrega un riesgo en el cuadro **Nuevo riesgo**, escriba la siguiente información:

   * **Descripción**: describe el riesgo. Este campo es obligatorio.
   * **Tipo de riesgo**: Indique en qué categoría se encuentra el riesgo.\
     El administrador de Workfront define los tipos de riesgos disponibles en el entorno. Para obtener información acerca de la definición de tipos de riesgos, consulte el artículo [Editar y crear tipos de riesgos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

   * **Probabilidad**: indique la probabilidad de que el riesgo se presente como un valor porcentual.
   * **Costo potencial**: Indique el costo estimado si el riesgo se presenta.
   * **Costo de mitigación**: indique el costo del plan de mitigación que debe establecer para evitar que se produzca el riesgo.
   * **Costo real**: indique el costo real del riesgo si éste se produjo.
   * **Plan de mitigación**: actualice la descripción del plan para mitigar el riesgo.

1. (Condicional) Haga clic en **Introducir** si está creando el riesgo en línea.

   O

   Haga clic en **Guardar** si está editando la información en el cuadro **Nuevo riesgo**.

1. (Opcional) Seleccione un **Estado** diferente para el riesgo en el menú desplegable **Estado** al aplicar la vista **Estándar** para la lista de riesgos.

   De manera predeterminada, el **estado** de un riesgo es **Identificado**.

### Edición de riesgos en el área Riesgos {#edit-risks-in-the-risks-area}

Es posible editar los riesgos durante la duración de un proyecto. Por ejemplo: al producirse cambios en la probabilidad, coste potencial o estado.

Edite los riesgos de uno en uno o varios de forma masiva.

Para editar riesgos:

1. Desplácese hasta un proyecto para el que quiera editar los riesgos existentes.
1. Haga clic en **Riesgos** en el panel izquierdo.
1. Comience a editar en línea los campos de los riesgos que vea en la lista para editar los riesgos de uno en uno.

   O

   Seleccione uno o varios riesgos y, a continuación, haga clic en **Editar** para editar varios riesgos al mismo tiempo.

   >[!NOTE]
   >
   >Se aplica la misma información a todos los riesgos seleccionados al editar varios riesgos al mismo tiempo. La información asociada con cada riesgo antes de los cambios se sobrescribe en una edición masiva.

1. Si ha hecho clic en **Editar**, se abrirá el cuadro **Editar riesgo** o **Editar riesgos**.

   Considere la posibilidad de editar los campos siguientes:

   * **Descripción**: edite la descripción del riesgo.
   * **Tipo de riesgo**: indique en qué categoría se encuentra el riesgo.
   * **Probabilidad**: indique la probabilidad de que el riesgo se presente como un valor porcentual.
   * **Costo potencial**: Indique el costo estimado si el riesgo se presenta.
   * **Costo de mitigación**: indique el costo del plan de mitigación que debe establecer para evitar que se produzca el riesgo.
   * **Costo real**: indique el costo real del riesgo si éste se produjo.
   * **Plan de mitigación**: actualice la descripción del plan para mitigar el riesgo.

1. Haga clic en **Guardar**.
1. (Opcional) Edite el **Estado** de un riesgo en el menú desplegable **Estado** al aplicar la vista **Estándar** para la lista de riesgos.

   >[!NOTE]
   >
   >No puede editar el **estado** de los riesgos en el cuadro de diálogo **Editar riesgo**. Solo es posible hacerlo en una edición en línea.
