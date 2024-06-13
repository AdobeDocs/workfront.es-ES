---
title: Compartir un formulario personalizado
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede configurar el acceso a un formulario personalizado para controlar quién (persona, función, grupo, equipo, compañía) puede verlo, compartirlo y editarlo.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: a264512f-54ab-426e-8dd7-5602ece81c57
source-git-commit: 6c43d836c24f893d1b7d7d01c1dd0b1cc3fba357
workflow-type: tm+mt
source-wordcount: '1408'
ht-degree: 1%

---

# Compartir un formulario personalizado

Puede configurar el acceso a un formulario personalizado para controlar quién (persona, función, grupo, equipo, compañía) puede verlo, compartirlo y editarlo.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## Acceso a formularios personalizados {#access-to-custom-forms}

De forma predeterminada, cuando crea un nuevo formulario personalizado y alguien lo adjunta a un objeto, cualquier usuario asignado al objeto puede ver y rellenar el formulario. Esto incluye a los usuarios con licencias de solicitud y a los usuarios externos.

Sin embargo, en un objeto en el que el formulario personalizado no esté adjunto, un usuario (incluso si tiene un nivel de acceso de Planificador) no puede adjuntarlo desde el menú desplegable Forms personalizado a menos que se cumpla una de las siguientes condiciones:

* Alguien compartió el formulario personalizado con el usuario o con su equipo, función del trabajo, grupo o compañía, y concedió al menos el permiso Ver con la opción Adjuntar a datos personalizados seleccionada
* El usuario tiene una licencia de planificación y su nivel de acceso permite el acceso administrativo a los formularios personalizados

## Compartir un formulario personalizado desde la lista de formularios

