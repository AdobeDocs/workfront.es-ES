---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Imprimir un resumen de prueba en Adobe Workfront
description: Puede imprimir un resumen de prueba, guardarlo como PDF o exportarlo como archivo XLS o archivo de PDF optimizado para Adobe Reader.
author: Courtney
feature: Digital Content and Documents
exl-id: 129c8e6b-5c66-445b-a5d0-7b1460aeabd6
source-git-commit: 918d51e3b832a3104777346cebd54a4830e2d826
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 1%

---

# Imprimir un resumen de prueba en Adobe Workfront

Puede imprimir un resumen de prueba, guardarlo como PDF o exportarlo como archivo XLS o archivo de PDF optimizado para Adobe Reader.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o Superior</p> <p>o</p> <p>Plan heredado: Select o Premium</p> <p>Para obtener más información sobre cómo revisar el acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o Plan</p> <p>Plan heredado: Cualquiera (debe tener la revisión habilitada para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Responsable o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si sigue sin tener acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para saber qué plan, función o perfil de permiso de revisión tiene, póngase en contacto con su administrador de Workfront o de Workfront Proof.

+++

## Imprimir un resumen de prueba o guardarlo como archivo de PDF

Puede imprimir un resumen de prueba directamente desde la lista de documentos.

>[!NOTE]
>
>* No se admiten resúmenes de más de 1 GB.
>* No se pueden imprimir varios resúmenes de prueba al mismo tiempo desde la lista de documentos.

1. En la lista de documentos que contiene la prueba, pase el ratón sobre la fila que contiene el documento y haga clic en **Imprimir resumen**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

   O

   Mientras visualiza la prueba en el visor de pruebas, haga clic en el icono **Imprimir** en la barra de herramientas izquierda. ![](assets/print-icon-in-pv.png) (Si la barra de herramientas izquierda no está visible, haga clic en el icono Menú ![](assets/menu-icon-in-pv.png) en la esquina superior izquierda del visor de revisión).

1. Utilice cualquiera de las siguientes opciones:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Mostrar</td> 
      <td> <p>Especifique lo que desea imprimir:</p> 
       <ul> 
        <li><strong>Versión actual</strong> o <strong>Todas las versiones</strong> de la revisión</li> 
        <li>Solo las <strong>páginas con comentarios</strong> o <strong>todas las páginas</strong></li> 
        <li>Solo las <strong>miniaturas de página</strong> (una pequeña representación de cada página) o <strong>páginas completas</strong> (una representación completa de la prueba)<br></li> 
        <p>Nota: Para ver los números de pin en el marcado de la salida impresa, debe seleccionar Páginas completas, no Miniaturas de página. </p> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Ordenar comentarios por</td> 
      <td> <p>(Disponible solo si ha seleccionado Miniaturas de página arriba) Especifique el orden en que desea que se impriman los comentarios de la prueba:</p> 
       <ul> 
        <li><strong>Más antiguo</strong>: Desde el primer comentario hasta el último</li> 
        <li><strong>Más reciente</strong>: Desde el último comentario hecho hasta el primero</li> 
        <li><strong>Página</strong>: Por página, de la primera página a la última o de la última página a la primera</li> 
        <li><strong>Creador</strong>: por los nombres de los usuarios que los agregaron, de A-Z o de Z-A</li> 
       </ul> <p>Estas opciones no afectan a la salida que exporta como archivo XLS o de PDF.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Filtrar comentarios por</td> 
      <td> <p>Puede utilizar cualquier combinación de estas opciones para incluir sólo determinados comentarios en la salida que imprima o exporte como archivo XLS o de PDF:</p> 
       <ul> 
        <li>Autores que seleccione (predeterminado)</li> 
        <li>Acciones seleccionadas</li> 
        <li><strong>Estado sin resolver</strong></li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Flujo de trabajo</td> 
      <td> <p>(Disponible solo si la prueba tiene un flujo de trabajo automatizado) Puede hacer clic en <strong>Mostrar diagrama</strong> para incluir un diagrama en la salida impresa que muestre las fases de la prueba y las decisiones tomadas en cada fase. En el diagrama que aparece, los colores representan las decisiones tomadas en un escenario:</p> <p><strong>Verde</strong>: aprobado</p> <p><strong>Azul</strong>: pendiente de decisión</p> <p><strong>Rojo</strong>: cambios necesarios para la decisión</p> <p><strong>Gris</strong>: aún no se inició</p> <p><strong>Amarillo</strong>: aprobado con cambios</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Haga clic en **Imprimir**.
1. En el panel derecho de la ventana que aparece, si desea imprimir el resumen, haga clic en el menú **Destino** y, a continuación, haga clic en **Ver más**. Haga clic en la impresora que desee usar en la lista que aparece y, a continuación, haga clic en **Imprimir**.

   O

   Si desea guardar el resumen como un archivo de PDF, haga clic en el menú **Destino**, haga clic en **Guardar como PDF** y, a continuación, haga clic en **Guardar**.

## Exportar un resumen de revisión como XLS o PDF

Puede exportar un resumen de prueba para contenido estático como archivo XLS o como archivo de PDF. Las exportaciones de prueba solo incluyen el contenido de la prueba.

1. En la lista de documentos que contiene la prueba, pase el ratón sobre la fila que contiene el documento y haga clic en **Imprimir resumen**.

   ![proof_printsummary.png](assets/proof-printsummary-350x166.png)

1. Haga clic en el icono XLS o en el PDF situado cerca de la esquina superior derecha de la página.

   ![](assets/xls-pdf-icons-350x136.png)

Cuando el archivo exportado esté listo, recibirá un correo electrónico desde el que podrá descargar el archivo.

Si ha exportado el resumen como un archivo de PDF, los comentarios sobre la prueba aparecerán en el PDF. Si un comentario tiene varias marcas asociadas, el comentario aparecerá varias veces en la lista de comentarios (una vez por cada marca).
