---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: Crear o editar un flujo de trabajo automatizado para una prueba existente
description: Los flujos de trabajo automatizados facilitan la administración del proceso de revisión si el proceso es complejo o si envía contenido para su revisión con regularidad a los mismos grupos de personas. Cuando crea una prueba con un flujo de trabajo automatizado, la prueba pasa de una fase a otra hasta la aprobación final. A los participantes se les notifica cuando les toca revisar el documento.
author: Courtney
feature: Digital Content and Documents
exl-id: 852f960f-1b57-4a8a-a928-407ad52418e6
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '1225'
ht-degree: 1%

---

# Crear o editar un flujo de trabajo automatizado para una prueba existente

Los flujos de trabajo automatizados facilitan la administración del proceso de revisión si el proceso es complejo o si envía contenido para su revisión con regularidad a los mismos grupos de personas. Cuando crea una prueba con un flujo de trabajo automatizado, la prueba pasa de una fase a otra hasta la aprobación final. A los participantes se les notifica cuando les toca revisar el documento.

Para obtener información sobre la creación de un flujo de trabajo automatizado para una prueba nueva, consulte [Creación de una prueba avanzada con un flujo de trabajo automatizado](../../../review-and-approve-work/proofing/creating-proofs-within-workfront/create-automated-proof-workflow.md).

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront*</td> 
   <td> <p>Plan actual: Pro o superior</p> <p>o</p> <p>Plan heredado: Premium</p> <p>Para obtener más información sobre la prueba de acceso con los diferentes planes, consulte <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Acceso a la funcionalidad de pruebas en Workfront</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront*</td> 
   <td> <p>Plan actual: Trabajo o plan</p> <p>Plan heredado: Cualquiera (debe tener las pruebas habilitadas para el usuario)</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Perfil de permiso de revisión </td> 
   <td>Administrador o superior</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso*</td> 
   <td> <p>Editar acceso a documentos</p> <p>Nota: Si todavía no tiene acceso, pregunte a su administrador de Workfront si establece restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, consulte <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Para averiguar qué plan, función o perfil de permiso de prueba tiene, póngase en contacto con el administrador de Workfront o Workfront Proof.

## Cree o edite un flujo de trabajo automatizado para una prueba existente:

1. Pase el ratón sobre el documento en el área Documentos y haga clic en Flujo de trabajo de prueba.

   O

   Si está revisando la prueba en el visor de pruebas, haga clic en **Flujo de trabajo** ![](assets/workflow-icon-proofing-viewer.png) en el panel izquierdo y, a continuación, haga clic en el icono Editar ![](assets/edit-icon-proofing-viewer.png) para abrir la configuración Flujo de trabajo automatizado de la prueba.

1. (Condicional) Si la prueba está utilizando actualmente un flujo de trabajo básico (sin etapas), haga clic en **Convertir en flujo de trabajo automatizado** en la pantalla que aparece.

   >[!NOTE]
   >
   >No se puede editar la primera etapa cuando se convierte de un flujo de trabajo básico a un flujo de trabajo automatizado, pero se pueden añadir y configurar nuevas etapas.

