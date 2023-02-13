---
user-type: administrator
content-type: overview
product-area: system-administration;user-management
navigation-topic: start-with-workfront-administration
title: Resumen del cortafuegos
description: Como Adobe Workfront se comunica con la red de su organización, el cortafuegos de su organización debe estar configurado para permitir esa comunicación. Los cortafuegos son medidas de seguridad muy eficaces que funcionan al separar la red de una organización de Internet. Garantizan que solo los datos seleccionados y el tráfico de red puedan entrar o salir de la red de la organización. El cortafuegos permite o bloquea los datos en función del sitio que envía o recibe los datos. Como administrador de Adobe Workfront, debe asegurarse de que los datos enviados a Workfront o desde puedan pasar a través del cortafuegos de su organización.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 172999e7-fb05-49a6-ad57-84b59e80a28e
source-git-commit: d0ab54670d1767e2fa2a9cdf2e7eda1ce8940c7f
workflow-type: tm+mt
source-wordcount: '753'
ht-degree: 0%

---

# Resumen del cortafuegos

Como Adobe Workfront se comunica con la red de su organización, el cortafuegos de su organización debe estar configurado para permitir esa comunicación. Los cortafuegos son medidas de seguridad muy eficaces que funcionan al separar la red de una organización de Internet. Garantizan que solo los datos seleccionados y el tráfico de red puedan entrar o salir de la red de la organización. El cortafuegos permite o bloquea los datos en función del sitio que envía o recibe los datos. Como administrador de Adobe Workfront, debe asegurarse de que los datos enviados a Workfront o desde puedan pasar a través del cortafuegos de su organización.

Esto se logra mediante una lista de permitidos, que es esencialmente una &quot;lista&quot; de sitios &quot;permitidos&quot; para enviar o recibir datos a través del cortafuegos. Los sitios se pueden identificar de una de las dos maneras siguientes:

* **Dirección IP**: una serie de números como 52.31.132.175
* **Dominio**: parte de una URL, como &quot;este dominio&quot; en www.thisdomain.com

Workfront utiliza direcciones IP y dominios específicos para la comunicación web. Deben agregarse a la lista de permitidos de su organización para poder utilizar Workfront en su organización.

Generalmente, un administrador de red configura una lista de permitidos. Póngase en contacto con el administrador de red de su organización para asegurarse de que el cortafuegos permita estas direcciones IP. Si no sabe quién es el administrador de red, el departamento de TI de su organización puede indicarle la dirección correcta.

>[!IMPORTANT]
>
>Como administrador de Workfront, debe asegurarse de que estas direcciones IP y dominios se añadan a la lista de permitidos de su organización. Esto es cierto incluso si no los agrega usted mismo. Workfront no puede configurar la lista de permitidos de su organización.

## Recopilar información para configurar el cortafuegos

Para configurar el firewall para Workfront, el administrador de la red debe saber qué direcciones IP y dominios agregar. Parte de esta información solo está disponible para administradores de Workfront. Como administrador de Workfront, debe localizar esta información y proporcionarla al administrador de red.

>[!NOTE]
>
>La práctica recomendada para la seguridad es añadir solo las direcciones IP y los dominios que se conectan a la funcionalidad que utiliza activamente su organización. Al proporcionar esta información, puede asegurarse de que se sigue esta práctica recomendada.

Proporcione a su administrador de red la siguiente información:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Direcciones IP y dominios específicos que permiten</td> 
   <td> <p>El artículo <a href="../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md" class="MCXref xref">Configurar la lista de permitidos del cortafuegos</a> contiene la lista de direcciones IP y dominios que su organización debe agregar a su lista de permitidos. </p> <p>Es posible que el administrador de red no tenga acceso al artículo "Configurar el cortafuegos". En ese caso, debe proporcionárselos. No se recomienda imprimir una copia impresa (en papel). Una copia digital permite al administrador de la red copiar y pegar las direcciones, lo que es más rápido y preciso que escribir desde una copia impresa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Su clúster</td> 
   <td>Para localizar el clúster de su organización, consulte <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Ver el clúster de su organización y el plan de Workfront</a></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Su plan de Workfront</td> 
   <td> <p>El plan de su organización es uno de los siguientes:</p> 
    <ul> 
     <li> <p>Empresa </p> </li> 
     <li> <p>Comercial </p> </li> 
     <li> <p>Pro </p> </li> 
     <li> <p>Equipo </p> </li> 
    </ul> <p>Para localizar su plan, consulte <a href="#view-your-organization-s-cluster-and-workfront-plan" class="MCXref xref">Vea el clúster de su organización y el plan de Workfront.</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Su dominio</td> 
   <td> <p>Para localizar su dominio, consulte la dirección web que utiliza para conectarse a Workfront.</p> <p>Ejemplo: en la dirección web <code>greatcompany.my.workfront.com</code>, el dominio es "big company"</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Otros productos de Adobe Workfront</td> 
   <td> <p>Informe al administrador de red si dispone de licencias para cualquiera de las siguientes opciones:</p> 
    <ul> 
     <li> <p>Prueba de Adobe Workfront</p> </li> 
     <li> <p>Adobe Workfront Fusion </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Integraciones de Adobe Workfront</td> 
   <td>Informe al administrador de red si utiliza cualquiera de las siguientes opciones:
    <ul>
     <li><p><p>Workfront para Jira</p></p></li>
     <li><p>Workfront para G Suite</p></li>
     <li><p>Workfront para Microsofts Teams</p></li>
     <li><p>Workfront para Outlook</p></li>
     <li><p>Workfront para Salesforce</p></li>
    </ul></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Funcionalidad adicional</td> 
   <td> <p>Informe al administrador de red si utiliza cualquiera de las siguientes opciones:</p> 
    <ul> 
     <li> <p>Una unidad de prueba de Workfront</p> </li> 
     <li> <p>Workfront Ascent</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

>[!IMPORTANT]
>
>Si agrega cualquiera de estos productos, integraciones o funcionalidades más adelante, debe ponerse en contacto con el administrador de la red para que pueda ajustar la lista de permitidos.

### Ver el clúster de su organización y el plan de Workfront {#view-your-organization-s-cluster-and-workfront-plan}

1. Haga clic en el **Menú principal** icono ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront, haga clic en **Configuración** ![](assets/gear-icon-settings.png).

1. Haga clic en **Sistema** en el panel izquierdo
1. Para ver el clúster, seleccione **Información del cliente**.

   El clúster se muestra cerca de la esquina superior derecha del **Información básica** para obtener más información.

   ![](assets/locate-cluster.png)

1. Para ver su plan de Workfront, seleccione **Licencias**.

   El plan se muestra cerca de la parte inferior de la página.

   ![](assets/locate-plan.png)
