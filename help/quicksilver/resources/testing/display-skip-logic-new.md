---
title: Agregar lógica de visualización y saltar lógica a un formulario personalizado
description: Agregar lógica de visualización y saltar lógica a un formulario personalizado
draft: Probably
source-git-commit: dd718ff8f497065018cdfb9592ff0804d7668bf8
workflow-type: tm+mt
source-wordcount: '1475'
ht-degree: 0%

---

# Agregar lógica de visualización y saltar lógica a un formulario personalizado

Puede utilizar reglas inteligentes para hacer que un formulario personalizado sea dinámico y más relevante para los usuarios que lo rellenan. Cuando un usuario responde de una determinada manera a un campo de opción múltiple en un formulario, una regla inteligente le muestra lo que desea que vea a continuación, en función de esa respuesta.

Los tipos de campo de opción múltiple son Desplegable, Casillas de verificación y Botones de opción.

* **Lógica de visualización**: configure una regla de lógica de visualización en el campo, widget o sección que desee que el usuario vea solo después de seleccionar una opción específica en un campo de opción múltiple anterior.

  **Ejemplo:** Está creando un formulario de solicitud de contenido de marketing en el que los miembros de su organización pueden solicitar un nuevo logotipo, una actualización de sitio web, un folleto u otro tipo de contenido de marketing. En función del tipo de contenido que desee el usuario, debe solicitarle diferentes tipos de detalles, como colores e ideas de diseño si necesitan un logotipo o una lista de funciones de producto si necesitan un folleto.

  En el campo que pregunta por los colores y los detalles de un nuevo logotipo, puede agregar una regla de lógica de visualización que muestre ese campo solo después de que el usuario seleccione el botón de opción Logotipo en el primer campo.

  Del mismo modo, en el campo que pregunta por las funciones del producto, puede agregar una regla de lógica de visualización que muestre ese campo solo después de que un usuario seleccione el botón de opción Folleto en el primer campo.

  ![](assets/display-logic-logo-request-350x196.png)

  Puede configurar reglas de lógica de visualización en cualquier campo, widget o salto de sección personalizado que siga a un campo de opción múltiple.

* **Regla de lógica de omisión**: esta regla se configura para ocultar partes de un formulario que el usuario no necesita. Cuando el usuario selecciona un elemento específico en un campo de opción múltiple anterior, la regla de lógica de omisión los omite al final del formulario o en un campo, widget o sección personalizados que desee que vean.

  **Ejemplo:** Alguien usa el formulario de solicitud de contenido de marketing anterior para solicitar un documento técnico, que proporciona Ventas, no Marketing. Para este usuario, una regla de lógica de omisión puede ocultar la pregunta y solicitar detalles y saltar a una línea de texto que le remite al departamento que necesita.

  ![](assets/skip-logic-white-paper-request-350x221.png)

  En este caso, puede agregar un campo de Texto descriptivo que haga referencia al usuario al departamento de ventas. En el primer campo personalizado que pregunta qué tipo de contenido de marketing necesita el usuario, puede agregar una regla de lógica de omisión que muestre solo la línea de texto cuando un usuario selecciona el botón de opción Libro blanco en el primer campo.

  Esto sería especialmente útil si agrega muchos otros campos acerca de logotipos, actualizaciones de sitios web y folletos que este usuario no necesita ver.
Puede aplicar una regla de lógica de omisión solo a un campo personalizado, no a un widget o a una sección.


## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>plan Adobe Workfront*</p> </td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Acceso administrativo a formularios personalizados</p> <p>Para obtener información acerca de cómo los administradores de Workfront conceden este acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">Conceder acceso administrativo a los usuarios a ciertas áreas</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;Para saber qué configuraciones de plan, tipo de licencia o nivel de acceso tiene, póngase en contacto con el administrador de Workfront.

## Crear un formulario personalizado de ejemplo con lógica de visualización y omisión

La mejor manera de aprender a agregar lógica de visualización y omisión a un formulario personalizado es a través del ejemplo práctico que se explica en las dos secciones siguientes:

