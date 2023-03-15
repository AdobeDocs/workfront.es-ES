---
title: Agregar campos calculados con el diseñador de formularios
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: Puede agregar un campo personalizado calculado que utilice datos existentes para generar nuevos datos cuando el formulario personalizado esté adjunto a un objeto.
author: Courtney
feature: System Setup and Administration
role: Admin
source-git-commit: 9b32c41c9f2971f3b0bbded230680677cc0b3c64
workflow-type: tm+mt
source-wordcount: '2317'
ht-degree: 0%

---


# Agregar campos calculados con el diseñador de formularios

{{highlighted-preview-article-level}}

Puede agregar un campo personalizado calculado que utilice datos existentes para generar nuevos datos cuando el formulario personalizado esté adjunto a un objeto.

Un campo personalizado calculado puede contener:

* Referencia sencilla a un único campo integrado.

   >[!INFO]
   >
   > **Ejemplo:** Para calcular los ingresos generados por los proyectos y las tareas, puede crear un campo personalizado calculado que contenga el campo integrado Ingresos reales. Cuando alguien adjunta el formulario personalizado a un proyecto o tarea, los ingresos del proyecto o la tarea se muestran en el campo .

* Expresión que hace referencia a uno o varios campos. Pueden ser campos personalizados, otros campos personalizados calculados y campos integrados.

   >[!INFO]
   >
   >**Ejemplo:** Para calcular el beneficio generado por proyectos y tareas, puede crear un campo personalizado calculado llamado Beneficio que contenga una expresión matemática que reste el coste de los ingresos.
   >
   >Para ello, puede utilizar la expresión matemática SUB (restar) con los campos integrados de Workfront Coste real e Ingresos reales.
   >
   >En los pasos siguientes, puede ver cómo se puede llevar a cabo este ejemplo.


## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan de Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td>Plan</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información sobre cómo los administradores de Workfront conceden este acceso, consulte <a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder a los usuarios acceso administrativo a determinadas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber qué plan, tipo de licencia o configuraciones de nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Reutilizar un campo personalizado calculado existente en un formulario personalizado

Puede utilizar el mismo campo personalizado calculado en formularios personalizados que pertenezcan a objetos diferentes. Por ejemplo, puede utilizar el campo calculado de beneficios que ha creado para el formulario personalizado del proyecto en un formulario personalizado de tareas.

Cuando se utiliza un campo personalizado calculado existente, el cálculo no se transfiere al nuevo formulario. Debe volver a agregar el cálculo, en el mismo campo, en el nuevo formulario personalizado.

También puede tener un cálculo diferente para el mismo campo, en el nuevo formulario. Mantener el mismo nombre para el campo personalizado calculado garantiza la coherencia y coherencia en la convención de nombres.

>[!IMPORTANT]
>
>Los cambios en las expresiones calculadas pueden hacer que el valor de campo de los objetos quede obsoleto. Para asegurarse de que siempre ve el cálculo actualizado en estos campos, realice una de las siguientes acciones:
>
>* Después de guardar un objeto en el que haya editado datos en un formulario personalizado adjunto, haga clic en el icono Más ![](assets/more-icon.png) en la página principal del objeto y, a continuación, vuelva a calcular las expresiones personalizadas.
>* Seleccione la opción Volver a calcular expresiones personalizadas al editar objetos de forma masiva.
>* Seleccione la opción Update previous calculations al editar un campo personalizado calculado en un formulario personalizado.


Para reutilizar un campo personalizado calculado existente:

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Forms personalizado** en el panel izquierdo.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Haga clic en **Nuevo formulario personalizado.**
1. Seleccione a qué tipos de objeto desea adjuntar el formulario personalizado y, a continuación, haga clic en **Continuar**.

1. En la parte superior izquierda de la pantalla, haga clic en **Biblioteca de campos**.

   ![](assets/field-library.png)

1. Utilice el cuadro de búsqueda o expanda el **Calculado** para localizar el campo calculado que necesita y, a continuación, arrastre el campo donde desea que aparezca en el formulario personalizado.

1. (Opcional) Repita el paso anterior para agregar cualquier otro campo.

   >[!NOTE]
   >
   >Puede agregar hasta 500 campos y utilidades en un solo formulario personalizado. Sin embargo, la degradación del rendimiento puede producirse cuando existen más de 100 en un formulario, según su complejidad.
   >
   >
   >Algunos ejemplos de formularios complejos son los formularios con parámetros en cascada, campos de datos personalizados calculados y varias opciones de valor en un solo campo.

