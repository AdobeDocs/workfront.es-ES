---
product-area: projects
navigation-topic: use-the-home-area
title: Uso del widget Mis solicitudes
description: Puede enviar solicitudes en el widget Mis solicitudes. También puede personalizar el widget con filtros y columnas.
author: Alina, Courtney
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 3893a57fb7ae31a1649b20beccc1f0b79f2421fb
workflow-type: tm+mt
source-wordcount: '1118'
ht-degree: 11%

---

# Uso del widget Mis solicitudes

>[!IMPORTANT]
>
>Este artículo describe el nuevo widget Mis solicitudes. Debe tener la nueva experiencia de solicitud habilitada para ver el nuevo widget.
>Puede activar la nueva experiencia de solicitud en el área Solicitudes.

El widget Mis solicitudes muestra las solicitudes que ha enviado. Puede filtrar las solicitudes, buscar solicitudes específicas o ajustar el orden de columnas y la visibilidad. También puede crear una nueva solicitud desde el widget Mis solicitudes.

>[!NOTE]
>
>* Cuando se carga el widget Mis solicitudes, se muestran hasta 50 solicitudes. Para mostrar más solicitudes, desplácese hacia abajo por la lista.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront package]</strong></td> 
   <td> <p>Cualquier paquete de Workfront o Workflow</p>
   <p>Cualquier paquete de Workfront Planning para acceder a las solicitudes de Workfront Planning y sus objetos creados</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia</strong></td> 
   <td> <p>Colaborador o superior</p>
   <p>Solicitud o superior</p> </td> 
  </tr> 
  <tr> 
   <!--
   <tr> 
   <td role="rowheader"><strong>Additional products</strong></td> 
   <td> You must have Adobe Workfront Planning to view Planning requests or request forms</td> 
   </tr> 
   -->
   <td role="rowheader"><strong>Configuración de nivel de acceso</strong></td> 
   <td> <p>Acceso de visualización o superior a cualquier objeto para el que esté etiquetado en una conversación o necesite resolver una aprobación (proyectos, tareas, problemas, documentos)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Permisos de [!UICONTROL View] o superiores para proyectos, tareas, problemas o documentos en los que esté etiquetado en una conversación o necesite resolver una aprobación</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Crear una solicitud

Puede crear una solicitud directamente desde el widget Mis solicitudes.

