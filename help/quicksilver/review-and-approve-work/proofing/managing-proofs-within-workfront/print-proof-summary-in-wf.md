---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Imprimir un resumen de prueba en Adobe Workfront
description: Puede imprimir un resumen de prueba, guardarlo como PDF o exportarlo como archivo XLS o archivo PDF optimizado para Adobe Reader.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: ac714bd5a5259d6f995ac445efbd0125e07022cb
workflow-type: tm+mt
source-wordcount: '670'
ht-degree: 91%

---

# Imprimir un resumen de prueba en Adobe Workfront

Puede imprimir un resumen de prueba, guardarlo como PDF o exportarlo como archivo XLS o archivo PDF optimizado para Adobe Reader.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">paquete de Adobe Workfront</td> 
   <td> <p>Cualquiera</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td> 
   <p>Estándar</p>
   <p>Trabajo o plan</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de prueba </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Acceso de edición a documentos</p> </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Imprimir un resumen de prueba o guardarlo como archivo PDF

Puede imprimir un resumen de prueba directamente desde la lista de documentos.

>[!NOTE]
>
>* No se admiten resúmenes de más de 1 GB.
>* No se pueden imprimir varios resúmenes de prueba al mismo tiempo desde la lista de documentos.

1. En la lista de documentos que contiene la prueba, pase el puntero por encima de la fila que contiene el documento y haga clic en **Resumen de impresión**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   O

   Mientras visualiza la prueba en el visor de pruebas, haga clic en el icono **Imprimir** icono ![Imprimir icono](assets/print-icon-in-pv.png) de la barra de herramientas izquierda. (Si la barra de herramientas izquierda no está visible, haga clic en el icono de menú ![Icono de menú](assets/menu-icon-in-pv.png) en la esquina superior izquierda del visor de revisiones).

1. Utilice cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mostrar</td> 
      <td> <p>Escriba lo que quiere imprimir:</p> 
       <ul> 
        <li>La <strong>Versión actual</strong> o <strong>Todas las versiones</strong> de la prueba</li> 
        <li>Solo las <strong>páginas con comentarios</strong> o <strong>Todas las páginas</strong></li> 
        <li>Solo las <strong>miniaturas de página</strong> (una pequeña representación de cada página) o <strong>Páginas completas</strong> (una representación completa de la prueba)<br></li> 
        <p>Nota: Para ver los números de pin en el marcado de la salida impresa, debe seleccionar Páginas completas, no Miniaturas de página. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ordenar comentarios por</td> 
      <td> <p>(Disponible solo si ha seleccionado Miniaturas de página arriba) Especifique el orden en el que desea que se impriman los comentarios de la prueba:</p> 
       <ul> 
        <li><strong>Más antiguo</strong>: desde el primer comentario hasta el último</li> 
        <li><strong>Más reciente</strong>: desde el último comentario realizado hasta el primero</li> 
        <li><strong>Página</strong>: por página, de la primera página a la última o de la última página a la primera</li> 
        <li><strong>Creador</strong>: por los nombres de los usuarios que los han añadido, de A-Z o de Z-A</li> 
       </ul> <p>Estas opciones no afectan a la salida que exporta como archivo XLS o de PDF.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filtrar comentarios por</td> 
      <td> <p>Puede utilizar cualquier combinación de estas opciones para incluir solo determinados comentarios en la salida que imprima o exporte como archivo XLS o PDF:</p> 
       <ul> 
        <li>Autores seleccionados (predeterminado)</li> 
        <li>Acciones seleccionadas</li> 
        <li>Estado <strong>Sin resolver</strong></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Flujo de trabajo</td> 
      <td> <p>(Disponible solo si la prueba tiene un flujo de trabajo automatizado) Puede hacer clic en <strong>Mostrar diagrama</strong> para incluir un diagrama en la salida impresa que muestre las fases de la prueba y las decisiones tomadas en cada fase. En el diagrama que aparece, los colores representan las decisiones tomadas en un escenario:</p> <p><strong>Verde</strong>: aprobado</p> <p><strong>Azul</strong>: pendiente de decisión</p> <p><strong>Rojo</strong>: cambios necesarios para la decisión</p> <p><strong>Gris</strong>: aún no se ha iniciado</p> <p><strong>Amarillo</strong>: documento aprobado con cambios</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Imprimir**.
1. En el panel derecho de la ventana que aparece, si desea imprimir el resumen, haga clic en el menú **Destino** y, a continuación, haga clic en **Ver más**. Haga clic en la impresora que desee utilizar en la lista que aparece y, a continuación, haga clic en **Imprimir**.

   O

   Si desea guardar el resumen como un archivo PDF, haga clic en el menú **Destino**, haga clic en **Guardar como PDF** y, a continuación, haga clic en **Guardar**.

## Exportar un resumen de revisión como XLS o PDF

Puede exportar un resumen de prueba para contenido estático como archivo XLS o como archivo PDF. Las exportaciones de prueba solo incluyen el contenido de la prueba.

1. En la lista de documentos que contiene la prueba, pase el puntero por encima de la fila que contiene el documento y haga clic en **Resumen de impresión**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Haga clic en el icono XLS o en el icono PDF situado cerca de la esquina superior derecha de la página.

   ![Icono de XLS PDF](assets/xls-pdf-icons-350x136.png)

Cuando el archivo exportado esté listo, recibirá un correo electrónico desde el que podrá descargar el archivo.

Si ha exportado el resumen como un archivo PDF, los comentarios sobre la prueba aparecerán en el lector de PDF. Si un comentario tiene varias marcas asociadas, el comentario aparecerá varias veces en la lista de comentarios (una vez por cada marca).
