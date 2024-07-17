---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: Agregar un campo personalizado a un formulario personalizado con el generador de formularios heredado
description: Cuando esté trabajando en un formulario personalizado, puede crear un nuevo campo personalizado y agregarlo a un formulario personalizado. También puede agregar un campo personalizado que ya se haya agregado a otro formulario personalizado.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 3579ae0f-1d2e-4ff5-bbdf-58fdd20d01d7
source-git-commit: 6b2a2160b5daaa94374707bad4b026daa13edf06
workflow-type: tm+mt
source-wordcount: '2338'
ht-degree: 2%

---

# Agregar un campo personalizado a un formulario personalizado con el generador de formularios heredado

<!-- Audited: 02/2024 -->

{{form-designer-default}}

Cuando esté trabajando en un formulario personalizado, puede crear un nuevo campo personalizado y agregarlo a un formulario personalizado.

También puede agregar un campo personalizado que ya se haya agregado a otro formulario personalizado. Para obtener instrucciones, consulte [Reutilizar un campo o widget personalizado en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

Para obtener información sobre cómo agregar un widget de recurso a un formulario personalizado, que es un proceso similar a agregar un campo personalizado, consulte [Agregar o editar un widget de recurso en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

>[!NOTE]
>
>En un formulario personalizado que contiene muchos campos personalizados o muchas opciones de selección múltiple en campos personalizados, es posible que los usuarios experimenten un rendimiento más lento al agregar o cambiar valores en esos campos. Por ejemplo, un formulario que contenga 100 campos personalizados o campos personalizados de selección múltiple con más de 200 opciones podría ser más lento cuando los usuarios interactúen con él.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td>Acceso administrativo a formularios personalizados </td> 
  </tr>  
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Agregar un campo personalizado a un formulario personalizado {#add-custom-field-to-custom-form}

1. Empiece a crear o editar un formulario personalizado, tal como se describe en [Crear o editar un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. Seleccione la ficha **Agregar un campo**.

   ![Agregar una ficha de campo](assets/add-a-field.jpg)

1. Con **Nuevo campo** ![Nuevo icono de campo](assets/new-field.jpg) seleccionado, seleccione uno de estos tipos de campo:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Campo de texto de línea única</td> 
      <td>Permite a los usuarios escribir una sola línea de texto en el campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Campo de texto de párrafo</td> 
      <td>Permite a los usuarios escribir varias líneas de texto en el campo.</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Campo de texto con formato</td> 
      <td>Permite a los usuarios escribir varias líneas de texto en el campo y aplicarle formato con negrita, cursiva, subrayado, viñetas, numeración, hipervínculos y comillas de bloque. Está disponible en Inicio, en el área de Actualizaciones, en las listas y en el área de Detalles para los objetos de Workfront. Un límite de 15 000 caracteres permite texto y formato abundantes.</p> <p>Este tipo de campo personalizado no se admite en filtros de listas e informes.</p> <p>Para obtener información sobre cómo obtener acceso a este campo a través de la API, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/rich-text-field-storage-in-the-api.md" class="MCXref xref">Almacenamiento de campo de texto enriquecido en la API</a>.</p> <p><b>NOTA</b>: Los campos de texto con formato no están disponibles para las aplicaciones móviles de Workfront. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Lista desplegable</td> 
      <td>Proporciona una lista de opciones desplegables.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Escritura anticipada </td> 
      <td>Permite a los usuarios escribir el nombre de un objeto que existe en Workfront. Aparece una lista de sugerencias cuando el usuario empieza a escribir.
      Este tipo de campo admite los siguientes objetos:
      <ul><li>Usuario</li>
      <li>Grupo</li>
      <li>Función</li>
      <li>Portafolio</li>
      <li>Programar</li>
      <li>Proyecto</li>
      <li>Equipo</li>
      <li>Plantilla</li>
      <li>Compañía</li>
      </ul>      
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Calculado</td> 
      <td>Permite definir una expresión y mostrar el resultado en el formulario personalizado. Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md" class="MCXref xref">Agregar datos calculados a un formulario personalizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Fecha</td> 
      <td>Muestra un calendario en el que los usuarios pueden seleccionar una fecha y una hora.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Casillas de verificación</td> 
      <td>Permite a los usuarios seleccionar varias opciones.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Botones de radio</td> 
      <td>Requiere que los usuarios seleccionen solo una opción.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texto descriptivo</td> 
      <td>Permite incluir instrucciones y vínculos a páginas fuera de Workfront.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Salto de sección</td> 
      <td>Un salto de sección no es en realidad un campo. Puede utilizar un salto de sección para organizar los campos personalizados y los widgets en secciones y, si es necesario, configurar diferentes permisos de visualización y edición para cada sección. Para obtener información acerca de cómo agregar y configurar saltos de sección, vea <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md" class="MCXref xref">Agregar un salto de sección a un formulario personalizado</a>.</td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Los campos que permiten selecciones múltiples, como la casilla de verificación y la lista desplegable, son difíciles de representar en gráficos y agrupar en los informes. Para facilitar la creación de gráficos y la agrupación en los informes, puede crear campos independientes para cada opción (por ejemplo, un campo de texto de una sola línea).

1. En la ficha **Configuración de campo**, configure las opciones disponibles para el tipo de campo personalizado que está agregando:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td> <p>(Obligatorio) Escriba una etiqueta descriptiva para mostrar encima del campo personalizado. Puede cambiar la etiqueta en cualquier momento.</p> <p><b>IMPORTANTE</b>: evite utilizar caracteres especiales en esta etiqueta. No se muestran correctamente en los informes.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Nombre</td> 
      <td> <p>(Obligatorio) Este nombre es el modo en que el sistema identifica el campo personalizado cuando se agrega a varias áreas de Workfront, como informes, Inicio e interacciones de API.</p> <p>Cuando configure el campo personalizado por primera vez y escriba la etiqueta, el campo Nombre se rellenará automáticamente para que coincida. Sin embargo, los campos Etiqueta y Nombre no están sincronizados, lo que le da la libertad de cambiar la etiqueta que ven los usuarios sin tener que cambiar el nombre que ve el sistema.</p> 
      <p><b>IMPORTANTE</b>:   
      <ul> 
      <li>Aunque es posible hacerlo, le recomendamos que no cambie este nombre después de que usted u otros usuarios empiecen a utilizar el formulario personalizado en Workfront. Si lo hace, el sistema ya no reconocerá el campo personalizado, donde ahora se podría hacer referencia a él en otras áreas de Workfront. <p>Por ejemplo, si agrega el campo personalizado a un informe y posteriormente cambia su nombre, Workfront no lo reconocerá en el informe y dejará de funcionar correctamente allí a menos que lo vuelva a agregar al informe con el nuevo nombre.</p> </li>
      <li> <p>Se recomienda no escribir un nombre que ya se utilice en los campos integrados de Workfront.</p> </li>
      <li><p>Se recomienda no utilizar el carácter punto/punto en el nombre del campo personalizado para evitar errores al utilizar el campo en diferentes áreas de Workfront.</p></li>
      </ul> <p>Cada nombre de campo personalizado debe ser único en la instancia de Workfront de su organización. De este modo, puede reutilizar uno que ya se haya creado para otro formulario personalizado. Para obtener más información, consulte <a href="#add-a-custom-field-to-a-custom-form">Agregar un campo personalizado a un formulario personalizado</a> en este artículo.</p> </td>
     </tr> 
     <tr> 
      <td role="rowheader">Instrucciones</td> 
      <td> <p>Escriba cualquier información adicional sobre el campo personalizado. Cuando los usuarios rellenan el formulario personalizado, pueden pasar el ratón sobre el icono del signo de interrogación para ver la información del objeto que contiene la información que escriba aquí.</p> 
      <p> <img src="assets/custom-field-tooltip.png"> </p>
      </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td> 
      <td> <p>Seleccione el tipo de datos que se capturarán en el campo personalizado. Puede cambiar la selección de formato después de guardar el formulario, pero el nuevo formato debe admitir el valor introducido.</p>

   <p><strong>Ejemplo:</strong> Si guarda un valor numérico para un campo con formato de texto en al menos un objeto y posteriormente cambia el formato a Número o Moneda, no se producirá ningún error. </p>
      <p>Sin embargo, si guarda un valor alfanumérico en un campo con formato de texto en al menos un objeto y, a continuación, intenta cambiar el formato a Número o Moneda, se producirá un error porque el valor alfanumérico guardado no es compatible con los formatos Número o Moneda. </p>

   <p><strong>Nota:</strong> El límite de caracteres para los campos de tipo Número es de 16. También puede utilizar un campo Text para introducir números y evitar el límite.</p>

   </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de presentación</td> 
      <td>(Solo listas desplegables, casillas de verificación y botones de opción) Cambie el tipo de selección de opciones que desee para el campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tamaño</td> 
      <td>(Solo campos de texto) Seleccione una anchura para el campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar hora del día</td> 
      <td>(Solo campos de fecha) Seleccione esta opción si desea mostrar la hora del día junto con la fecha en el campo.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tipo de objeto referenciado</td> 
      <td> <p>(Solo campos de escritura anticipada) Seleccione el tipo de objeto que desea asociar al campo.</p> <p>Una vez que haya hecho clic en Aplicar o en Guardar+Cerrar, no puede cambiar el tipo de objeto del campo.</p> <p><b>NOTA</b>:   
        <ul> 
         <li>Si el administrador de Workfront personalizó el nombre para Portfolio, Programas o Proyectos en la interfaz de usuario de Workfront, el nombre predeterminado de Workfront para el objeto aparecerá en esta lista desplegable, no en el nombre personalizado. Póngase en contacto con el administrador de Workfront si necesita ayuda con esto.<br></li> 
         <li>Los siguientes tipos de objetos son compatibles con las aplicaciones móviles de iOS y Android Workfront: usuario, empresa, grupo, función de trabajo, Portfolio, programa, proyecto y plantilla.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Agregar filtro</td> 
      <td> <p>(Solo campos de escritura anticipada) Agregue un filtro para un tipo de objeto para limitar los objetos que los usuarios pueden elegir cuando utilizan el campo. </p> <p>Por ejemplo, puede limitar un campo para que los nombres de usuario solo se puedan seleccionar si cumplen los siguientes criterios:</p> 
       <ul> 
        <li>Pertenecen a uno o varios grupos especificados</li> 
        <li>Están asociados a un rol o cargo que especifique</li> 
        <li>Pertenecen al mismo grupo que la persona que utiliza el campo</li> 
       </ul> <p>Debe definir el filtro para el tipo de objeto seleccionado mediante la sintaxis de Modo de texto. Para obtener información acerca de cómo crear un filtro mediante el modo de texto, vea <a href="/help/quicksilver/reports-and-dashboards/reports/text-mode/edit-text-mode-in-filter.md" class="MCXref xref">Editar un filtro mediante el modo de texto</a>.</p>
       <p><b>NOTA</b>:   
        <ul> 
         <li>Si está editando un formulario personalizado existente, al agregar un filtro a un campo de escritura anticipada no se elimina ningún objeto (fuera del ámbito del filtro) que los usuarios ya hayan agregado mediante el campo.</li> 
         <li>Este filtro no está disponible en dispositivos móviles. Si utiliza el filtro para un campo de escritura anticipada, el campo aparecerá en los dispositivos móviles de los usuarios no afectados por el filtro.</li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Texto descriptivo</td> 
      <td>(Solo campos de texto descriptivo) Escriba el texto que desea mostrar para proporcionar instrucciones o un vínculo en el formulario personalizado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Hipervínculo</td> 
      <td>(Solo campos de texto descriptivo) Si desea aplicar un hipervínculo al texto descriptivo que ha escrito, agréguelo aquí.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Cambiar un campo a obligatorio</td> 
      <td>Seleccione esta opción si desea que el campo sea obligatorio para que el usuario complete el formulario personalizado. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Seguir cambios de los campos en las fuentes de actualización</td> 
      <td><p>Haga clic en la lista desplegable y, a continuación, seleccione los tipos de objeto donde desee rastrear automáticamente los cambios de valor del campo.</p> 
      <p><b>NOTA</b>: esta opción no está disponible para lo siguiente:</p> 
      <ul> 
      <li>Formularios personalizados asociados a los siguientes tipos de objetos: gasto, compañía, iteración, registro de facturación, documento y grupo.</li> 
      <li>Los siguientes tipos de campo: Calculado, Texto descriptivo y Salto de sección</li> 
      </ul>
      <p><b>IMPORTANTE</b>: si selecciona o anula la selección de un tipo de objeto aquí, se afectarán todos los formularios personalizados asociados con el tipo de objeto seleccionado y que contengan este campo. Por ejemplo, si anula la selección de un tipo de objeto aquí y guarda el formulario personalizado, los cambios de valor del campo ya no se rastrean para ese tipo de objeto en ningún formulario personalizado que contenga el campo.</p>
       <p>Después de seleccionar un tipo de objeto aquí para un campo y guardar el formulario personalizado, el campo se muestra en la pestaña Campos personalizados del área Actualizar fuentes de Configuración.</p> 
       <p>Por el contrario, si este campo se elimina en el área Actualizar fuentes de Configuración, el tipo de objeto de esta configuración no estará seleccionado en todos los formularios personalizados asociados al tipo de objeto y que contengan este campo.</p> 
       <p>Para obtener más información, consulte la sección <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md#add-fields-you-want-workfront-to-track">Agregar campos que desea que Workfront rastree</a> en el artículo <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/configure-system-updates.md">Configurar actualizaciones del sistema</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Agregar lógica</td>
      <td>Especifique qué campos deben aparecer en el formulario, en función de las selecciones que realicen los usuarios en los campos existentes. Para obtener más información, consulte <a href="../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md" class="MCXref xref">Agregar lógica de visualización y omitir lógica a un formulario personalizado</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Opciones </td> 
      <td> <p>(Solo desplegables, casillas de verificación o botones de opción; opcional)</p> 
       <ol> 
        <li> <p>Haga clic en <b>Opciones</b> y, a continuación, habilite cualquiera de las siguientes opciones:</p> 
           <ul> 
            <li><strong>Mostrar valores</strong>: muestra los valores de cada opción en el campo. La etiqueta de cada opción se muestra de forma predeterminada.</li> 
            <li><strong>Ordenar opciones A-Z</strong>: ordena las opciones que se agregan alfabéticamente en el campo.</li> 
           </ul> 
        </li> 
        <li> <p>Para cada opción que agregue para el usuario, haga clic en el icono de engranaje <img src="assets/gear-icon-settings.png"> y, a continuación, seleccione una de las siguientes opciones:</p> 
           <ul> 
            <li><strong>Seleccionar de forma predeterminada</strong>: seleccione la opción de forma predeterminada en el campo.</li> 
            <li> <p><strong>Ocultar opción</strong>: oculta la opción en el campo. Las opciones ocultas siguen siendo accesibles en los informes.</p> </li> 
            <li> <p><strong>Quitar opción</strong>: quite la opción del campo.</p> <p><b>ADVERTENCIA</b>: Si tiene objetos actuales que utilizan esta opción, no la quite del campo. Si lo elimina, se perderán datos históricos. En su lugar, seleccione la opción para ocultarla, lo que impide que los usuarios la seleccionen en el futuro.</p> </li> 
           </ul> 
        </li> 
       </ol> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Condicional) Para cambiar el tipo de presentación de un campo en el formulario personalizado, haga clic en el menú desplegable **Tipo de presentación** y, a continuación, haga clic en el tipo que desee.

   Puede cambiar entre los siguientes tipos de visualización de campo:

   * **Campos de tipo selección**: Casillas de verificación, Lista desplegable, Botones de opción.
   * **Campos de tipo texto**: Campo de texto de línea única, Campo de texto de párrafo. (No se puede cambiar un campo de texto con formato a otro tipo de presentación. Sin embargo, puede eliminarlo y agregar otro tipo de campo).

   Por ejemplo, si ha creado un campo Casillas de verificación, puede cambiarlo a un campo Desplegable o a un campo Botones de opción. O bien, si ha creado un campo de texto de una sola línea, puede cambiarlo a un campo de texto de párrafo.

   >[!NOTE]
   >
   >Tenga en cuenta lo siguiente cuando desee cambiar el tipo de visualización de un campo de un campo de casilla de verificación o de un campo desplegable de selección múltiple (un menú desplegable que permite seleccionar más de una opción) a un tipo de campo de selección única:
   >
   >* Si cambia a Botones de opción, Workfront conserva los valores de selección múltiple que haya introducido un usuario en el campo hasta que el usuario cambie y guarde los datos en cualquier parte del formulario. En este punto, todos los valores seleccionados mediante el campo multi-select-type se sustituyen por el valor seleccionado en el botón de opción.
   >* Si cambia a un menú desplegable de selección única, Workfront conserva los valores de selección múltiple que un usuario haya introducido en el campo hasta que el usuario cambie y guarde los valores en el campo. En este punto, cualquier valor seleccionado mediante el campo multi-select-type se reemplazará por el valor desplegable seleccionado.

1. (Opcional) Repita los pasos del 3 al 5 para agregar más campos personalizados.

   O

   Agregue campos que ya se hayan creado para su organización, como se explica en [Reutilizar un campo o widget personalizado en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   >[!NOTE]
   >
   >Puede agregar hasta 500 campos y widgets en un solo formulario personalizado. Sin embargo, puede producirse una degradación del rendimiento cuando existen más de 100 en un formulario, según su complejidad. Algunos ejemplos de formularios complejos son formularios con parámetros en cascada, campos de datos personalizados calculados y varias opciones de valor en un único campo.

1. Haga clic en **Aplicar**.
1. Si desea seguir creando el formulario personalizado de otras formas, consulte uno de los siguientes artículos:

   * [Coloque campos y widgets personalizados en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [Agregar o editar un widget de recursos en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [Agregar datos calculados a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [Agregar un salto de sección a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [Reutilizar un campo personalizado calculado existente en un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [Agregar lógica de visualización y saltar lógica a un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [Previsualización y cumplimentación de un formulario personalizado](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