Para obtener instrucciones, vea la sección [Crear una solicitud](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md/#create-a-request) en el artículo [Crear elementos de trabajo y proyectos desde el área de inicio](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md).

## Copiar una solicitud

Puede copiar una solicitud en el widget Mis solicitudes, editarla y enviarla como una solicitud nueva.

Para obtener instrucciones, vea [Copiar y enviar solicitudes](/help/quicksilver/manage-work/requests/create-requests/copy-and-submit-requests.md).

## Filtrar solicitudes

El widget Mis solicitudes presenta un filtro personalizable que le permite controlar qué solicitudes aparecen en el widget. Puede configurar este filtro para diferentes campos y valores, y puede apilar condiciones mediante los operadores AND y OR.

Para configurar el filtro en el widget Mis solicitudes:

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono de menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Para agregar el widget **Mis solicitudes** a la pantalla de inicio. Haga clic en **Personalizar**, busque **Mis solicitudes** y, a continuación, haga clic en él para agregarlo a la **página principal**.
1. En el widget **Mis solicitudes**, haga clic en **Filtro**.
1. Seleccione el campo por el que desea filtrar. Entre las opciones disponibles se encuentran:

   * Espacio de trabajo
   * Tipo de objeto
   * Fecha de entrada
   * Formulario de solicitud
   * Estado
   * Introducido por
   * Campos personalizados de la solicitud o del objeto creado

1. En el campo siguiente, seleccione el operador que desee utilizar para esta condición de filtro. Los operadores disponibles dependen del campo elegido.
1. (Condicional) Si un campo aparece a la derecha del operador, seleccione el valor por el que desea filtrar.
1. (Opcional) Para agregar otra condición de filtro, haga clic en **Agregar condición** y repita los pasos 4-6.
1. (Opcional y condicional) Si tiene varias condiciones, cambie el valor AND u OR haciendo clic en **And** o **Or** a la izquierda de la condición.

El filtro se guarda automáticamente.

>[!TIP]
>
>Si su organización ha adquirido Workfront Planning además de Adobe Workfront, el widget Mis solicitudes incluirá las solicitudes de Workfront y Workfront Planning.
> 
>* Para filtrar solo por solicitudes de Workfront, establezca el filtro en **Tipo de objeto** > **Tiene alguno de** > **Problemas**.
>* Para filtrar solo las solicitudes de Workfront Planning, establezca el filtro en **Tipo de objeto** > **No tiene ninguno de** > **Problemas**.

## Ajuste o adición de columnas

Puede elegir cuál de las columnas disponibles aparece en el widget Mis solicitudes y establecer su orden.

Las columnas disponibles incluyen:

* Asunto
* Objeto creado
* Tipo de objeto
* Estado
* Formulario de solicitud
* Fecha de entrada
* Introducido por

Para ajustar las columnas en el widget Mis solicitudes:

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Para agregar el widget **Mis solicitudes** a la pantalla de inicio. Haz clic en **Personalizar**, busca **Mis solicitudes** y luego haz clic en él para agregarlo a **Inicio**.
1. En el widget **Mis solicitudes**, haga clic en **Columnas**.
1. (Opcional) Para reordenar las columnas, haga clic en el controlador de arrastre ![controlador de arrastre](assets/drag-handle.png) de la columna que desee mover y arrástrelo a las ubicaciones que desee. La columna situada en la parte superior de la lista aparece en el widget Mis solicitudes como primera columna.
1. (Opcional) Utilice el botón de alternancia para ocultar o mostrar la columna en la lista de solicitudes.
1. Para agregar un campo personalizado como columna, haga clic en el icono **Agregar columna** ![Agregar columna](assets/add-column.png) situado en la esquina superior derecha de la lista, y haga clic en el icono más situado junto al campo personalizado que desea agregar como columna al widget.

   Los campos personalizados de los formularios adjuntos al objeto en la lista están disponibles para agregarse como columnas.

Las preferencias de columna se guardan automáticamente.

## Crear una vista

Puede crear vistas en el widget Mis solicitudes para cambiar la forma en que se muestra la información en la lista de solicitudes.

Tenga en cuenta lo siguiente al trabajar con vistas en el widget Mis solicitudes:

* Una vista del widget Mis solicitudes contiene las columnas y filtros aplicados a la vista.
* Puede crear vistas y compartirlas con otros usuarios. Los filtros y las columnas que seleccione para la vista antes de compartirla se incluyen en las vistas que comparta.
* La siguiente es una vista de sistema que no se puede editar, compartir ni eliminar:

   * Widget Unified Requests Vista predeterminada
* Crear y editar una vista en el widget Mis solicitudes es similar a las listas mejoradas. Para obtener más información, consulte [Usar listas mejoradas](/help/quicksilver/workfront-basics/navigate-workfront/use-lists/enhanced-lists.md).

## Solicitudes de búsqueda

Para buscar solicitudes específicas en el widget Mis solicitudes:

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Para agregar el widget **Mis solicitudes** a la pantalla de inicio. Haz clic en **Personalizar**, busca **Mis solicitudes** y luego haz clic en él para agregarlo a **Inicio**.
1. En la barra de búsqueda cerca de la parte superior derecha del widget Mis solicitudes, introduzca el término que desea buscar.

   Las solicitudes que contienen el término se resaltan en naranja.

1. (Opcional) Para saltar a las solicitudes resaltadas, haga clic en las flechas arriba o abajo en la barra de búsqueda.

## Ir a un objeto creado por una solicitud

Puede encontrar objetos creados por una solicitud en el widget Mis solicitudes.

>[!NOTE]
>
>Los vínculos a objetos creados están disponibles en la nueva experiencia de solicitud sólo para solicitudes de Planning, en los casos en los que la propia solicitud creó un objeto. Si una solicitud de Workfront se convierte en un proyecto u otro objeto, un vínculo a ese objeto convertido no estará disponible en la lista de solicitudes de la nueva experiencia de solicitud.

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono de menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Para agregar el widget **Mis solicitudes** a la pantalla de inicio. Haga clic en **Personalizar**, busque **Mis solicitudes** y, a continuación, haga clic en él para agregarlo a la **página principal**.
1. Busque la solicitud que creó el objeto.
1. Haga clic en el nombre del objeto en la columna **Objeto creado** para esa solicitud.

   Se abre la página del objeto.

