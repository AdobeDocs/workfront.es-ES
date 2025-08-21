---
product-area: projects
navigation-topic: use-the-home-area
title: Uso del widget Mis solicitudes
description: Puede enviar solicitudes en el widget Mis solicitudes. También puede personalizar el widget con filtros y columnas.
author: Becky
feature: Get Started with Workfront
exl-id: 2b994f44-2404-4aa3-8c38-0686a0c287b7
source-git-commit: 2fe55f61bd24ebb3ecfe09fff29c4aad2ca33608
workflow-type: tm+mt
source-wordcount: '825'
ht-degree: 17%

---

# Uso del widget Mis solicitudes

<span class="preview">La información de esta página hace referencia a una funcionalidad que aún no está disponible de forma general. Solo está disponible en el entorno de vista previa para todos los clientes. Después de las versiones mensuales en Production, las mismas funciones también están disponibles en el entorno Production para los clientes que habilitaron versiones rápidas. </span>

<span class="preview">Para obtener información sobre las versiones rápidas, consulte [Habilitar o deshabilitar las versiones rápidas para su organización](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md).

>[!IMPORTANT]
>
>Este artículo describe el nuevo widget Mis solicitudes. Debe tener la nueva experiencia de solicitud habilitada para ver el nuevo widget.
>>Puede activar la nueva experiencia de solicitud en el área de solicitudes.

El widget Mis solicitudes muestra las solicitudes que se han enviado a su organización. Puede filtrar las solicitudes, buscar solicitudes específicas o ajustar el orden y la visibilidad de las columnas. También puede crear una nueva solicitud desde el widget Mis solicitudes.

>[!NOTE]
>
>* Cuando se carga el widget Mis solicitudes, muestra hasta 50 solicitudes. Para mostrar más solicitudes, desplácese hacia abajo por la lista.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Product]</strong></td> 
   <td> <ul><li>Adobe Workfront</li><li>Debe tener Adobe Workfront Planning para ver solicitudes de Planning o formularios de solicitud</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan]</strong></td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licencia*</strong></td> 
   <td> <p>Nuevo: colaborador o superior</p>
   O   
   <p>Actual: [!UICONTROL Request] o superior</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Configuración de nivel de acceso</strong></td> 
   <td> <p>Ver el acceso o superior a cualquier objeto para el que esté etiquetado en una conversación o para el que necesite resolver una aprobación (proyectos, tareas, problemas, documentos)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Permisos de objeto</strong></td> 
   <td> <p>Permisos de [!UICONTROL View] o superiores para proyectos, tareas, problemas o documentos en los que esté etiquetado en una conversación o necesite resolver una aprobación</p> </td> 
  </tr> 
 </tbody> 
</table>

*Para saber qué plan, tipo de licencia o acceso tiene, póngase en contacto con el administrador de [!DNL Workfront]. Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Creación de una solicitud

Puede crear una solicitud directamente desde el widget Mis solicitudes.

Para obtener instrucciones, vea [Crear una solicitud](/help/quicksilver/workfront-basics/using-home/using-the-home-area/create-work-items-in-home.md#create-a-request) en el artículo Crear elementos de trabajo y proyectos desde el área de Inicio.

## Filtrar solicitudes

El widget Mis solicitudes incluye un filtro personalizable que le permite controlar qué solicitudes aparecen en el widget. Puede configurar este filtro para diferentes campos y valores, así como apilar condiciones mediante AND y OR.

Para configurar el filtro en el widget Mis solicitudes:

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Para agregar el widget **Mis solicitudes** a la pantalla de inicio. Haga clic en **Personalizar** y busque **Mis solicitudes**.
1. En el widget Mis solicitudes, haga clic en **Filtro**.
1. En el campo situado más a la izquierda, seleccione por qué desea filtrar. Entre las opciones disponibles se encuentran:

   * Espacio de trabajo
   * Tipo de objeto
   * Fecha de entrada
   * Formulario de solicitud
   * Estado
   * Introducido por

1. En el campo siguiente, seleccione el operador que desee utilizar para esta condición de filtro. Los operadores disponibles dependen del campo elegido.
1. (Condicional) Si un campo aparece a la derecha del operador, seleccione el valor por el que desea filtrar.
1. (Opcional) Para agregar otra condición de filtro, haga clic en **Agregar condición** y repita los pasos 4-6.
1. (Opcional y condicional) Si tiene varias condiciones, cambie el valor AND u OR haciendo clic en **And** o **Or** a la izquierda de la condición.

El filtro se guarda automáticamente.

>[!TIP]
>
>Si su organización ha adquirido Workfront Planning, el widget Mis solicitudes incluirá las solicitudes de Workfront y Workfront Planning.
> 
>* Para filtrar solo las solicitudes Workfront, establezca el filtro en **Tipo de objeto** > **Tiene cualquiera de** > **Problemas**.
>* Para filtrar solo las solicitudes de Workfront Planning, establezca el filtro en **Tipo de objeto** > **No tiene ninguno de** > **Problemas**.

## Ajustar columnas

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
1. (Condicional) Para agregar el widget **Mis solicitudes** a la pantalla de inicio. Haga clic en **Personalizar** y busque **Mis solicitudes**.
1. En el widget Mis solicitudes, haga clic en **Columnas**.
1. (Opcional) Para reordenar las columnas, haga clic en el controlador de arrastre ![controlador de arrastre](assets/drag-handle.png) de la columna que desee mover y arrástrela a las ubicaciones que desee. La columna situada en la parte superior de la lista aparece en el widget Mis solicitudes como la columna situada más a la izquierda.
1. (Opcional) Utilice el conmutador para controlar si se muestra una columna en el widget Mis solicitudes.

Las preferencias de columna se guardan automáticamente.

## Solicitudes de búsqueda

Para buscar solicitudes específicas en el widget Mis solicitudes:

1. Haga clic en el **[!UICONTROL Menú principal]** ![icono del menú principal](assets/main-menu-icon.png) en la esquina superior derecha y, a continuación, haga clic en **[!UICONTROL Inicio]**.
1. (Condicional) Para agregar el widget **Mis solicitudes** a la pantalla de inicio. Haga clic en **Personalizar** y busque **Mis solicitudes**.
1. En la barra de búsqueda cerca de la parte superior derecha del widget Mis solicitudes, introduzca el término que desea buscar.

   Las solicitudes que contienen el término se resaltan en naranja.

1. (Opcional) Para saltar a las solicitudes resaltadas, haga clic en las flechas arriba o abajo de la barra de búsqueda.
