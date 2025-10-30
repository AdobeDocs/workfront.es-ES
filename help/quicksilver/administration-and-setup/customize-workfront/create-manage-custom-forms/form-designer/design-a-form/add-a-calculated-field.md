---
title: Agregar campos calculados a un formulario
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede añadir un campo personalizado calculado que utilice datos existentes para generar datos nuevos cuando el formulario personalizado se adjunte a un objeto.
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 407aae49-4bc3-4364-a794-7e170a57a6d3
source-git-commit: f6e0329ec63038b33006325701007c564c4126cc
workflow-type: tm+mt
source-wordcount: '2446'
ht-degree: 79%

---

# Añadir campos calculados a un formulario

{{preview-fast-release-general}}

<!-- Audited: 5/2025 -->

Puede añadir un campo personalizado calculado que utilice datos existentes para generar datos nuevos cuando el formulario personalizado se adjunte a un objeto.

Un campo personalizado calculado puede contener:

* Una sencilla referencia a un único campo integrado.

  >[!INFO]
  >
  >**Ejemplo:** Para calcular los ingresos generados por proyectos y tareas, puede crear un campo personalizado calculado que contenga el campo integrado Ingresos reales. Cuando alguien adjunte el formulario personalizado a un proyecto o tarea, los ingresos del proyecto o tarea se mostrarán en el campo.

* Expresión que hace referencia a uno o varios campos. Pueden ser campos personalizados, otros campos personalizados calculados y campos integrados.

  >[!INFO]
  >
  >**Ejemplo:** Para calcular el beneficio generado por proyectos y tareas, puede crear un campo personalizado calculado denominado Beneficio que contenga una expresión matemática que reste el coste de los ingresos.
  >
  >Para ello, se puede utilizar la expresión matemática SUB (subtract) con los campos integrados de Workfront Coste real e Ingresos reales.
  >
  >En los pasos siguientes, puede ver cómo crear una expresión como en este ejemplo.

>[!NOTE]
>
>Los cambios en un campo directo almacenan automáticamente en déclencheur una actualización del valor del campo calculado. (Los campos directos son campos disponibles en el Explorador de API de Workfront o campos personalizados en un formulario personalizado adjunto a un objeto). Los cambios realizados en una referencia o fórmula requieren que se recalculen manualmente los valores de los campos.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>paquete de Adobe Workfront</td> 
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

## Reutilizar un campo personalizado calculado existente en un formulario personalizado

Puede utilizar el mismo campo personalizado calculado en formularios personalizados que pertenezcan a objetos diferentes. Por ejemplo, puede utilizar el campo calculado Beneficio que ha creado para el formulario personalizado del proyecto en un formulario personalizado de tarea.

Al utilizar un campo personalizado calculado existente, el cálculo no se transfiere al nuevo formulario. Debe volver a agregar el cálculo en el mismo campo del nuevo formulario personalizado.

Puede tener un cálculo diferente para el mismo campo en el nuevo formulario. Mantener el mismo nombre para el campo personalizado calculado garantiza la coherencia y la cohesión en la convención de nomenclatura.

>[!IMPORTANT]
>
>Los cambios en las expresiones calculadas pueden hacer que el valor del campo en los objetos quede obsoleto. Para asegurarse de ver siempre el cálculo actualizado en estos campos, realice una de las siguientes acciones:
>
>* Después de guardar un objeto en el que haya editado datos en un formulario personalizado adjunto, haga clic en el icono Más ![Icono Más](assets/more-icon.png) de la página principal del objeto y, a continuación, vuelva a calcular las expresiones personalizadas.
>* Seleccione la opción Recalcular expresiones personalizadas al editar objetos de forma masiva.
>* Seleccione la opción Actualizar cálculos anteriores al editar un campo personalizado calculado en un formulario personalizado.

Para reutilizar un campo personalizado calculado existente:

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Forms personalizado** y luego en **Forms**.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Haga clic en **Nuevo formulario personalizado**.

1. En el cuadro de diálogo **Nuevo formulario personalizado**, seleccione a qué tipos de objeto desea adjuntar el formulario personalizado y, a continuación, haga clic en **Continuar**.
1. En la parte superior izquierda de la pantalla, haga clic en **Biblioteca de campos**.

   ![Biblioteca de campos](assets/field-library.png)

1. Utilice el cuadro de búsqueda o expanda la sección **Calculado** para localizar el campo calculado que necesita y, a continuación, arrastre el campo al lugar donde desea que aparezca en el formulario personalizado.

1. (Opcional) Repita el paso anterior para añadir otros campos.

   >[!NOTE]
   >
   >Puede añadir hasta 500 campos y widgets en un único formulario personalizado. Sin embargo, puede producirse una degradación del rendimiento cuando existan más de 100 campos en un formulario, según su complejidad. 
   >
   >
   >Algunos ejemplos de formularios complejos son los formularios con parámetros en cascada, los campos de datos personalizados calculados y varias opciones de valor en un único campo.

