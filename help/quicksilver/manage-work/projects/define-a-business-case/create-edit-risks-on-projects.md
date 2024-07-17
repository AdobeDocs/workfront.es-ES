---
product-area: projects
navigation-topic: business-case-and-scorecards
title: Crear y editar riesgos en proyectos
description: Los riesgos son posibles eventos o factores que impiden que un proyecto finalice a tiempo o dentro del presupuesto. Los riesgos se pueden registrar como parte del caso empresarial de un proyecto o mediante la pestaña Riesgos. Los riesgos solo se crean en un proyecto. No puede asociar riesgos con tareas o problemas.
author: Alina
feature: Work Management
exl-id: 6125c477-c0d8-43b4-88d8-35b0c2412468
source-git-commit: 8611c7bf8be6405f8ec8462ff2fd0f5998e8a995
workflow-type: tm+mt
source-wordcount: '1083'
ht-degree: 0%

---

# Crear y editar riesgos en proyectos

Los riesgos son posibles eventos o factores que impiden que un proyecto finalice a tiempo o dentro del presupuesto. Los riesgos se pueden registrar como parte del caso empresarial de un proyecto o mediante la pestaña Riesgos. Los riesgos solo se crean en un proyecto. No puede asociar riesgos con tareas o problemas.

Los riesgos pueden estar asociados con el costo, pero el costo de riesgo real no afecta al costo real del proyecto.

