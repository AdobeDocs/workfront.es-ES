---
product-area: projects
navigation-topic: business-case-and-scorecards
title: Crear y editar riesgos en proyectos
description: Los riesgos son posibles eventos o factores que impiden que un proyecto finalice a tiempo o dentro del presupuesto. Los riesgos se pueden registrar como parte de la creación del Caso de negocio de un proyecto o utilizando la pestaña Riesgos . Los riesgos solo se crean en un proyecto. No puede asociar riesgos con tareas o problemas.
author: Alina
feature: Work Management
exl-id: 6125c477-c0d8-43b4-88d8-35b0c2412468
source-git-commit: 8611c7bf8be6405f8ec8462ff2fd0f5998e8a995
workflow-type: tm+mt
source-wordcount: '1083'
ht-degree: 0%

---

# Crear y editar riesgos en proyectos

Los riesgos son posibles eventos o factores que impiden que un proyecto finalice a tiempo o dentro del presupuesto. Los riesgos se pueden registrar como parte de la creación del Caso de negocio de un proyecto o utilizando la pestaña Riesgos . Los riesgos solo se crean en un proyecto. No puede asociar riesgos con tareas o problemas.

Los riesgos pueden asociarse con el costo, pero el costo real de riesgo no afecta al costo real del proyecto.

