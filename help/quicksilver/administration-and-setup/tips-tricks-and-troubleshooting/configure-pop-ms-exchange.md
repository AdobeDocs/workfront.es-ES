---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;setup
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Configurar POP en Microsoft Exchange
description: Una cuenta de correo electrónico POP en [!DNL Microsoft Exchange] está desactivado.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 4f7b6f40-cfbd-4f02-8c3e-de26b05db13b
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Configurar POP en [!DNL Microsoft Exchange]

## Problema

Una cuenta de correo electrónico POP en [!DNL Microsoft Exchange] está desactivado.

## Solución

Antes de pasar tiempo solucionando el problema, asegúrese de que la cuenta POP del usuario esté configurada correctamente. Si sigue teniendo problemas después de confirmar que la cuenta POP está configurada correctamente, póngase en contacto con [!DNL Microsoft] Asistencia o a uno de sus socios para obtener ayuda adicional.

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
   <td> <p>Debe ser [!DNL Workfront] administrador. Para obtener más información, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Conceder a un usuario acceso administrativo completo</a>.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte a su [!DNL Workfront] administrador si establecen restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo se [!DNL Workfront] administrador puede modificar el nivel de acceso, consulte <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Configurar POP en [!DNL Microsoft Exchange]

>[!NOTE]
>
>Los siguientes pasos pueden utilizarse como guía general para configurar POP en [!DNL Microsoft Exchange] para una producción [!DNL Workfront] sistema. Los pasos pueden variar significativamente según la versión de Exchange o los cambios de código realizados por Microsoft.

1. Inicie y habilite el servicio POP3 en el servidor Exchange 2010.

   >[!NOTE]
   >
   >De forma predeterminada, el servicio POP3 no está iniciado.

   1. Inicio [!DNL Microsoft]Administrador del servidor de .
   1. Navegar: **[!UICONTROL Administrador del servidor]** > **[!UICONTROL Configuración]** >**[!UICONTROL Firewall de Windows con seguridad avanzada]** > **[!UICONTROL Servicios]**.

   1. Clic con el botón derecho **[!DNL Microsoft Exchange]POP3** y haga clic en **[!UICONTROL Propiedades]**.

   1. (Condicional) Para garantizar que el servicio POP se inicie automáticamente, en la variable **[!UICONTROL General]** , establezca la variable **[!UICONTROL Inicio]** escriba a [!UICONTROL Automático].

1. Configure POP3 para el servidor.

   1. Inicie el [!DNL Microsoft Exchange] Consola de administración.
   1. Navegar: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuración del servidor]** > **[!UICONTROL Acceso de cliente]**.

   1. Choose **[!UICONTROL POP3]**.

      POP3 está en la lista bajo la [!UICONTROL POP3] y [!UICONTROL IMAP4] pestañas.

   1. En el lado derecho, debajo de **[!UICONTROL Acciones]**, seleccione **[!UICONTROL POP3]** y, a continuación, elija **[!UICONTROL Propiedades]**.

   1. Haga clic en **[!UICONTROL Propiedades POP3]** y, a continuación, abra el **[!UICONTROL Enlace]** pestaña .

      Se muestran todas las direcciones IP disponibles y los números de puerto configurados para el servidor POP3. El cuadro superior muestra el cuadro Sin encriptar y el cuadro inferior muestra la IP y los puertos para las conexiones SSL/TLS.

   1. Haga clic en **[!UICONTROL Propiedades POP3]** y, a continuación, abra el **[!UICONTROL Autenticación]** pestaña .

   1. **[!UICONTROL Seleccionar seguro]** inicio de sesión.

      Se requiere una conexión TLS para que el cliente se autentique en el servidor.

1. Habilitar o permitir que los usuarios se conecten a POP.

   1. Inicie el [!DNL Microsoft Exchange] Consola de administración.
   1. Navegar: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuración de destinatario]** > **[!UICONTROL Buzón]**.

      Se muestra una lista de buzones o usuarios.

   1. Resalte el correo electrónico que se utiliza en [!DNL Workfront].
   1. En el lado derecho, debajo de **[!UICONTROL Acciones]**, seleccione **[!UICONTROL Propiedades]** y, a continuación, abra el **[!UICONTROL Funciones de buzón]** pestaña .

   1. (Condicional) Si POP3 está deshabilitado, haga clic en **[!UICONTROL POP3]** y haga clic en **[!UICONTROL Habilitar]**.

      Se muestra una lista de buzones o usuarios.

1. Configure los conectores de recepción.

   1. Inicio [!DNL Microsoft Exchange] Consola de administración.
   1. Navegar: [!DNL Microsoft] **[!UICONTROL Exchange On-Premise]** > **[!UICONTROL Configuración del servidor]** > **[!UICONTROL Transporte de concentradores]**.

      Se muestra una lista de conectores de recepción.

   1. Confirmar el conector de recepción *Cliente* *EX01* está activada.

      Donde *Cliente* *EX01* es el nombre de su servidor Exchange.

   1. Select *Cliente EX01*, luego a la derecha debajo de **[!UICONTROL Acciones]**, seleccione **[!UICONTROL Propiedades]**.

   1. Abra el **[!UICONTROL Autenticación]** y, a continuación, asegúrese **[!UICONTROL Seguridad de capa de transporte (TLS)]** está activada.

      >[!NOTE]
      >
      >Para tener autenticación básica, es posible que tenga que iniciar TLS y autenticación integrada de Windows.
