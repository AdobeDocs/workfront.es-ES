---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configuración de POP en Microsoft Exchange
description: Se deshabilitó una cuenta de correo electrónico POP en  [!DNL Microsoft Exchange] .
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '473'
ht-degree: 0%

---

# Configurar POP en [!DNL Microsoft Exchange]

## Problema

Se deshabilitó una cuenta de correo electrónico POP en [!DNL Microsoft Exchange].

## Solución

Antes de dedicar tiempo a solucionar el problema, asegúrese de que la cuenta POP del usuario está configurada correctamente. Si sigue teniendo problemas después de confirmar que la cuenta POP está configurada correctamente, póngase en contacto con el soporte técnico de [!DNL Microsoft] o con uno de sus socios para obtener ayuda adicional.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For instructions on integrating a POP account in Adobe Workfront, see .</p>
-->

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Cualquiera</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licencia</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de [!DNL Workfront]. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder acceso administrativo completo a un usuario</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de [!DNL Workfront] si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de [!DNL Workfront] puede modificar su nivel de acceso, vea <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar POP en [!DNL Microsoft Exchange]

>[!NOTE]
>
>Los siguientes pasos pueden utilizarse como guía general para configurar POP en [!DNL Microsoft Exchange] para un sistema de producción [!DNL Workfront]. Los pasos pueden variar significativamente según la versión de Exchange o los cambios de código realizados por Microsoft.

1. Inicie y habilite el servicio POP3 en el servidor de Exchange 2010.

   >[!NOTE]
   >
   >De forma predeterminada, el servicio POP3 no está iniciado.

   1. Inicie el Administrador del servidor de [!DNL Microsoft].
   1. Vaya: **[!UICONTROL Administrador de servidores]** > **[!UICONTROL Configuración]** >**[!UICONTROL Firewall de Windows con seguridad avanzada]** > **[!UICONTROL Servicios]**.

   1. Haga clic con el botón secundario en **[!DNL Microsoft Exchange]POP3** y, a continuación, haga clic en **[!UICONTROL Propiedades]**.

   1. (Condicional) Para asegurarse de que el servicio POP se inicia automáticamente, en la ficha **[!UICONTROL General]**, establezca el tipo **[!UICONTROL Inicio]** en [!UICONTROL Automático].

1. Configure POP3 para el servidor.

   1. Inicie la consola de administración de [!DNL Microsoft Exchange].
   1. Vaya: [!DNL Microsoft] **[!UICONTROL Exchange local]** > **[!UICONTROL Configuración del servidor]** > **[!UICONTROL Acceso de cliente]**.

   1. Elija **[!UICONTROL POP3]**.

      POP3 está en la lista bajo las fichas [!UICONTROL POP3] y [!UICONTROL IMAP4].

   1. En el lado derecho debajo de **[!UICONTROL Acciones]**, seleccione **[!UICONTROL POP3]** y, a continuación, elija **[!UICONTROL Propiedades]**.

   1. Haga clic en **[!UICONTROL Propiedades POP3]** y, a continuación, abra la ficha **[!UICONTROL Enlace]**.

      Se mostrarán todas las direcciones IP y números de puerto disponibles configurados para el servidor POP3. El cuadro superior muestra Sin cifrar y el cuadro inferior muestra la IP y los puertos para las conexiones SSL/TLS.

   1. Haga clic en **[!UICONTROL Propiedades POP3]** y, a continuación, abra la ficha **[!UICONTROL Autenticación]**.

   1. **[!UICONTROL Seleccionar inicio de sesión seguro]**.

      Se requiere una conexión TLS para que el cliente se autentique en el servidor.

1. Habilitar o permitir a los usuarios conectarse a POP.

   1. Inicie la consola de administración de [!DNL Microsoft Exchange].
   1. Navegar: [!DNL Microsoft] **[!UICONTROL Exchange local]** > **[!UICONTROL Configuración de destinatario]** > **[!UICONTROL Buzón]**.

      Se muestra una lista de buzones o usuarios.

   1. Resaltar el correo electrónico que se está usando en [!DNL Workfront].
   1. A la derecha, debajo de **[!UICONTROL Acciones]**, seleccione **[!UICONTROL Propiedades]** y, a continuación, abra la ficha **[!UICONTROL Características del buzón]**.

   1. (Condicional) Si POP3 está deshabilitado, haga clic en **[!UICONTROL POP3]** y, a continuación, en **[!UICONTROL Habilitar]**.

      Se muestra una lista de buzones o usuarios.

1. Configure los conectores de recepción.

   1. Iniciar [!DNL Microsoft Exchange] consola de administración.
   1. Vaya: [!DNL Microsoft] **[!UICONTROL Exchange local]** > **[!UICONTROL Configuración del servidor]** > **[!UICONTROL Transporte de concentradores]**.

      Se muestra una lista de conectores de recepción.

   1. Confirme que el conector de recepción *Client* *EX01* está habilitado.

      Donde *Cliente* *EX01* es el nombre de su servidor de Exchange.

   1. Seleccione *Cliente EX01* y, a continuación, a la derecha debajo de **[!UICONTROL Acciones]**, seleccione **[!UICONTROL Propiedades]**.

   1. Abra la ficha **[!UICONTROL Autenticación]** y asegúrese de que **[!UICONTROL Seguridad de la capa de transporte (TLS)]** esté marcada.

      >[!NOTE]
      >
      >Para tener la autenticación básica, es posible que tenga que iniciar TLS y la autenticación de Windows integrada.