En lugar de dejar un formulario personalizado en el estado de uso compartido predeterminado (descrito en [Acceso a formularios personalizados](#access-to-custom-forms) en este artículo), puede configurar niveles específicos de acceso al formulario para determinados usuarios, funciones del puesto, grupos, equipos y empresas.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Seleccione el formulario personalizado y haga clic en ![Icono Compartir](assets/share-icon.png).
1. En el cuadro que se muestra, debajo de **Conceder acceso a formularios personalizados a**, empiece a escribir el nombre del usuario, equipo, función del puesto, grupo o empresa con el que desea compartir el formulario personalizado y, a continuación, pulse **Entrar** cuando se muestra el nombre.
1. Para ajustar el acceso del usuario, equipo, función del trabajo, grupo o compañía que acaba de agregar, haga clic en el menú desplegable situado a la derecha del nombre y, a continuación, configure una de las siguientes opciones disponibles y cualquiera de sus opciones avanzadas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Verlo</td> 
      <td> <p>Capacidad para ver y rellenar el formulario personalizado en objetos.</p> <p><b>NOTA</b>: Para los usuarios con licencias Light y Contributor (o licencias Work, Review y Request), esta es la opción disponible más alta.</p> <p>Clic <strong>Configuración avanzada</strong> para especificar si desea permitir lo siguiente:</p> 
       <ul> 
        <li><strong>Adjuntar a datos personalizados</strong>: capacidad para adjuntar el formulario personalizado a proyectos, tareas y problemas para los que tienen acceso de administración</li> 
        <li> <p><strong>Compartir</strong>: capacidad para compartir el formulario personalizado con otros usuarios del sistema</p> <p>Los usuarios con una licencia básica o de colaborador (o licencia de trabajo, revisión o solicitud) solo pueden compartir un formulario personalizado a través de la API o un informe de formularios personalizados.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Administrarlo</td> 
      <td> <p>Disponible solo para usuarios con licencia estándar o de planificación. </p> <p>Además de poder agregar el formulario a los objetos a los que tienen acceso para editarlo, los usuarios también pueden editar completamente el formulario personalizado, lo que incluye agregar, editar y eliminar campos.</p> <p>Clic <strong>Configuración avanzada</strong> para especificar si desea permitir lo siguiente:</p> 
       <ul> 
        <li> <p><strong>Adjuntar a datos personalizados</strong>: capacidad para adjuntar el formulario personalizado a proyectos, tareas y problemas para los que tienen acceso de administración</p> </li> 
        <li><strong>Eliminar</strong>: elimine el formulario personalizado del sistema</li> 
        <li><strong>Compartir</strong>: comparta el formulario personalizado con otros usuarios del sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita los pasos 4-5 para añadir otros nombres a la lista y configurar sus opciones.
1. (Opcional) Si desea limitar el acceso al formulario personalizado (en objetos donde esté adjunto) a los especificados en los pasos anteriores, haga clic en el icono de engranaje ![](assets/gear-icon-settings-with-dn-arrow.jpg) en la esquina superior derecha del cuadro para compartir, haga clic en **Eliminar acceso en todo el sistema**.

   Si cambia de opinión, puede hacer clic en **Hacer esto visible en todo el sistema** (la opción predeterminada).

   >[!NOTE]
   >
   >* Cuando se hace visible un formulario personalizado en todo el sistema, se permite a los usuarios ver y rellenar únicamente los objetos a los que están asignados, no adjuntarlos a otros objetos. Puede conceder la capacidad de adjuntar el formulario personalizado a objetos mediante la opción &quot;Adjuntar a datos personalizados&quot; que se explica en el paso 5.
   >* La mayoría de las organizaciones desea garantizar que todos los miembros del sistema puedan rellenar un formulario personalizado cuando esté adjunto a objetos en los que trabajan y vean sus datos en los informes. Si esto es así para su organización, le recomendamos que utilice **Hacer esto visible en todo el sistema**. Cuando la opción se configura de esta manera, aparece &quot;Visible en todo el sistema&quot; en el cuadro de diálogo:
   >   
   >![](assets/visible-system-wide-350x480.png)
   >   
   >Si le preocupa un formulario personalizado en el que los usuarios puedan introducir datos confidenciales cuando esté adjunto a determinados objetos, limitando el uso compartido de los mismos *objetos* podría ser mejor que limitar el acceso al propio formulario.

1. Haga clic en **Guardar**.

## Compartir un formulario personalizado desde el diseñador de formularios

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Abra un formulario personalizado o cree uno nuevo.
1. Clic **Compartir** en la parte superior derecha del diseñador de formularios cuando esté listo para compartir el formulario.
1. En el cuadro que se muestra, debajo de **Conceder acceso al formulario personalizado a**, empiece a escribir el nombre del usuario, equipo, función del puesto, grupo o empresa con el que desea compartir el formulario personalizado y, a continuación, pulse **Entrar** cuando se muestra el nombre.
1. Para ajustar el acceso del usuario, equipo, función del trabajo, grupo o compañía que acaba de agregar, haga clic en el menú desplegable situado a la derecha del nombre y, a continuación, configure una de las siguientes opciones disponibles y cualquiera de sus opciones avanzadas:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Verlo</td> 
      <td> <p>Capacidad para ver y rellenar el formulario personalizado en objetos.</p> <p><b>NOTA</b>: Para los usuarios con licencias Light y Contributor (o licencias Work, Review y Request), esta es la opción disponible más alta.</p> <p>Clic <strong>Configuración avanzada</strong> para especificar si desea permitir lo siguiente:</p> 
       <ul> 
        <li><strong>Adjuntar a datos personalizados</strong>: capacidad para adjuntar el formulario personalizado a proyectos, tareas y problemas para los que tienen acceso de administración</li> 
        <li> <p><strong>Compartir</strong>: capacidad para compartir el formulario personalizado con otros usuarios del sistema</p> <p>Los usuarios con una licencia básica o de colaborador (o licencia de trabajo, revisión o solicitud) solo pueden compartir un formulario personalizado a través de la API o un informe de formularios personalizados.</p> </li>
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Administrarlo</td> 
      <td> <p>Disponible solo para usuarios con licencia estándar o de planificación. </p> <p>Además de poder agregar el formulario a los objetos a los que tienen acceso para editarlo, los usuarios también pueden editar completamente el formulario personalizado, lo que incluye agregar, editar y eliminar campos.</p> <p>Clic <strong>Configuración avanzada</strong> para especificar si desea permitir lo siguiente:</p> 
       <ul> 
        <li> <p><strong>Adjuntar a datos personalizados</strong>: capacidad para adjuntar el formulario personalizado a proyectos, tareas y problemas para los que tienen acceso de administración</p> </li> 
        <li><strong>Eliminar</strong>: elimine el formulario personalizado del sistema</li> 
        <li><strong>Compartir</strong>: comparta el formulario personalizado con otros usuarios del sistema</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Opcional) Repita los pasos 5-6 para añadir otros nombres a la lista y configurar sus opciones.
1. (Opcional) Si desea limitar el acceso al formulario personalizado (en objetos donde esté adjunto) a los especificados en los pasos anteriores, haga clic en la flecha desplegable debajo de **Quién tiene acceso**, luego seleccione **Solo las personas invitadas pueden acceder a**.

   Si cambia de opinión, puede seleccionar **Todos los usuarios del sistema pueden ver**.

   >[!NOTE]
   >
   >* Cuando se hace visible un formulario personalizado en todo el sistema, se permite a los usuarios ver y rellenar únicamente los objetos a los que están asignados, no adjuntarlos a otros objetos. Puede conceder la capacidad de adjuntar el formulario personalizado a objetos mediante la opción &quot;Adjuntar a datos personalizados&quot; que se explica en el paso 6.
   >* La mayoría de las organizaciones desea garantizar que todos los miembros del sistema puedan rellenar un formulario personalizado cuando esté adjunto a objetos en los que trabajan y vean sus datos en los informes. Si esto es así para su organización, le recomendamos que utilice **Todos los usuarios del sistema pueden ver**. Cuando la opción se configura de esta manera, aparece &quot;Visible en todo el sistema&quot; en el cuadro de diálogo:
   >   
   >![Compartir formulario personalizado](assets/share-custom-form-in-designer.png)
   >   
   >Si le preocupa un formulario personalizado en el que los usuarios puedan introducir datos confidenciales cuando esté adjunto a determinados objetos, limitando el uso compartido de los mismos *objetos* podría ser mejor que limitar el acceso al propio formulario.

1. Haga clic en **Guardar**.

## Quitar el acceso a un formulario personalizado de la lista de formularios

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Forms personalizado**.
1. Seleccione el formulario personalizado y haga clic en ![Icono Compartir](assets/share-icon.png).
1. En el cuadro que aparece, haga clic en la X situada a la derecha del nombre del usuario, equipo, función, grupo o empresa a los que ya no desea tener acceso especial al formulario.
1. (Opcional) Repita el paso anterior a para los demás nombres que desee eliminar.
1. Haga clic en **Guardar**.