1. Condicional) Para usar una plantilla de flujo de trabajo automatizado que el administrador de Adobe Workfront haya creado y compartido con usted, haga clic en **Agregar plantilla**, seleccione la plantilla en el cuadro que aparece y haga clic en **Agregar plantilla**.

   Para obtener más información, consulte [Acerca del uso de plantillas de flujo de trabajo automatizadas](#about-using-automated-workflow-templates) en este artículo.

1. Agregue un escenario al flujo de trabajo automatizado:

   1. Haga clic en **Nueva etapa** cerca de la esquina superior derecha.
   1. En el cuadro que aparece, escriba un **Nombre** para el escenario.
   1. (Opcional) Establezca una fecha límite para la etapa.
   1. En el **Activar etapa** , elija cómo desea que se active el escenario:


      <table>
      <tbody>
      <tr>
      <td><strong>Creación de pruebas</strong></td>
      <td>El escenario se activa automáticamente porque la prueba ya se ha creado.</td>
      </tr>
      <tr>
      <td><strong>Cuando haya pasado la fecha límite de la fase anterior</strong></td>
      <td>Haga clic en el paso anterior de la <strong>Fase principal</strong> lista desplegable .</td>
      </tr>
      <tr>
      <td><strong>En una fecha y hora específicas</strong></td>
      <td>Haga clic en el <strong>Activado</strong> para seleccionar la fecha y, a continuación, haga clic en el cuadro de la derecha para seleccionar la hora.</td>
      </tr>
      <tr>
      <td><strong>Todas las decisiones son aprobadas o aprobadas con cambios en la fase principal</strong></td>
      <td>Haga clic en el paso principal del <strong>Fase principal</strong> lista desplegable.</td>
      </tr>
      <tr>
      <td><strong>Todas las decisiones se aprueban en la fase principal</strong></td>
      <td>Haga clic en el paso principal del <strong>Fase principal</strong> lista desplegable.</td>
      </tr>
      <tr>
      <td><strong>Todas las decisiones se toman</strong></td>
      <td>Haga clic en el paso principal del <strong>Fase principal</strong> lista desplegable.</td>
      </tr>
      </tbody>
      </table>


   1. Introduzca un nombre de contacto o una dirección de correo electrónico y configure los ajustes de los revisores del escenario.

      Para obtener información sobre cómo agregar revisores, consulte [Acerca de la adición de revisores a un escenario](#about-adding-reviewers-to-a-stage) en este artículo.

   1. Utilice cualquiera de las siguientes opciones para configurar aún más el escenario:

      <table style="table-layout:auto">
       <col>
       <col>
       <tbody>
        <tr>
         <td role="rowheader"><strong>Opciones de fecha límite</strong> </td>
         <td><p>Para establecer una fecha límite para el escenario, haga clic en una opción del <strong>Opciones de fecha límite</strong> lista desplegable. A continuación, debajo de <strong>Fecha límite</strong>, realice una de las siguientes acciones:</p>
          <ul>
           <li>Si elige <strong>Establecer fecha específica</strong>: Seleccione la fecha y la hora límite que desee.</li>
           <li>Si elige <strong>Calcular a partir de la fecha de activación del escenario</strong>: Seleccione el número de días hábiles que desea agregar a la fecha de activación de la etapa para determinar la fecha límite.</li>
          </ul></td>
        </tr>
        <tr>
         <td role="rowheader">Bloqueo del escenario</td>
         <td>Especifique cuándo se puede bloquear el escenario. </td>
        </tr>
        <tr>
         <td role="rowheader">Responsable de toma de decisiones principal</td>
         <td><p>Seleccione el responsable de decisión primario en el escenario (disponible solo después de agregar al menos una persona a la fase que tenga una función de prueba de Aprobador o superior). Si selecciona un responsable de decisión principal, la variable <strong>Solo se requiere una decisión</strong> está desactivada en esta etapa.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Solamente se requiere una decisión</td>
         <td>Finaliza todo el proceso de revisión cuando uno de los responsables de la toma de decisiones toma una decisión.<p>Esta opción no está disponible si ha designado un usuario en la variable <strong>Creador de decisiones principal</strong> menú desplegable.</p></td>
        </tr>
        <tr>
         <td role="rowheader">Fase privada</td>
         <td>Permite que solo las siguientes personas vean los comentarios y decisiones realizados durante esta fase: Supervisores, administradores de Adobe Workfront y administradores de Workfront Proof</td>
        </tr>
        <tr>
         <td role="rowheader">Notificar a las personas por correo electrónico</td>
         <td>Alerta a los revisores con una notificación por correo electrónico cuando les toca trabajar en la prueba.</td>
        </tr>
       </tbody>
      </table>

   1. Haga clic en **Agregar etapa**.

1. Repita el paso anterior según sea necesario para agregar más etapas.

   A medida que se añaden etapas al flujo de trabajo automatizado, aparece un diagrama en la pantalla para representarlas:

   ![](assets/workflow-diagram-existing-proof-qs-350x215.png)

1. Cuando haya terminado de añadir etapas, haga clic en **Listo**.

## Acerca del uso de plantillas de flujo de trabajo automatizadas {#about-using-automated-workflow-templates}

Tenga en cuenta lo siguiente cuando utilice una plantilla Flujo de trabajo automatizado :

1. La configuración de una plantilla Flujo de trabajo automatizado determina lo que puede hacer con el Flujo de trabajo automatizado para una prueba. Por ejemplo, si el botón Add a stage está desactivado en la plantilla, no está visible ya que se trabaja con la configuración de flujo de trabajo automatizado para la prueba.
1. Cuando se añade una persona a un mensaje en una plantilla Flujo de trabajo automatizado , pero también ya está presente como revisor en la prueba, al aplicar la plantilla, se elimina al revisor de la fase. Si no agrega otro revisor a la fase, un mensaje le pedirá que añada uno.
1. La capacidad de modificar una plantilla de flujo de trabajo automatizado depende de la configuración de la plantilla del administrador de Workfront, tal como se describe en . Si la capacidad de modificar la plantilla está deshabilitada, solo el propietario de la plantilla puede modificarla.

## Acerca de la adición de revisores a un escenario {#about-adding-reviewers-to-a-stage}

Tenga en cuenta lo siguiente al agregar revisores a una etapa:

* Después de agregar un usuario a una etapa, puede configurar las opciones de ese usuario en la prueba, como la función de prueba y los permisos adicionales que deben tener y el tipo de alertas de correo electrónico que recibirán cuando las personas realicen comentarios y decisiones sobre la prueba.
* Puede arrastrar uno o varios usuarios de un escenario a otro. Puede arrastrar a los usuarios directamente a otro paso o a un escenario en el **Etapas** diagrama. Para seleccionar varios usuarios, pulse Mayús+Ctrl (en Windows) o Mayús+Comando (en Mac).
* Puede agregar un revisor a una prueba solo una vez, lo que significa que no puede agregar la misma persona a más de un paso de la prueba.
* Los revisores que no se agregan a un escenario privado no pueden ver ese escenario en la prueba o los comentarios realizados en ese escenario.
* De forma predeterminada, agregar un usuario a una etapa concede a ese usuario acceso para ver la prueba desde el momento en que se crea la prueba.

   El administrador de Workfront puede restringir el acceso de los usuarios a la prueba hasta que el flujo de trabajo entre en la fase en la que se agregó el usuario. Para obtener más información, consulte en .
