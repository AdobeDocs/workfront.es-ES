---
title: Organización y previsualización de un formulario
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede organizar un formulario personalizado con Form Designer.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 08de894a-82f0-4440-a350-680d6648f01e
source-git-commit: 7373ee9f31e4b7561735920f3ff02cbd4fdce44a
workflow-type: tm+mt
source-wordcount: '1341'
ht-degree: 11%

---

# Organización y previsualización de un formulario

Puede organizar un formulario personalizado con el diseñador de formularios y obtener una vista previa del mismo para comprobar que está correctamente configurado.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Plan de Adobe Workfront</p> </td> 
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

Para obtener más información sobre el contenido de esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agregar un salto de sección

Puede agrupar los campos y widgets personalizados en un formulario personalizado en secciones con encabezados. Esto resulta útil para presentar una experiencia organizada a los usuarios que rellenan el formulario. Además, si necesita limitar el acceso a determinados campos personalizados y widgets a determinados usuarios, puede colocarlos en una sección y, a continuación, conceder acceso a la sección únicamente a esos usuarios.

Por ejemplo, si necesita realizar el seguimiento de información confidencial que solo los administradores del sistema deben poder ver o editar, puede crear un salto de sección con permisos de Solo administración y colocar los campos confidenciales en esa sección.

La configuración de acceso que seleccione para una sección está directamente vinculada a los permisos que los usuarios tienen en el objeto de Workfront donde está adjunto el formulario personalizado. Puede ocultar o mostrar una sección en función de si el usuario tiene acceso para ver, contribuir o administrar ese objeto. O puede establecer una sección en Solo administrador para que solo los usuarios con un nivel de acceso de administrador del sistema puedan acceder a ella.

