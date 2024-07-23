---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Crear o editar un flujo de trabajo automatizado para una revisión existente
description: Los flujos de trabajo automatizados facilitan la administración del proceso de revisión si el proceso es complejo o si envía contenido regularmente para su revisión a los mismos grupos de personas. Cuando se crea una prueba con un flujo de trabajo automatizado, esta se desplaza de una fase a otra hasta la aprobación final. Se notifica a los participantes cuando les toca revisar el documento.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: f252e3562b8ea73486d407138251b3d15d4b9f3a
workflow-type: tm+mt
source-wordcount: '1236'
ht-degree: 1%

---

# Crear o editar un flujo de trabajo automatizado para una revisión existente

Los flujos de trabajo automatizados facilitan la administración del proceso de revisión si el proceso es complejo o si envía contenido regularmente para su revisión a los mismos grupos de personas. Cuando se crea una prueba con un flujo de trabajo automatizado, esta se desplaza de una fase a otra hasta la aprobación final. Se notifica a los participantes cuando les toca revisar el documento.

Para obtener información sobre cómo crear un flujo de trabajo automatizado para una nueva prueba, consulte [Crear una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o Superior</p> <p>o</p> <p>Plan heredado: Premium</p> <p>Para obtener más información sobre cómo revisar el acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de revisión en Workfront</a>.</p> </td> 
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

## Cree o edite un flujo de trabajo automatizado para una revisión existente:

1. Pase el ratón sobre el documento en el área Documentos y haga clic en Flujo de trabajo de revisión.

   O

   Si está revisando la prueba en el visor de revisión, haga clic en **Flujo de trabajo** ![](assets/workflow-icon-proofing-viewer.png) en el panel izquierdo y, a continuación, haga clic en el icono Editar ![](assets/edit-icon-proofing-viewer.png) para abrir la configuración del Flujo de trabajo automatizado para la prueba.

1. (Condicional) Si la revisión está usando un flujo de trabajo básico (sin fases), haga clic en **Convertir en flujo de trabajo automatizado** en la pantalla que aparece.

   >[!NOTE]
   >
   >No puede editar la primera fase al convertir un flujo de trabajo básico en un flujo de trabajo automatizado, pero puede añadir y configurar nuevas fases.

1. Condicional) Para usar una plantilla de flujo de trabajo automatizado que el administrador de Adobe Workfront haya creado y compartido con usted, haga clic en **Agregar plantilla**, selecciónela en el cuadro que aparece y, a continuación, haga clic en **Agregar plantilla**.

   Para obtener más información, consulte [Acerca del uso de plantillas de flujo de trabajo automatizadas](#about-using-automated-workflow-templates) en este artículo.

1. Añada una fase al flujo de trabajo automatizado:

   1. Haga clic en **Nuevo escenario** cerca de la esquina superior derecha.
   1. En el cuadro que aparece, escriba un **Nombre** para el escenario.
   1. (Opcional) Establezca una fecha límite para la etapa.
   1. En la sección **Activar fase**, elija cómo desea que se active la fase:


      <table>
      <tbody>
      <tr>
      <td><strong>Al crear la prueba</strong></td>
      <td>La fase se activa automáticamente porque ya se ha creado la prueba.</td>
      </tr>
      <tr>
      <td><strong>Cuando haya pasado la fecha límite de la fase anterior</strong></td>
      <td>Haga clic en la etapa anterior en la lista desplegable <strong>Fase principal</strong></td>
      </tr>
      <tr>
      <td><strong>En una fecha y hora específicas</strong></td>
      <td>Haga clic en el cuadro <strong>El</strong> para seleccionar la fecha y, a continuación, haga clic en el cuadro situado a la derecha para seleccionar la hora.</td>
      </tr>
      <tr>
      <td><strong>Todas las decisiones se aprueban o aprueban con cambios en la fase principal</strong></td>
      <td>Haga clic en la fase principal en la lista desplegable <strong>Fase principal</strong>.</td>
      </tr>
      <tr>
      <td><strong>Todas las decisiones se aprueban en la fase principal</strong></td>
      <td>Haga clic en la fase principal en la lista desplegable <strong>Fase principal</strong>.</td>
      </tr>
      <tr>
      <td><strong>Todas las decisiones se toman</strong></td>
      <td>Haga clic en la fase principal en la lista desplegable <strong>Fase principal</strong>.</td>
      </tr>
      </tbody>
      </table>


   1. Introduzca un nombre de contacto o una dirección de correo electrónico y configure las opciones de los revisores de la fase.

      Para obtener información acerca de cómo agregar revisores, vea [Agregar revisores a una fase](#about-adding-reviewers-to-a-stage) en este artículo.

   1. Utilice cualquiera de las siguientes opciones para configurar aún más la fase:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>Opciones de fecha límite</strong> </td>
         <td><p>Para establecer una fecha límite para la fase, haga clic en una opción de la lista desplegable <strong>Opciones de fecha límite</strong>. A continuación, en <strong>Plazo</strong>, realice una de las siguientes acciones:</p>
          <ul>
           <li>Si elige <strong>Establecer fecha específica</strong>: seleccione la fecha y la hora límite que desee.</li>
           <li>Si elige <strong>Calcular a partir de la fecha de activación de la fase</strong>: seleccione el número de días laborables que desee agregar a la fecha de activación de la fase para determinar la fecha límite.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Bloquear fase</td>
         <td>Especifique cuándo se puede bloquear el escenario. </td>
        </tr>
        <tr>
         <td role="rowheader">Responsable de toma de decisiones principal</td>
         <td><p>Seleccione el responsable de la toma de decisiones principal en la fase (disponible solo después de añadir al menos una persona a la fase que tenga la función de Aprobador o superior en Prueba). Si selecciona un responsable de la toma de decisiones principal, la opción <strong>Solo se requiere una decisión</strong> se deshabilita en este escenario.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Solamente se requiere una decisión</td>
         <td>Finaliza todo el proceso de revisión cuando uno de los responsables de la toma de decisiones toma una decisión.<p>Esta opción no está disponible si ha designado un usuario en el menú desplegable <strong>Responsable principal de la toma de decisiones</strong>.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Fase privada</td>
         <td>Permite que solo las siguientes personas vean los comentarios y las decisiones tomadas durante esta fase: supervisores, administradores de Adobe Workfront y administradores de Workfront Proof</td>
        </tr>
        <tr>
         <td role="rowheader">Notificar a las personas por correo electrónico</td>
         <td>Avisa a los revisores con una notificación por correo electrónico cuando les toca trabajar en la prueba.</td>
        </tr>
       </tbody>
      </table>

   1. Haga clic en **Agregar fase**.

1. Repita el paso anterior según sea necesario para agregar más etapas.

   A medida que se añaden fases al flujo de trabajo automatizado, se forma un diagrama en la pantalla para representarlas:

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. Cuando termine de agregar etapas, haga clic en **Listo**.

## Acerca del uso de plantillas de flujo de trabajo automatizado {#about-using-automated-workflow-templates}

Tenga en cuenta lo siguiente cuando utilice una plantilla de flujo de trabajo automatizado:

1. La configuración de una plantilla de Flujo de trabajo automatizado determina lo que puede hacer con el Flujo de trabajo automatizado para una prueba. Por ejemplo, si el botón Add a stage está desactivado en la plantilla, no está visible mientras trabaja con la configuración del flujo de trabajo automatizado para la prueba.
1. Cuando se añade una persona a una etapa en una plantilla de flujo de trabajo automatizado, pero también está presente como revisor en la prueba, al aplicar la plantilla se elimina al revisor de la etapa. Si no agrega otro revisor al escenario, aparecerá un mensaje en el que se le pedirá que agregue uno.
1. La posibilidad de modificar una plantilla de flujo de trabajo automatizado depende de la configuración de la plantilla que establezca el administrador de Workfront, tal como se describe en Si la capacidad para modificar la plantilla está desactivada, solo el propietario de la plantilla puede modificarla.

## Agregar revisores a una fase {#about-adding-reviewers-to-a-stage}

Tenga en cuenta lo siguiente al agregar revisores a una fase:

* Después de agregar un usuario a una fase, puede configurar las opciones de ese usuario en la prueba, como la función de prueba y los permisos adicionales que debe tener y el tipo de alertas de correo electrónico que recibirá cuando las personas realicen comentarios y decisiones sobre la prueba.
* Puede arrastrar a uno o varios usuarios de una fase a otra. Puede arrastrar a los usuarios directamente a otra fase o arrastrarlos a una fase del diagrama **Fases**. Para seleccionar varios usuarios, presione Mayús+Ctrl (en Windows) o Mayús+Comando (en Mac).
* Puede agregar un revisor a una prueba solo una vez, lo que significa que no puede agregar la misma persona a más de un paso de la prueba.
* Los revisores que no se agregan a una fase privada no pueden ver esa fase en la prueba ni en los comentarios realizados en esa fase.
* De forma predeterminada, añadir un usuario a una fase concede a ese usuario acceso para ver la prueba desde el momento en que se crea la prueba.

  El administrador de Workfront puede restringir el acceso de los usuarios a la prueba hasta que el flujo de trabajo entre en la fase en la que se añadió el usuario. Para obtener más información, consulte  en .