>[!NOTE]
>
>Este artículo define los riesgos asociados al proyecto tal como los define en el caso empresarial del proyecto o a medida que los añade en la pestaña Riesgos del proyecto. Para obtener información sobre el campo Riesgo que está disponible al editar un proyecto, consulte [Editar proyectos](../../../manage-work/projects/manage-projects/edit-projects.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a Proyectos y Datos Financieros</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede cambiar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Permisos de objeto</td> 
   <td> <p> Administre permisos que incluyan Administrar finanzas en el proyecto para el que desee crear o editar riesgos. </p> <p>Para obtener más información sobre los permisos del proyecto, consulte el artículo <a href="../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Uso compartido de un proyecto en Adobe Workfront</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear y editar riesgos en el caso empresarial

Puede crear riesgos como parte de la planificación del caso empresarial de un proyecto. Posteriormente puede editarlos en el caso empresarial, cuando se produzcan cambios en su probabilidad, plan de mitigación o coste, por ejemplo. Para obtener información sobre cómo crear un caso práctico, consulte [Creación de un caso empresarial para un proyecto](../../../manage-work/projects/define-a-business-case/create-business-case.md).

El administrador de Workfront o el administrador de grupos deben habilitar la variable **Riesgos** del caso empresarial en el área Preferencias del proyecto para poder verlo a nivel de proyecto en la sección Caso empresarial . Para obtener información sobre cómo definir las preferencias del proyecto, consulte [Configurar las preferencias de proyecto de todo el sistema](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

La creación y edición de riesgos en Business Case es idéntica.

Para crear o editar un riesgo en el caso empresarial:

1. Vaya al proyecto para el que desea crear riesgos.
1. Haga clic en **Caso empresarial** en el panel izquierdo.
1. En el **Riesgos** , haga clic en **Editar riesgos**.
1. Introduzca o edite la siguiente información:

   * **Descripción:** describa el riesgo.

   * **Costo potencial**: indicar el coste estimado si debe producirse el riesgo.

   * **Probabilidad**: indican la probabilidad de que se produzca el riesgo como valor porcentual.

   * **Tipo:** indicar en qué categoría se encuentra el riesgo.
   * **Plan de mitigación**: actualizar la descripción del plan para mitigar el riesgo.

   * **Coste de mitigación**: indique el coste del plan de mitigación que debe poner en marcha para evitar que se produzca el riesgo.

   ![](assets/crp1-350x117.png)

1. (Opcional) Haga clic en **Añadir otro riesgo** para añadir riesgos adicionales.
1. Haga clic en **Guardar**.

## Crear y editar riesgos en el área Riesgos

Además de crear y editar riesgos en el caso empresarial, puede hacerlo utilizando la variable **Riesgos** de un proyecto.

* [Crear riesgos en el área de riesgos](#create-risks-in-the-risks-area)
* [Editar riesgos en el área de riesgos](#edit-risks-in-the-risks-area)

### Crear riesgos en el área de riesgos {#create-risks-in-the-risks-area}

1. Vaya al proyecto para el que desea crear riesgos.
1. Haga clic en **Riesgos** en el panel izquierdo.

   ![Sección de riesgos de la tarea](assets/risks-section-on-project-2022.png)

1. Haga clic en **Empezar a añadir riesgos** y crear riesgos mediante la edición en línea de su información.

   O

   Haga clic en **Nuevo riesgo**. La variable **Nuevo riesgo** se abre.

1. Introduzca la siguiente información:

   * **Descripción**: describa el riesgo.
   * **Tipo de riesgo**: indicar en qué categoría se encuentra el riesgo.\
      El administrador de Workfront define los tipos de riesgo disponibles en su entorno. Para obtener información sobre la definición de tipos de riesgo, consulte el artículo [Editar y crear tipos de riesgo](../../../administration-and-setup/set-up-workfront/configure-system-defaults/edit-create-risk-types.md).

   * **Probabilidad**: indican la probabilidad de que se produzca el riesgo como valor porcentual.
   * **Costo potencial**: indicar el coste estimado si debe producirse el riesgo.
   * **Coste de mitigación**: indique el coste del plan de mitigación que debe poner en marcha para evitar que se produzca el riesgo.
   * **Costo real**: indicar el coste real del riesgo si se produjo.
   * **Plan de mitigación**: actualizar la descripción del plan para mitigar el riesgo.

1. (Condicional) Haga clic en **Entrar** si está creando el riesgo en línea.

   O

   Haga clic en **Guardar** si está editando la información en la sección **Nuevo riesgo** para abrir el Navegador.

1. (Opcional) Seleccione otro **Estado** para el riesgo, en el **Estado** menú desplegable, al aplicar la variable **Estándar** para ver la lista de riesgos.

   De forma predeterminada, el estado de un riesgo es **Identificado**.

### Editar riesgos en el área de riesgos {#edit-risks-in-the-risks-area}

Puede editar los riesgos durante la vida de un proyecto, cuando se produzcan cambios en su probabilidad, coste potencial o estado, por ejemplo.

Puede editar un riesgo a la vez o editar varios riesgos de forma masiva.

Para editar los riesgos:

1. Desplácese a un proyecto para el que quiera editar los riesgos existentes.
1. Haga clic en **Riesgos** en el panel izquierdo.
1. Comience a editar en línea los campos de los riesgos que ve en la lista para editar un riesgo a la vez.

   O

   Seleccione uno o varios riesgos y haga clic en **Editar** para editar varios riesgos al mismo tiempo.

   >[!NOTE]
   >
   >Aplica la misma información a todos los riesgos seleccionados, cuando edita múltiples riesgos al mismo tiempo. La información asociada con cada riesgo antes de los cambios se sobrescribe en una edición masiva.

1. Si ha hecho clic en **Editar**, el **Editar riesgo** se abre.

   Considere la posibilidad de editar los campos siguientes:

   * **Descripción**: edite la descripción del riesgo.
   * **Tipo de riesgo**: indicar en qué categoría se encuentra el riesgo.
   * **Probabilidad**: indican la probabilidad de que se produzca el riesgo como valor porcentual.
   * **Costo potencial**: indicar el coste estimado si debe producirse el riesgo.
   * **Coste de mitigación**: indique el coste del plan de mitigación que debe poner en marcha para evitar que se produzca el riesgo.
   * **Costo real**: indicar el coste real del riesgo si se produjo.
   * **Plan de mitigación**: actualizar la descripción del plan para mitigar el riesgo.

1. Haga clic en **Guardar cambios**.
1. (Opcional) Edite el **Estado** para un riesgo, en el **Estado** menú desplegable, al aplicar la variable **Estándar** para ver la lista de riesgos.

   >[!NOTE]
   >
   >No se puede editar la variable **Estado** de riesgos en el **Editar riesgo** para abrir el Navegador. Solo puede hacerlo en una edición en línea.