1. Para guardar los cambios, haga clic en **Aplicar** y pase a otra sección para seguir creando el formulario.

   o

   Haga clic en **Guardar y cerrar**.

## Añadir un nuevo campo calculado

>[!IMPORTANT]
>
>Antes de crear un nuevo campo personalizado calculado, identifique los campos existentes que desee incluir para estar seguro de que los datos necesarios para el cálculo están presentes en Workfront.

{{step-1-to-setup}}

1. En el panel izquierdo, haga clic en **Forms personalizado** y luego en **Forms**.

1. Haga clic en **Nuevo formulario personalizado**.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. En el cuadro de diálogo **Nuevo formulario personalizado**, seleccione a qué tipos de objeto desea adjuntar el formulario personalizado y, a continuación, haga clic en **Continuar**.

1. En el lado izquierdo de la pantalla, busque **Calculado** y arrástrelo hasta una sección del lienzo.

   ![Arrastrar campo a sección](assets/drag-field-to-section.png)

1. En el lado derecho de la pantalla, configure las opciones disponibles para el tipo de campo personalizado que va a añadir:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td>Escriba una etiqueta para el campo. Es lo que los usuarios verán cuando usen el formulario personalizado. Workfront, en los informes, hace referencia al campo <b>Nombre</b>, que se rellena automáticamente.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">Instrucciones</td> 
      <td> De forma predeterminada, la fórmula que cree para el campo se almacena aquí. Puede añadir texto para ofrecer información adicional sobre el campo y la fórmula que contiene. Esto puede resultar útil de dos maneras: 
       <ul> 
      <li><p>Como recordatorio de lo qué es la fórmula y cómo funciona. Resulta especialmente útil si piensa utilizar este campo personalizado calculado en varios formularios.</p> </li> 
      <li> <p>Como ayuda contextual, los usuarios pueden ver cuando pasan el puntero por encima del campo. Aquí puede añadir el texto que desee que vean en la ayuda contextual.</p> <p>Si no desea que vean la fórmula en la ayuda contextual, lo que puede resultar confuso para ellos, puede ocultarla.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td> 
      <td> <p>El formato en el que desea que se almacenen y muestren los resultados del campo.</p> <p>Si el campo se va a utilizar en cálculos matemáticos, utilice siempre un formato <strong>Número</strong> o <strong>Moneda</strong>. Si selecciona <strong>Número</strong> o <strong>Moneda</strong>, el sistema trunca automáticamente los números que comienzan por 0.</p> 
      <p><b>IMPORTANTE</b>: antes de elegir un formato, tenga en cuenta el formato correcto para el nuevo campo. El campo de formato no se puede editar después de guardar el formulario personalizado. Y seleccionar el formato incorrecto podría afectar a futuros cálculos y valores acumulados en las agrupaciones de informes y listas.</p>
      <p><strong>NOTA</strong>: los campos calculados con un formato <strong>Divisa</strong> no deben incluir comillas. (Por ejemplo, use 800,00 y no "800,00"). El uso de comillas puede tener consecuencias inesperadas debido a los matices del formato de idioma para los tipos de moneda.</p></td>
     </tr> 
     <tr>
      <td><span class="preview">Activo</span></td>
      <td><span class="preview"><p>Esta opción está activada de forma predeterminada.<p><p>Cuando se establece un campo como Inactivo, se excluye de los informes, filtros y vistas y ya no está disponible en la biblioteca de campos de formularios personalizados.</p></span></td>
     </tr>
    </tbody> 
   </table>

1. En el cuadro **Cálculo**, empiece a crear el cálculo:
   1. Haga clic en **Maximizar** para abrir el Editor de cálculos y generar el cálculo.</p>
