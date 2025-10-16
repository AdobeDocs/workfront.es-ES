---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configurar POP en Microsoft Exchange
description: Se deshabilitó una cuenta de correo electrónico POP en  [!DNL Microsoft Exchange] .
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: 929502c256011b464d938ad1095c127407e4a795
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 99%

---

# Configurar POP en [!DNL Microsoft Exchange]

## Problema

Se deshabilitó una cuenta de correo electrónico POP en [!DNL Microsoft Exchange].

## Solución

Antes de dedicar tiempo a solucionar el problema, asegúrese de que la cuenta POP del usuario esté configurada correctamente. Si sigue teniendo problemas después de confirmar que la cuenta POP está configurada correctamente, póngase en contacto con la asistencia técnica de [!DNL Microsoft] o con uno de sus socios para obtener ayuda adicional.

## Requisitos de acceso

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!DNL Adobe Workfront] paquete</td> 
   <td><p>Cualquiera</p></td> 
  </tr> 
  <tr> 
   <td>[!DNL Adobe Workfront] licencia</td> 
   <td><p>Estándar</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Configuraciones de nivel de acceso</td> 
   <td>[!UICONTROL System Administrator]</td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Configurar POP en [!DNL Microsoft Exchange]

>[!NOTE]
>
>Los siguientes pasos pueden utilizarse como guía general para configurar POP en [!DNL Microsoft Exchange] para un sistema de producción [!DNL Workfront]. Los pasos pueden variar significativamente según la versión de Exchange o los cambios de código realizados por Microsoft.

1. Inicie y habilite el servicio POP3 en el servidor de Exchange 2010.

   >[!NOTE]
   >
   >De forma predeterminada, el servicio POP3 no se inicia.

   1. Inicie el Administrador del servidor de [!DNL Microsoft].
   1. Vaya a: **[!UICONTROL Administrador de servidores]** > **[!UICONTROL Configuración]** >**[!UICONTROL Cortafuegos de Windows con seguridad avanzada]** > **[!UICONTROL Servicios]**.

   1. Haga clic con el botón secundario en **[!DNL Microsoft Exchange]POP3** y, a continuación, haga clic en **[!UICONTROL Propiedades]**.

   1. (Condicional) Para asegurarse de que el servicio POP se inicie automáticamente, en la pestaña **[!UICONTROL General]**, establezca el tipo **[!UICONTROL Inicio]** en [!UICONTROL Automático].

1. Configure POP3 para el servidor.

   1. Inicie la consola de administración de [!DNL Microsoft Exchange].
   1. Vaya a: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuración del servidor]** > **[!UICONTROL Acceso de cliente]**.

   1. Elija **[!UICONTROL POP3]**.

      POP3 está en la lista bajo las pestañas [!UICONTROL POP3] y [!UICONTROL IMAP4].

   1. En el lado derecho, debajo de **[!UICONTROL Acciones]**, seleccione **[!UICONTROL POP3]** y, a continuación, elija **[!UICONTROL Propiedades]**.

   1. Haga clic en **[!UICONTROL Propiedades POP3]** y, a continuación, abra la pestaña **[!UICONTROL Enlace]**.

      Se mostrarán todas las direcciones IP y números de puerto disponibles configurados para el servidor POP3. El cuadro superior muestra Sin cifrar y el cuadro inferior muestra la IP y los puertos para las conexiones SSL/TLS.

   1. Haga clic en **[!UICONTROL Propiedades POP3]** y, a continuación, abra la pestaña **[!UICONTROL Autenticación]**.

   1. **[!UICONTROL Seleccionar inicio de sesión seguro en]**.

      Se requiere una conexión TLS para que el cliente se autentique en el servidor.

1. Habilitar o permitir a los usuarios conectarse a POP.

   1. Inicie la consola de administración de [!DNL Microsoft Exchange].
   1. Vaya a: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuración del destinatario]** > **[!UICONTROL Buzón]**.

      Se muestra una lista de buzones o usuarios.

   1. Seleccione el correo electrónico que se está usando en [!DNL Workfront].
   1. A la derecha, debajo de **[!UICONTROL Acciones]**, seleccione **[!UICONTROL Propiedades]** y, a continuación, abra la pestaña **[!UICONTROL Características del buzón]**.

   1. (Condicional) Si POP3 está deshabilitado, haga clic en **[!UICONTROL POP3]** y, a continuación, en **[!UICONTROL Habilitar]**.

      Se muestra una lista de buzones o usuarios.

1. Configure los conectores de recepción.

   1. Inicie la consola de administración de [!DNL Microsoft Exchange] 
   1. Vaya a: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuración del servidor]** > **[!UICONTROL Concentrador de transporte]**.

      Se muestra una lista de conectores de recepción.

   1. Compruebe que el conector de recepción *Client* *EX01* esté habilitado.

      Donde *Client* *EX01* es el nombre de su servidor de Exchange.

   1. Seleccione *Cliente EX01* y, a continuación, a la derecha, debajo de **[!UICONTROL Acciones]**, seleccione **[!UICONTROL Propiedades]**.

   1. Abra la pestaña **[!UICONTROL Autenticación]** y asegúrese de que la opción **[!UICONTROL Seguridad de la capa de transporte (TLS)]** esté marcada.

      >[!NOTE]
      >
      >Para poder tener Autenticación Básica, es posible que necesites iniciar TLS y Autenticación Integrada de Windows.