1. Para guardar los cambios, haga clic en **Aplicar** y pase a otra sección para seguir creando el formulario.

   o

   Haga clic en **Guardar y cerrar**.

## Añadir un nuevo campo calculado

>[!IMPORTANT]
>
>Antes de crear un nuevo campo personalizado calculado, identifique los campos existentes que desee incluir para asegurarse de que los datos necesarios para el cálculo están presentes en Workfront.

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Forms personalizado** en el panel izquierdo.

   <!-- >[!TIP]
    >
    >In the view that appears, you can review all custom forms and custom fields that have been created for your organization. You can also see who created each form and the fields that are associated with it. -->

1. Haga clic en **Nuevo formulario personalizado.**
1. Seleccione a qué tipos de objeto desea adjuntar el formulario personalizado y, a continuación, haga clic en **Continuar**.

1. En el lado izquierdo de la pantalla, busque **Calculado** y arrástrela a una sección del lienzo.

   ![](assets/drag-field-to-section.png)

1. A la derecha de la pantalla, configure las opciones que están disponibles para el tipo de campo personalizado que está agregando:

   <table style="table-layout:auto"> 
    <col> 
    </col> 
    <col> 
    </col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Etiqueta</td> 
      <td>Escriba una etiqueta para el campo. Esto es lo que verán los usuarios cuando utilicen el formulario personalizado. El campo <b>Nombre</b>, que se rellena automáticamente, Workfront hace referencia a ella en los informes.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" id="instructions">Instrucciones</td> 
      <td> De forma predeterminada, la fórmula que cree para el campo se almacena aquí. Puede añadir texto para proporcionar información adicional sobre el campo y la fórmula que contiene. Esto puede resultar útil de dos maneras: 
       <ul> 
      <li><p>Como recordatorio de qué es la fórmula y cómo funciona. Esto resulta especialmente útil si planea utilizar este campo personalizado calculado en varios formularios.</p> </li> 
      <li> <p>Como información sobre herramientas, los usuarios pueden ver cuando pasan el ratón por encima del campo. Agregue aquí cualquier texto que desee que vean en la información del objeto.</p> <p>Si no desea que vean la fórmula en la información del objeto, lo que puede ser confuso para ellos, puede ocultarla.</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Formato</td> 
      <td> <p>Formato en el que desea almacenar y mostrar los resultados del campo.</p> <p>Si el campo se va a utilizar en cálculos matemáticos, utilice siempre un <strong>Número</strong> o <strong>Moneda</strong> formato. Cuando selecciona Número o Moneda, el sistema trunca automáticamente los números que comienzan por 0.</p> 
      <p><b>IMPORTANTE</b>: Antes de elegir un formato, considere el formato correcto para el nuevo campo. El campo de formato no se puede editar una vez guardado el formulario personalizado. Y seleccionar el formato incorrecto podría afectar a los cálculos futuros y a los valores acumulados en las agrupaciones de informes y listas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. En el **Cálculo** , empiece a crear el cálculo:
   1. Haga clic en **Maximizar** para abrir el Editor de cálculos y crear el cálculo.</p>
Un cálculo suele comenzar con una expresión, seguida de paréntesis que contienen los campos a los que desea hacer referencia cuando el formulario personalizado está adjunto a un objeto.

      Cada campo debe estar rodeado de llaves. Al empezar a escribir el nombre de un campo, el sistema realiza sugerencias y puede seleccionar una para insertarla en el cálculo.