Un cálculo suele comenzar con una expresión, seguida de paréntesis que contienen los campos a los que se desea hacer referencia cuando se adjunta el formulario personalizado a un objeto.

      Cada campo debe estar comprendido entre corchetes. Cuando empiece a escribir el nombre de un campo, el sistema realiza sugerencias y puede seleccionar una para insertarla en el cálculo.

      +++ **Ampliar para ver la sintaxis requerida en los campos personalizados calculados**

      Cada campo debe utilizar la sintaxis que se explica a continuación, con corchetes entre cada nombre de campo. Cuando empiece a escribir el nombre de un campo, el sistema realiza sugerencias y puede seleccionar una para insertarla en el cálculo. Si introduce datos incorrectamente en un cálculo, un mensaje de advertencia le avisará. No puede guardar el formulario a menos que edite el cálculo para que contenga campos válidos y una expresión calculada válida.

      >[!NOTE]
      >
      >Actualmente, el sistema solo realiza sugerencias cuando empiece a escribir el nombre de un campo al que desea hacer referencia en un objeto al que se adjuntará el formulario personalizado. No se sugieren campos del objeto principal.

      **Poner los nombres de campo entre llaves**

      * Si desea que el cálculo haga referencia a un campo integrado, el nombre del campo debe estar entre llaves.

        Por ejemplo, `{actualRevenue}`

        Los nombres de campo distinguen entre mayúsculas y minúsculas y deben aparecer en el cálculo exactamente como aparecen en el sistema de Workfront.

        Vaya a [Explorador de API de Workfront](https://developer.adobe.com/workfront/api-explorer/) para identificar los nombres de campo que se pueden utilizar en los cálculos.

      * Si desea que el cálculo haga referencia a un campo personalizado, el nombre del campo debe ir entre llaves y precedido de `DE:` dentro de las llaves.

        Por ejemplo, `{DE:Profit}`

        El sistema enumera todos los campos personalizados que puede elegir al escribir `DE:`.

         * Si desea que el cálculo haga referencia a un campo que extraerá datos del objeto *parent* cuando el formulario personalizado esté adjunto a un objeto, debe anteponer el nombre del campo al tipo de objeto del objeto principal, también entre llaves.

        Por ejemplo, si el formulario personalizado está configurado para trabajar con tareas y desea que el campo calcule los ingresos reales del objeto principal cuando el formulario se adjunta a una tarea, debe indicar `Project` como el tipo de objeto del campo:

        `{project}.{actualRevenue}`

        O bien, si es un campo personalizado:

        `{project}.{DE:profit}`

        **Separar elementos con puntos**

        Cuando haga referencia a un objeto relacionado en un campo personalizado calculado, debe separar los nombres y atributos de los objetos con puntos.

        Por ejemplo, en un formulario personalizado de tipo de tarea, para mostrar el nombre del Propietario de portafolio en un campo personalizado calculado, debe escribir lo siguiente:

        `{project}.{porfolio}.{owner}`

        Esto determinaría lo siguiente: desde el objeto del formulario personalizado (una tarea), puede acceder al siguiente objeto relacionado con la tarea (un proyecto). Desde allí, puede acceder al siguiente objeto relacionado con el proyecto (un portafolio) y, a continuación, hacer referencia a los campos definidos para el objeto del portafolio (el propietario)

        **Sintaxis de nombre para hacer referencia a un campo personalizado**

        Cuando haga referencia a otro campo personalizado en un campo personalizado calculado, debe introducir el nombre del campo tal y como se muestra en la interfaz de usuario de Workfront.

        Por ejemplo, para hacer referencia a la opción seleccionada en un campo personalizado denominado Patrocinador ejecutivo, debe escribir lo siguiente:

        `{DE:Executive sponsor}`

        >[!NOTE]
        >
        >La sintaxis de un campo de escritura anticipada es un poco diferente a la de otros tipos de campos porque necesita añadir `:name` al final.
        >
        >Por ejemplo, para hacer referencia a la opción seleccionada en un campo de escritura anticipada personalizado denominado &quot;Patrocinador ejecutivo&quot;, escribiría:
        >
        >`{DE:Executive sponsor:name}`


        **Campos personalizados calculados en formularios personalizados de varios objetos**

        En un formulario personalizado de varios objetos, los tipos de objeto seleccionados deben ser compatibles con al menos un campo al que se haga referencia en los campos personalizados calculados del formulario. Los campos no compatibles con el objeto mostrarán N/D en el formulario.

        Para asegurarse de que el campo calculado muestra un resultado correcto para todos los tipos de objeto, debe utilizar `$$OBJCODE` para definir un cálculo para cada tipo de objeto.

        >[!INFO]
        >
        >**Ejemplo:**
        >
        >En un formulario personalizado configurado para trabajar con proyectos, tareas y problemas, puede utilizar la siguiente fórmula para mostrar el tipo de objeto:
        >
        >`IF($$OBJCODE="PROJ","This is a project",IF($$OBJCODE="TASK","This is a task","This is an issue"))`
        >
        >En un proyecto, el campo mostrará &quot;Esto es un proyecto&quot;, en una tarea mostrará &quot;Esto es una tarea&quot; y en un problema dirá &quot;Esto es un problema&quot;.


        >[!INFO]
        >
        >**Ejemplo:** Aunque no hay ningún campo Asignado a: Nombre en los proyectos, hay un campo Propietario integrado (que se rellena automáticamente con el nombre de la persona que creó el proyecto, a menos que alguien lo cambie manualmente).
        >
        >Por lo tanto, en su campo personalizado A cargo, puede utilizar `$$OBJCODE` como se muestra a continuación para hacer referencia al campo Propietario cuando el formulario personalizado se adjunta a un proyecto y al campo Asignado a: Nombre cuando el formulario se adjunta a una tarea:
        >
        >`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

        Para obtener más información acerca de variables como `$$OBJCODE,`, consulte [Información general de las variables de filtro comodín](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

        **Actualizaciones automáticas de campos personalizados calculados**

        Los campos personalizados calculados en un objeto se vuelven a calcular automáticamente cuando ocurren las siguientes cosas:

         * Algo en el objeto cambia, como un cálculo diario de la línea de tiempo.
         * Alguien edita otro campo al que se hace referencia mediante un campo personalizado calculado en el objeto.
         * La expresión calculada está vacía y el campo contiene un valor; esto establece el valor en nulo.

           >[!NOTE]
           >
           ><div>En un formulario personalizado adjunto a un objeto, las instrucciones de fecha y hora de los campos personalizados calculados se calculan y guardan a partir de la hora universal coordinada (UTC), no mediante las configuraciones de zona horaria establecidas para la instancia de su organización y el perfil de usuario. Los cálculos de un formulario personalizado se generan en función de las zonas horarias individuales de cada usuario.</div>

        +++

   1. Haga clic en el cuadro de texto grande y, a continuación, haga clic en **Expresiones** y **Campos** que están disponibles para añadirlos al cálculo.

      Expanda un nombre de objeto bajo **Campos** para ver todos los campos disponibles para ese objeto. La lista está limitada a 200 elementos. Si conoce el nombre del campo, puede buscarlo.

      También puede empezar a escribir una expresión o campo en el cuadro de texto grande y, a continuación, seleccionarlo cuando se muestre. Cada elemento se muestra con una &quot;F&quot; para el campo o una &quot;E&quot; para la expresión.

      Si escribe un paréntesis de apertura, el paréntesis de cierre se añade automáticamente.

      +++ **Amplíe para ver sugerencias útiles**

      >[!TIP]
      >
      >Puede realizar cualquiera de las siguientes acciones para obtener ayuda con el cálculo:
      > 
      >* Pase el ratón sobre una expresión del cálculo para ver una descripción, un ejemplo que muestra cómo se puede usar y un vínculo de **Más información** para obtener más información en el artículo [Información general sobre las expresiones de datos calculados](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
      >  ![Texto de ayuda de expresión](assets/hover-expression-help-text.jpg)
      >* Utilice la codificación de color para identificar los componentes que ha añadido. Las expresiones se muestran en azul y los campos en verde.
      >  ![Colores para expresiones de campo](assets/colors-fields-expressions.jpg)
      >* Busque errores de cálculo resaltados en rosa a medida que avanza. Puede situarse sobre un error resaltado para mostrar una breve descripción de su causa.
      >  ![Ayuda de error](assets/error-help.png)
      >* En el área debajo del cálculo, previsualice los resultados de un objeto de Workfront existente.
      ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->
      >  ![Cálculo de vista previa](assets/preview-calc.jpg)
      >* Expresiones de referencia en un cálculo largo utilizando los números de línea que se muestran a la izquierda.

      +++
   1. Haga clic en **Minimizar** cuando termine de crear el cálculo para el campo personalizado calculado.

   1. (Opcional) Utilice cualquiera de las siguientes opciones para configurar aún más el campo personalizado calculado:

      <table style="table-layout:auto">
   <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Agregar lógica</td> 
      <td>Puede agregar Lógica de visualización para determinar si el campo calculado se muestra, en función de al menos una opción que realice un usuario en un campo de opción múltiple anterior (Lista desplegable, Casillas de verificación o Botones de opción) al rellenar el formulario. <!-- For more information, see <a href="Need to add link for new article when it's written" class="MCXref xref">Add display logic and skip logic to a custom form</a>.--> <p>Esto solo está disponible cuando al menos una casilla de verificación, un botón de opción o un campo desplegable preceden al campo personalizado calculado en el formulario. </p> <p>La lógica de omisión no está disponible para los campos personalizados calculados.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actualizar cálculos anteriores</td> 
      <td>Cuando esté editando un campo personalizado calculado existente, puede seleccionar esta opción para activar una actualización en el cálculo cuando guarde el formulario personalizado. Esto solo ocurre una vez al guardar el formulario personalizado. Una vez se hace, la opción vuelve a su estado deshabilitado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar fórmula en las instrucciones</td> 
      <td>Deje esta opción habilitada si desea que los usuarios que rellenan el formulario personalizado vean la fórmula del campo cuando pasen el puntero por encima del campo. Para obtener más información, consulte <a href="#instructions" class="MCXref xref">Instrucciones</a> más arriba en la tabla.</td> 
     </tr> 
    </tbody> 
   </table>

1. Para guardar los cambios, haga clic en **Aplicar** y pase a otra sección para seguir generando el formulario.

   o

   Haga clic en **Guardar y cerrar**.
