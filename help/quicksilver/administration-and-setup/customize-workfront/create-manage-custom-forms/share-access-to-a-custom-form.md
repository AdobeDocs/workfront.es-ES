---
title: Compartir un formulario personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede configurar el acceso para un formulario personalizado con el fin de controlar quién puede verlo, compartirlo y editarlo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
TQID: 'https://experienceleague.adobe.com/gpJQedqcdtjaxvhVuWKgJVpfAPAT2ICSgO6nRFLvimM'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ecee8b1aadd804a45ff0830e04e77981a3269cff
workflow-type: tm+mt
source-wordcount: '967'
ht-degree: 47%
---
# Compartir un formulario personalizado

Puede configurar el acceso para un formulario personalizado con el fin de controlar quién (persona, función, grupo, equipo, empresa, perfil empresarial) puede verlo, compartirlo y editarlo.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Paquete de Adobe Workfront</td> 
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

## Acceso a los formularios personalizados {#access-to-custom-forms}

De forma predeterminada, cuando crea un nuevo formulario personalizado y alguien lo adjunta a un objeto, cualquier usuario asignado al objeto puede ver y rellenar el formulario. Esto incluye a los usuarios con licencias de colaborador o solicitud y a los usuarios externos.

Sin embargo, en un objeto en el que el formulario personalizado no esté adjunto, un usuario (incluso si tiene un nivel de acceso Estándar o Planificador) no puede adjuntarlo desde el menú desplegable Forms personalizado a menos que se cumpla una de las siguientes condiciones:

* Alguien compartió el formulario personalizado como &quot;Todos los usuarios del sistema pueden verlo y adjuntarlo&quot;
* Alguien compartió el formulario personalizado con el usuario o con su equipo, función de trabajo, grupo, empresa o perfil empresarial que concede al menos el permiso Ver con la opción Adjuntar a datos personalizados seleccionada
* El usuario tiene una licencia estándar o de planificación y su nivel de acceso permite el acceso administrativo a los formularios personalizados

## Compartir un formulario personalizado

En lugar de dejar un formulario personalizado en el estado de uso compartido predeterminado (descrito en [Acceso a formularios personalizados](#access-to-custom-forms) en este artículo), puede configurar niveles específicos de acceso al formulario para determinados usuarios, roles, grupos, equipos, empresas y perfiles empresariales.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Formularios personalizados**.
1. Seleccione el formulario personalizado en la lista y haga clic en ![Compartir icono](assets/share-icon.png).

   O

   Abra un formulario personalizado o cree uno nuevo. A continuación, haga clic en **Compartir** en la parte superior derecha del diseñador de formularios.

1. En el cuadro para compartir, en **Conceder acceso a formulario personalizado a**, empiece a escribir el nombre del usuario, equipo, rol, grupo, compañía o perfil empresarial con el que desea compartir el formulario personalizado y, a continuación, presione **Entrar** cuando se muestre el nombre.
1. Para ajustar el acceso para el usuario, equipo, función de trabajo, grupo, compañía o perfil empresarial que acaba de agregar, haga clic en el menú desplegable a la derecha del nombre y, a continuación, configure una de las siguientes opciones disponibles y cualquiera de sus configuraciones avanzadas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Ver</td> 
      <td> <p>Esta opción proporciona la capacidad de ver y rellenar el formulario personalizado en objetos. En el nivel de objeto, los usuarios también deben tener al menos acceso de tipo Contribuir con la configuración avanzada <strong>Editar formulario personalizado</strong> habilitada. Por ejemplo, si el formulario está adjunto a un proyecto, los usuarios deben tener acceso de tipo Contribuir a ese proyecto; de lo contrario, no podrán rellenarlo.</p>

   <p><b>NOTA</b>: Para los usuarios con licencias Light y de colaborador (o licencias de trabajo, revisión y solicitud), esta es la opción disponible más alta.</p> <p>Haga clic en <strong>Ajustes avanzados</strong> para especificar si desea permitir lo siguiente:</p> 
       <ul> 
        <li><strong>Adjuntar a datos personalizados</strong>: capacidad para adjuntar el formulario personalizado a proyectos, tareas y problemas para los que tienen el acceso Administrar</li> 
        <li> <p><strong>Compartir</strong>: capacidad para compartir el formulario personalizado con otros usuarios del sistema</p> <p>Los usuarios con una licencia Light o de colaborador (o licencia de trabajo, revisión o solicitud) solo pueden compartir un formulario personalizado a través de la API o un informe de formularios personalizados.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Administrar</td> 
      <td> <p>Esta opción solo está disponible para usuarios con una licencia estándar o de planificación. </p> <p>Además de poder añadir el formulario a los objetos a los que tienen acceso para editarlo, los usuarios también pueden editar completamente el formulario personalizado, lo que incluye la adición, edición y eliminación de campos.</p> <p>Haga clic en <strong>Ajustes avanzados</strong> para especificar si desea permitir lo siguiente:</p> 
       <ul> 
        <li> <p><strong>Adjuntar a datos personalizados</strong>: capacidad para adjuntar el formulario personalizado a proyectos, tareas y problemas para los que tienen acceso de administración</p> </li> 
        <li><strong>Eliminar</strong>: elimina el formulario personalizado del sistema</li> 
        <li><strong>Compartir</strong>: comparte el formulario personalizado con otros usuarios del sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita los pasos del 4 al 5 para añadir otros nombres a la lista y configurar sus opciones.
1. (Opcional) Si desea limitar el acceso al formulario personalizado (en objetos donde esté adjunto) a los especificados en los pasos anteriores, haga clic en la flecha desplegable debajo de la opción **Quién tiene acceso** y, a continuación, seleccione **Solo las personas invitadas pueden acceder**.

   Si cambia de opinión, puede seleccionar **Todos los usuarios del sistema pueden verlo**.

   >[!NOTE]
   >
   >* Cuando se hace visible un formulario personalizado en todo el sistema, se permite a los usuarios ver y rellenar únicamente los objetos a los que están asignados, no adjuntarlos a otros objetos. Puede conceder la capacidad de adjuntar el formulario personalizado a objetos mediante la opción “Adjuntar a datos personalizados” que se explica en el paso 5.
   >* La mayoría de las organizaciones desea garantizar que todos los miembros del sistema puedan rellenar un formulario personalizado cuando se adjunta a objetos en los que trabajan y ver sus datos en los informes. Si esto es así para su organización, le recomendamos que utilice la opción **Todos los usuarios del sistema pueden verlo**.
   >* Si selecciona **Todos los usuarios del sistema pueden ver y adjuntar**, todos los usuarios podrán adjuntar el formulario a otros objetos.
   >
   >![Compartir un formulario personalizado](assets/share-custom-forms-all-can-attach.png)
   >   
   >Si le preocupa un formulario personalizado en el que los usuarios puedan introducir datos confidenciales cuando se adjuntan a determinados objetos, limitar el uso compartido de esos *objetos* podría ser más eficaz que limitar el acceso al propio formulario.

1. Haga clic en **Guardar**.

## Eliminar el acceso a un formulario personalizado

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Formularios personalizados**.
1. Seleccione el formulario personalizado en la lista y haga clic en ![Compartir icono](assets/share-icon.png).
1. En el cuadro para compartir, haga clic en el menú desplegable situado a la derecha del nombre del usuario, equipo, función, grupo, empresa o perfil empresarial que ya no desee que tenga acceso especial al formulario y seleccione **Quitar**.
1. (Opcional) Repita el paso anterior para los demás nombres que desee eliminar.
1. Haga clic en **Guardar**.