Para obtener información acerca de los permisos de los objetos, vea [Información general sobre los permisos de uso compartido de los objetos](/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

Para obtener información sobre los campos y widgets personalizados en los formularios personalizados, consulte [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

### Creación y configuración del acceso a una sección de un formulario personalizado

1. Empiece a crear o editar un formulario personalizado y a agregar campos, tal como se describe en [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Haga clic en **Salto de sección** y arrástrelo a la posición que desee en el lienzo.

1. En el panel derecho, configure las opciones que desee para la sección:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima de la sección. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Descripción</td> 
      <td>Escriba texto si desea explicar a los usuarios para qué sirve la sección. Esto se muestra debajo de la etiqueta de la sección en el formulario personalizado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>Conceder acceso</p> </td> 
      <td> <p> Seleccione los permisos que necesitan los usuarios en un objeto donde se adjunta el formulario personalizado para ver esta sección y editar sus valores de campo. 
       <p>Los siguientes permisos están disponibles en <b>Los usuarios con este acceso al objeto pueden ver los valores de los campos</b>:</p> 
         <ul>
          <li><strong>Ver</strong>: vea los permisos del objeto</li>
          <li><p><b>Edición limitada</b>: (disponible solo si el objeto es un proyecto, tarea, problema o usuario):</p> 
          <p>Permite a los usuarios contribuir al objeto si se trata de un proyecto, una tarea o un problema.</p>
          <p>Permite a los usuarios editar el perfil o poseer el permiso de perfil para el objeto si es un usuario.</p></li> 
          <li><b>Editar</b>: administre permisos para el objeto </li> 
          <li><b>Solo administrador</b>: nivel de acceso de administrador del sistema</li> 
         </ul> </li> 
        <p>Los siguientes permisos están disponibles en <b>Los usuarios con este acceso al objeto pueden editar los valores de campo</b>: </p> 
         <ul> 
          <li> <p><b>Edición limitada</b>: (disponible solo si el objeto es un proyecto, tarea, problema o usuario):</p> 
           <p>Si el objeto es un proyecto, una tarea o un problema, este permiso permite a los usuarios contribuir al objeto</p>
          <p>Si el objeto es un usuario, este permiso permite a los usuarios editar el perfil o poseer el permiso de perfil para el objeto.</p> 
          <li><b>Editar</b>: administre permisos para el objeto </li> 
          <li><b>Solo administrador</b>: nivel de acceso de administrador del sistema</li> 
         </ul> </li> 
       </ul> 
       <p>Para obtener información acerca de los permisos de los objetos, vea <a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md" class="MCXref xref">Información general sobre los permisos de uso compartido de los objetos</a>.</p> 
       <p><b>NOTA</b>:  
       <ul> 
       <li> <p>Los usuarios sin los permisos especificados aquí no pueden ver los campos y widgets personalizados en la sección. </p> <p>Esto también se aplica si se muestran los valores de los campos en los informes o si se utilizan en campos calculados en los informes en modo de texto.</p> </li> 
       <li><p>Para formularios personalizados de solicitud/problema: si se necesita acceso de visualización para ver los campos en el salto de sección, pero se necesita acceso de administrador para editar los campos, los usuarios que no sean administradores no podrán ver la sección y todos sus campos cuando rellenen el formulario. Una vez creada la solicitud, los usuarios con acceso de visualización pueden ver los campos en la sección.</p></li>
       <li> <p>La asociación de varios tipos de objetos con el formulario puede cambiar los permisos de visualización y edición disponibles en estos pasos. Para obtener más información, consulte <a href="#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form" class="MCXref xref">Cómo pueden afectar varios tipos de objetos a los permisos de saltos de sección en un formulario personalizado</a> en este artículo.</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><p>Agregar lógica</p></td> 
      <td><p>Utilice la lógica de visualización para especificar si la sección debe mostrarse en el formulario, en función de las selecciones que realicen los usuarios en los campos personalizados de opción múltiple al rellenar el formulario.</p><p><strong>NOTA:</strong> Si se les ha aplicado lógica de visualización a todos los campos individuales bajo un salto de sección y todos están ocultos como resultado de la lógica, toda la sección estará oculta en el formulario personalizado. Esto sucederá incluso si la lógica de visualización no se aplica al salto de sección.</p><p>Para obtener más información, consulte <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md" class="MCXref xref">Agregar lógica de visualización y omitir lógica con el diseñador de formularios</a>.</p></td> 
     </tr> 
    </tbody> 
   </table>

1. Arrastre o agregue al menos un campo o widget personalizado a la nueva sección. Es necesario antes de guardar la sección.

1. Haga clic en **Listo**.

   >[!TIP]
   >
   >Puede hacer clic en **Aplicar** en cualquier momento mientras crea un formulario personalizado para guardar los cambios y mantener el formulario abierto.

### Cómo pueden afectar varios tipos de objetos a los permisos de salto de sección {#how-multiple-object-types-can-affect-section-break-permissions-in-a-custom-form}

El permiso de Edición limitada para saltos de sección de formularios personalizados solo está disponible para los tipos de objeto Proyecto, Tarea, Problema y Usuario.

En un formulario personalizado con un salto de sección configurado con el permiso Editar de forma limitada, si agrega uno de los demás tipos de objetos al formulario (Portfolio, Programa, Documento, Empresa, Registro de facturación, Iteración, Gasto o Grupo), se le pedirá que cambie al permiso Editar, que es compatible tanto con ese tipo de objeto como con los tipos de objeto existentes en el formulario.

>[!INFO]
>
>**Ejemplo:** En un formulario personalizado asociado al tipo de objeto Proyecto, se configura un salto de sección con el permiso Editar de forma limitada.
>
>Se agrega el tipo de objeto Portfolio al formulario, lo que significa que la opción de permiso Editar de forma limitada ya no está disponible para el salto de sección del formulario.
>
>Un mensaje en pantalla le pedirá que cambie al permiso Editar, que es el nivel mínimo de permisos compatibles tanto con el tipo de objeto Proyecto como con el tipo de objeto Portfolio.


## Colocar campos y widgets personalizados en un formulario personalizado


1. Empiece a crear o editar un formulario personalizado, tal como se describe en [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Para colocar campos y widgets personalizados en la misma fila, arrastre uno junto al otro hasta que aparezca una línea entre ellos.

   >[!NOTE]
   >
   >* Puede usar el botón **Vista previa** de la esquina superior derecha para hacerse una idea de cómo se mostrarán los campos y widgets personalizados en el formulario.
   >* Es posible que los campos y widgets personalizados no siempre se muestren igual en el formulario, según el espacio de pantalla disponible cuando un usuario lo esté viendo. Por ejemplo, el tercer campo de una fila de campos puede ajustarse a la siguiente fila de campos si el espacio horizontal es limitado.

1. (Opcional) Para colocar un campo o widget personalizado encima o debajo de otro, arrástrelo arriba o abajo hasta que aparezca una línea azul horizontal entre los elementos.

1. Para mover un campo personalizado a otra sección del formulario, puede arrastrarlo y colocarlo en su lugar, o bien hacer clic en el icono **Mover a** del campo y seleccionar la sección a la que desea moverlo.

   ![Mover el campo a una sección](assets/move-field-to-section.png)

1. Para guardar los cambios, haga clic en **Aplicar**

   o

   Haga clic en **Guardar y Cerrar**.

## Previsualización de un formulario personalizado

1. Empiece a crear o editar un formulario personalizado y a agregar campos, tal como se describe en [Crear un formulario personalizado](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

1. Haga clic en **Vista previa** en la esquina superior derecha para ver el aspecto que tendrá el formulario cuando se utilice y, a continuación, haga clic en **Finalizar vista previa** para regresar a la edición del formulario.

   >[!NOTE]
   >
   >La lógica avanzada no se admite en el modo de vista previa del diseñador de formularios.