* [Lógica de visualización: ejemplo práctico](#display-logic-practical-example)
* [Lógica de omisión: ejemplo práctico](#skip-logic-practical-example)

### Lógica de visualización: ejemplo práctico {#display-logic-practical-example}

En este ejemplo, creará un formulario personalizado con un campo de botón de opción de selección múltiple. A continuación, agregará la lógica de visualización que conecta este campo con un segundo campo.

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. En el panel izquierdo, seleccione **Forms personalizado** ![](assets/custom-forms-icon.png).

1. Haga clic en **Nuevo formulario personalizado**, seleccione **Proyecto** en el cuadro que se muestra y, a continuación, seleccione **Continuar**.

1. En el cuadro de texto **Título del formulario**, escriba **Formulario personalizado de ejemplo - Lógica de visualización de aprendizaje y omita la lógica** para asignar un nombre al formulario.

   ![](assets/form-title-box-350x247.png)

1. Para agregar el primer campo al formulario, haga lo siguiente:

   1. Abra la ficha **Agregar un campo**.

      ![](assets/add-a-field-tab-350x237.png)

   1. Seleccione el tipo de campo **Botones de radio** y, a continuación, escriba *¿Qué tipo de contenido de marketing necesita?* como **etiqueta** para el campo.

   1. En **Opciones**, reemplace **Opción 1** y **Opción 2** con el siguiente texto para crear dos opciones que los usuarios puedan elegir en el campo:

      *Actualización del sitio web*

      *Diseño de logotipo*

1. Para agregar el siguiente campo personalizado y agregarle una regla de lógica de visualización:

   1. Abra la ficha **Agregar un campo** de nuevo y agregue un nuevo campo de **Botones de opción** denominado *¿Qué tipo de actualización de sitio web necesita?*

      Añadiremos las opciones de este campo más adelante.

   1. En la sección **Configuración adicional**, seleccione **Agregar lógica**.

      ![](assets/add-logic-btn-350x408.png)

1. En el cuadro que aparece, con la ficha **Lógica de visualización** abierta, configure el segundo campo de modo que aparezca solamente para los usuarios que seleccionaron *Diseño de sitio web* en el primer campo:

   1. En el primer menú desplegable, seleccione **¿Qué tipo de contenido de marketing necesita?**
   1. En el segundo menú desplegable, seleccione **Diseño de sitio web**.
   1. Si deja el tercer menú desplegable establecido en **Seleccionado**, seleccione **Guardar**.

   Observe los pequeños cuadrados de color con una D, que indican que el segundo campo está conectado con la lógica de visualización a la selección del usuario en el primer campo:

   ![](assets/red-display-logic-indicators-350x250.png)

1. Seleccione **Vista previa** para asegurarse de que la lógica funciona como desea en el formulario y, a continuación, seleccione **Finalizar vista previa**.

1. Haga clic en **Guardar + Cerrar** para guardar el formulario y, a continuación, continúe con [Omitir lógica: ejemplo práctico](#skip-logic-practical-example) a continuación.

### Lógica de omisión: ejemplo práctico {#skip-logic-practical-example}

La lógica de omisión funciona de manera similar a la lógica de visualización, pero actúa como lo contrario: en lugar de hacer que se muestren campos de opción múltiple personalizados específicos basados en selecciones anteriores del usuario, usted determina cuáles deben ocultarse (omitirse) porque no son relevantes para el usuario.

Para obtener más información, siga trabajando en el formulario personalizado de ejemplo que creó en la sección [Lógica de visualización: ejemplo práctico](#display-logic-practical-example) de este artículo.

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Haga clic en **Forms personalizado**.
1. Haga clic en el nombre del formulario **Formulario personalizado de ejemplo: lógica de visualización de aprendizaje y lógica de omisión** que creó en los pasos anteriores para abrirlo y editarlo.
1. Seleccione el campo desplegable que creó denominado *¿Qué tipo de sitio web necesita?*, agregue las siguientes opciones al campo y haga clic en **Aplicar**:

   *Comercio electrónico*

   *Folleto*

   *Pertenencia*

1. Abra la ficha **Agregar un campo** y cree un campo **Texto con formato **campo denominado *¿Cuál es el objetivo del sitio web?* y luego haga clic en **Aplicar**.

   En esta organización, el equipo de redacción técnica crea un sitio de documentación de Ayuda, no el departamento de marketing. Por lo tanto, no se necesita más información de un usuario que selecciona la documentación de Ayuda en el segundo campo. Crearemos una línea de texto (un campo de texto descriptivo) que les dirá que vean al equipo de escritura técnica en su lugar. Y usaremos una regla de lógica de omisión que salta a ese usuario a esa línea de texto.

1. Para crear la línea de texto:

   1. Abra **Agregar un campo** y cree un **campo Texto descriptivo**.

   1. Para la **Etiqueta**, escriba *Consulte Equipo de escritura técnica*.

   1. Para el **texto descriptivo**, escriba *Consulte con el equipo de redacción técnica cómo crear documentación de ayuda en línea*.

   1. Seleccione **Aplicar**.

1. Para crear la regla de lógica de omisión:

   1. Seleccione el segundo campo desplegable, *¿Qué tipo de sitio web necesita?*
   1. En la sección **Ajustes adicionales** s, selecciona **Editar lógica**.
   1. En el cuadro que aparece, abra la ficha **Omitir lógica**.
   1. Establezca la primera lista desplegable en **Documentación de ayuda**, deje la segunda lista desplegable establecida en **Seleccionado** y establezca la tercera lista desplegable en **Consulte al equipo de redacción técnica**.
   1. Seleccione **Guardar**.

   Observe los pequeños cuadrados de lógica de omisión con una S, que indican que el usuario omitirá algo después de seleccionar una determinada opción en el segundo campo.

   ![](assets/notice-skip-logic-squares-350x249.png)

1. Haga clic en **Vista previa**  para asegurarse de que la lógica se aplica de la manera que desee.
1. Haga clic en **Guardar +Cerrar**.

Al crear un formulario como este, puede agregar más campos de texto para solicitar información a los usuarios que seleccionen Comercio electrónico o Folleto en el segundo campo. Estos campos pueden preguntar quién es la audiencia objetivo del sitio web, cuál es el objetivo para crearlo, cuál es el presupuesto, etc.

Y, con reglas lógicas, se podrían crear rutas de preguntas ramificadas.

Por ejemplo, para los usuarios que seleccionan Comercio electrónico, puede crear campos que hagan preguntas sobre fotos de productos, descripciones, precios y opciones de pago. Para los usuarios que seleccionan Folleto, puede crear campos que pregunten por el contenido.

Un usuario que seleccionara la documentación de Ayuda nunca vería ninguno de estos campos adicionales que son irrelevantes para él.

>[!TIP]
>
>Puede agregar lógica de visualización y lógica de omisión a un campo personalizado si se cumplen todas las condiciones siguientes en relación con el campo:
>
>* Es un campo de opción múltiple (botones de opción, listas desplegables o casillas de verificación)
>* Va precedido de un campo de opción múltiple
>* Va seguido de otro campo personalizado
>

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Multi-field display logic statements</h2>
-->