>[!NOTE]
>
>Este artículo define los riesgos asociados con el proyecto tal como los define en el caso comercial del proyecto o como los agrega en la pestaña Riesgos del proyecto. Para obtener información acerca del campo Riesgo que está disponible al editar un proyecto, vea [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos y datos financieros</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p> Administre permisos que incluyan Administrar finanzas en el proyecto para el que desea crear o editar riesgos </p> <p>Para obtener más información acerca de los permisos del proyecto, vea el artículo <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Compartir un proyecto en Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear y editar riesgos en el caso comercial

Puede crear riesgos como parte de la planificación del caso empresarial de un proyecto. Posteriormente, puede editarlos en el caso comercial, cuando se produzcan cambios en su probabilidad, plan de mitigación o coste, por ejemplo. Para obtener información sobre cómo crear un caso empresarial, vea [Crear un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

El administrador de Workfront o del grupo debe habilitar la sección **Riesgos** en su caso comercial en el área Preferencias del proyecto para poder verlo en el nivel de proyecto en la sección Caso comercial. Para obtener información sobre cómo establecer las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Crear y editar riesgos en el caso comercial es idéntico.

Para crear o editar un riesgo en el caso comercial:

1. Vaya al proyecto para el que desea crear riesgos.
1. Haga clic en **Caso comercial** en el panel izquierdo.
1. En la sección **Riesgos**, haga clic en **Editar riesgos**.
1. Introduzca o edite la siguiente información:

   * **Descripción:** describe el riesgo.

   * **Costo potencial**: indique el costo estimado si se debe producir el riesgo.

   * **Probabilidad**: indique la probabilidad de que el riesgo se presente como un valor porcentual.

   * **Tipo:** indica en qué categoría se encuentra el riesgo.
   * **Plan de mitigación**: actualice la descripción del plan para mitigar el riesgo.

   * **Costo de mitigación**: indique el costo del plan de mitigación que debe establecer para evitar que se produzca el riesgo.

   ![](assets/crp1-350x117.png)

1. (Opcional) Haga clic en **Agregar otro riesgo** para agregar riesgos adicionales.
1. Haga clic en **Guardar**.

## Crear y editar riesgos en el área Riesgos

Además de crear y editar riesgos en el caso comercial, puede hacerlo usando la sección **Riesgos** de un proyecto.

* [Crear riesgos en el área de riesgos](#create-risks-in-the-risks-area)
* [Editar riesgos en el área Riesgos](#edit-risks-in-the-risks-area)

### Crear riesgos en el área Riesgos {#create-risks-in-the-risks-area}

1. Vaya al proyecto para el que desea crear riesgos.
1. Haga clic en **Riesgos** en el panel izquierdo.

   ![Sección de riesgos de la tarea](assets/risks-section-on-project-2022.png)

1. Haga clic en **Comenzar a agregar riesgos** y cree riesgos editando en línea su información.

   O

   Haga clic en **Nuevo riesgo**. Se abre el cuadro de diálogo **Nuevo riesgo**.

1. Introduzca la siguiente información:

   * **Descripción**: describa el riesgo.
   * **Tipo de riesgo**: indique en qué categoría se encuentra el riesgo.\
     El administrador de Workfront define los tipos de riesgos disponibles en su entorno. Para obtener información acerca de la definición de tipos de riesgos, vea el artículo [Editar y crear tipos de riesgos](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

   * **Probabilidad**: indique la probabilidad de que el riesgo se presente como un valor porcentual.
   * **Costo potencial**: indique el costo estimado si se debe producir el riesgo.
   * **Costo de mitigación**: indique el costo del plan de mitigación que debe establecer para evitar que se produzca el riesgo.
   * **Costo real**: indique el costo real del riesgo si éste se produjo.
   * **Plan de mitigación**: actualice la descripción del plan para mitigar el riesgo.

1. (Condicional) Haga clic en **Introducir** si está creando el riesgo en línea.

   O

   Haga clic en **Guardar** si está editando la información en el cuadro de diálogo **Nuevo riesgo**.

1. (Opcional) Seleccione un **Estado** diferente para el riesgo, en el menú desplegable **Estado**, al aplicar la vista **Estándar** para la lista de riesgos.

   De manera predeterminada, el estado de un riesgo es **Identificado**.

### Editar riesgos en el área Riesgos {#edit-risks-in-the-risks-area}

Puede editar los riesgos durante la duración de un proyecto, cuando se producen cambios en su probabilidad, coste potencial o estado, por ejemplo.

Puede editar los riesgos de uno en uno o varios riesgos de forma masiva.

Para editar riesgos:

1. Desplácese hasta un proyecto para el que desee editar los riesgos existentes.
1. Haga clic en **Riesgos** en el panel izquierdo.
1. Comience a editar en línea los campos de los riesgos que ve en la lista para editar los riesgos de uno en uno.

   O

   Seleccione uno o varios riesgos y, a continuación, haga clic en **Editar** para editar varios riesgos al mismo tiempo.

   >[!NOTE]
   >
   >Aplica la misma información a todos los riesgos seleccionados al editar varios riesgos al mismo tiempo. La información asociada con cada riesgo antes de los cambios se sobrescribe en una edición masiva.

1. Si ha hecho clic en **Editar**, se abrirá el cuadro de diálogo **Editar riesgo**.

   Considere la posibilidad de editar los campos siguientes:

   * **Descripción**: edite la descripción del riesgo.
   * **Tipo de riesgo**: indique en qué categoría se encuentra el riesgo.
   * **Probabilidad**: indique la probabilidad de que el riesgo se presente como un valor porcentual.
   * **Costo potencial**: indique el costo estimado si se debe producir el riesgo.
   * **Costo de mitigación**: indique el costo del plan de mitigación que debe establecer para evitar que se produzca el riesgo.
   * **Costo real**: indique el costo real del riesgo si éste se produjo.
   * **Plan de mitigación**: actualice la descripción del plan para mitigar el riesgo.

1. Haga clic en **Guardar cambios**.
1. (Opcional) Edite el **Estado** de un riesgo, en el menú desplegable **Estado**, al aplicar la vista **Estándar** para la lista de riesgos.

   >[!NOTE]
   >
   >No puede editar el **estado** de los riesgos en el cuadro de diálogo **Editar riesgo**. Solo puede hacerlo en una edición en línea.