+++ **Expandir para ver la sintaxis necesaria en los campos personalizados calculados**

      Cada campo debe utilizar la sintaxis que se explica a continuación, con llaves alrededor de cada nombre de campo. Al empezar a escribir el nombre de un campo, el sistema realiza sugerencias y puede seleccionar una para insertarla en el cálculo. Si introduce datos incorrectamente en un cálculo, aparecerá un mensaje de advertencia. No se puede guardar el formulario a menos que edite el cálculo para que contenga campos válidos y una expresión calculada válida.

      >[!NOTE]
      >
      >Actualmente, el sistema solo realiza sugerencias cuando empieza a escribir el nombre de un campo al que desea hacer referencia en un objeto al que se adjuntará el formulario personalizado. Los campos del objeto principal no se sugieren.

      **Rodee los nombres de los campos con llaves**

      * Si desea que el cálculo haga referencia a un campo integrado, el nombre del campo debe estar entre llaves.

         Por ejemplo: `{actualRevenue}`

         Los nombres de campo distinguen entre mayúsculas y minúsculas y deben aparecer en el cálculo exactamente como aparecen en el sistema Workfront.

         Vaya a la [Explorador de API de Workfront](https://developer.adobe.com/workfront/api-explorer/) para identificar los nombres de campo que se pueden utilizar en los cálculos.

      * Si desea que el cálculo haga referencia a un campo personalizado, el nombre del campo debe estar entre llaves y precedido por `DE:` entre corchetes.

         Por ejemplo: `{DE:Profit}`

         El sistema enumera todos los campos personalizados que puede elegir al escribir `DE:`.

         * Si desea que el cálculo haga referencia a un campo que extraerá datos del *parent* cuando el formulario personalizado está adjunto a un objeto, debe preceder al nombre del campo con el tipo de objeto del objeto principal, también entre llaves.

         Por ejemplo, si el formulario personalizado está configurado para funcionar con tareas y desea que el campo calcule los ingresos reales del objeto principal cuando el formulario está adjunto a una tarea, debe indicar `Project` como tipo de objeto del campo:

         `{project}.{actualRevenue}`

         O, si es un campo personalizado:

         `{project}.{DE:profit}`

         **Separar elementos con períodos**

         Cuando se hace referencia a un objeto relacionado en un campo personalizado calculado, se deben separar los nombres y atributos de los objetos con puntos.

         Por ejemplo, en un formulario personalizado de tipo tarea, para mostrar el nombre del propietario del Portfolio en un campo personalizado calculado, debe escribir lo siguiente:

         `{project}.{porfolio}.{owner}`

         Esto determinaría lo siguiente: Desde el objeto del formulario personalizado (una tarea), puede acceder al siguiente objeto relacionado con la tarea (un proyecto). Desde allí, puede acceder al siguiente objeto relacionado del proyecto (un portafolio) y, a continuación, hacer referencia a los campos definidos para el objeto de portafolio (el propietario)

         **Sintaxis del nombre para hacer referencia a un campo personalizado**

         Al hacer referencia a otro campo personalizado en un campo personalizado calculado, debe introducir el nombre del campo tal como aparece en la interfaz de usuario de Workfront.

         Por ejemplo, para hacer referencia a la opción seleccionada en un campo personalizado etiquetado como patrocinador ejecutivo, debe escribir lo siguiente:

         `{DE:Executive sponsor}`

         >[!NOTE]
         >
         >La sintaxis de un campo typeforward es un poco diferente a la de otros tipos de campos, ya que es necesario agregar `:name` al final.
         >
         >Por ejemplo, para hacer referencia a la opción seleccionada en un campo personalizado de tipo &quot;Analizador ejecutivo&quot;, debe escribir:
         >
         >`{DE:Executive sponsor:name}`


         **Campos personalizados calculados en formularios personalizados con varios objetos**

         En un formulario personalizado de varios objetos, los tipos de objeto seleccionados deben ser compatibles con al menos un campo al que se haga referencia en los campos personalizados calculados del formulario. Los campos no compatibles con el objeto mostrarán N/A en el formulario.

         Para garantizar que el campo calculado muestre un resultado correcto para todos los tipos de objeto, debe utilizar `$$OBJCODE` para definir un cálculo para cada tipo de objeto.

         >[!INFO]
         >
         >**Ejemplo:**
         >
         >En un formulario personalizado configurado para trabajar con proyectos, tareas y problemas, puede utilizar la siguiente fórmula para mostrar el tipo de objeto:
         >
         >`IF($$OBJCODE="PROJ","This is a project",IF($$OBJCODE="TASK","This is a task","This is an issue"))`
         >
         >En un proyecto, el campo mostrará &quot;Este es un proyecto&quot;, en una tarea mostrará &quot;Esta es una tarea&quot; y en un problema dirá &quot;Este es un problema&quot;.


         >[!INFO]
         >
         >**Ejemplo:** Aunque no hay asignado a: Campo Nombre de los proyectos, hay un campo Propietario integrado (que se rellena automáticamente con el nombre de la persona que creó el proyecto, a menos que alguien lo cambie manualmente).
         >
         >Por lo tanto, en el campo personalizado A cargo, puede usar `$$OBJCODE` como se muestra a continuación para hacer referencia al campo Propietario cuando el formulario personalizado está adjunto a un proyecto y Assigned To: Campo Nombre cuando el formulario está adjunto a una tarea:
         >
         >`IF($$OBJCODE="PROJ",{owner}.{name},{assignedTo}.{name})`

         Para obtener más información sobre variables como `$$OBJCODE,` see [Variables de filtro comodín](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/understand-wildcard-filter-variables.md).

         **Actualizaciones automáticas de campos personalizados calculados**

         Los campos personalizados calculados en un objeto se vuelven a calcular automáticamente cuando suceden los siguientes hechos:

         * Algo en el objeto cambia, como el cálculo diario de la cronología.
         * Alguien edita otro campo al que se hace referencia en un campo personalizado calculado del objeto.
         * La expresión calculada está vacía y el campo contiene un valor; esto establece el valor en null.

            >[!NOTE]
            >
            ><div>En un formulario personalizado adjunto a un objeto, las instrucciones de fecha y hora de los campos personalizados calculados se calculan y se guardan en la Hora universal coordinada (UTC), no en las configuraciones de zona horaria establecidas para la instancia de su organización y su perfil de usuario. Los cálculos en un formulario personalizado se generan en función de los husos horarios individuales de cada usuario.</div>

+++
   1. Haga clic en el cuadro de texto grande y, a continuación, haga clic en **Expresiones** y **Campos** que están disponibles para agregarlas al cálculo.

      También puede empezar a escribir una expresión o campo en el cuadro de texto grande y, a continuación, seleccionarlo cuando se muestre. Cada elemento aparece con una &quot;F&quot; para el campo o una &quot;E&quot; para la expresión.

      Si escribe un paréntesis de apertura, el paréntesis de cierre se agrega automáticamente.

+++ **Expandir para ver sugerencias útiles**
      >[!TIP]
      >
      >Puede realizar cualquiera de las siguientes acciones para obtener ayuda con su cálculo:
      > 
      >* Pase el ratón sobre una expresión en el cálculo para ver una descripción, un ejemplo que muestre cómo se puede utilizar y un vínculo &quot;Más información&quot; para obtener más información en el artículo [Expresiones de datos calculadas](/help/quicksilver/reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).
         >  ![](assets/hover-expression-help-text.jpg)
      >* Utilice la codificación de color para identificar los componentes que ha añadido. Las expresiones se muestran en azul y los campos en verde.
         >  ![](assets/colors-fields-expressions.jpg)
      >* Busque errores de cálculo, resaltados en rosa, a medida que avanza. Puede situarse sobre un error resaltado para mostrar una breve descripción de su causa.
         >  ![](assets/error-help.png)
      >* En el área inferior al cálculo, previsualice los resultados en un objeto de Workfront existente.
         ><!--or by providing test values (NOT READY YET; CHANGE THIS SCREENSHOT WHEN IT IS)-->

         >  ![](assets/preview-calc.jpg)
      >* Haga referencia a las expresiones en un cálculo largo utilizando los números de línea que aparecen a la izquierda.


+++
   1. Haga clic en **Minimizar** cuando haya terminado de crear el cálculo para el campo personalizado calculado.

   1. (Opcional) Utilice cualquiera de las siguientes opciones para seguir configurando el campo personalizado calculado:

      <table style="table-layout:auto">
   <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Agregar lógica</td> 
      <td>Puede agregar Lógica de visualización para determinar si se muestra el campo calculado, en función de al menos una opción que realice un usuario en un campo de opción múltiple anterior (menú desplegable, casillas de verificación o botones de opción) al rellenar el formulario. <!-- For more information, see <a href="Need to add link for new article when it's written" class="MCXref xref">Add display logic and skip logic to a custom form</a>.--> <p>Solo está disponible cuando al menos una casilla de verificación, un botón de opción o un campo desplegable precede al campo personalizado calculado del formulario. </p> <p>La lógica de omisión no está disponible para los campos personalizados calculados.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Actualizar cálculos anteriores</td> 
      <td>Cuando edita un campo personalizado calculado existente, puede seleccionar esta opción para almacenar en déclencheur una actualización en el cálculo al guardar el formulario personalizado. Esto sucede solo una vez cuando se guarda el formulario personalizado. Después de hacerlo, la opción vuelve a su estado desactivado.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Mostrar fórmula en las instrucciones</td> 
      <td>Deje esta opción activada si desea que los usuarios que rellenen el formulario personalizado vean la fórmula del campo cuando pasen el ratón por encima del campo. Para obtener más información, consulte la información sobre <a href="#instructions" class="MCXref xref">Instrucciones</a> más temprano en esta tabla.</td> 
     </tr> 
    </tbody> 
   </table>

1. Para guardar los cambios, haga clic en **Aplicar** y pase a otra sección para seguir creando el formulario.

   o

   Haga clic en **Guardar y cerrar**.


