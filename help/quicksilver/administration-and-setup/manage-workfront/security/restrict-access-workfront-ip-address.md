---
user-type: administrator
product-area: system-administration
navigation-topic: security
title: Restringir el acceso a Adobe Workfront por dirección IP
description: Puede configurar una lista de permitidos IP de Adobe Workfront que limite el acceso a Workfront a 45 direcciones IP o rangos de direcciones IP que especifique. Esto proporciona un nivel adicional de seguridad para la aplicación de Workfront.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: aed65b42-d534-453a-885d-f922114987bc
source-git-commit: 7bd3d2252b124a07a112aaa2b7798063087e7cab
workflow-type: tm+mt
source-wordcount: '451'
ht-degree: 1%

---

# Restringir el acceso a Adobe Workfront por dirección IP

Puede configurar una lista de permitidos IP de Adobe Workfront que limite el acceso a Workfront a 45 direcciones IP o rangos de direcciones IP que especifique. Esto proporciona un nivel adicional de seguridad para la aplicación de Workfront.

El administrador de red debe proporcionar estas direcciones IP o intervalos de direcciones IP.

## Requisitos de acceso

Debe tener lo siguiente para realizar los pasos de este artículo:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">plan de Adobe Workfront</td> 
   <td> <p>Empresa</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Licencia de Adobe Workfront</td> 
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td> <p>Debe ser administrador de Workfront.</p> <p><b>NOTA</b>: Si todavía no tiene acceso, pregunte al administrador de Workfront si ha establecido restricciones adicionales en su nivel de acceso. Para obtener información sobre cómo un administrador de Workfront puede modificar su nivel de acceso, vea <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Crear o modificar niveles de acceso personalizados</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Otras listas de permitidos

Si el cortafuegos o el servidor de correo están configurados para permitir el acceso solo a determinados proveedores, debe añadir determinadas direcciones IP a su lista de permitidos. Esto abre la comunicación entre su entorno y los servidores de Adobe Workfront. Para obtener información al respecto, consulte [Configuración de la lista de permitidos del firewall](../../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

Además, si su organización utiliza el plan empresarial, puede configurar la lista de permitidos de correo electrónico de Workfront para controlar qué dominios de correo electrónico pueden aceptar correos electrónicos de Workfront y qué dominios de correo electrónico pueden estar en la dirección de correo electrónico que los usuarios especifican en su perfil de usuario de Workfront. Para obtener más información, consulte [Configuración de la lista de permitidos por correo electrónico](../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md).

## Añadir direcciones IP a la lista de permitidos

Después de agregar direcciones IP a la lista de permitidos de Workfront, solo se podrán usar esas direcciones IP para acceder a Workfront. Los usuarios que intenten acceder a Workfront desde otra dirección IP recibirán un mensaje de error que indica que su dirección IP está bloqueada.

1. Haga clic en el icono **Menú principal** ![](assets/main-menu-icon.png) en la esquina superior derecha de Adobe Workfront y, a continuación, haga clic en **Configurar** ![](assets/gear-icon-settings.png).

1. Haga clic en **Sistema** > **Información del cliente.**

1. En la sección **lista de permitidos IP**, seleccione **Habilitar lista de permitidos IP.**

   Esta opción está desactivada de forma predeterminada.

1. Especifique la dirección IP que está utilizando actualmente para acceder al sistema de Workfront.

   O

   Especifique un rango de direcciones IP que incluya la que está utilizando actualmente para acceder al sistema de Workfront.

   La dirección IP que utiliza para acceder a Workfront debe añadirse a la lista de permitidos antes de activar la lista de permitidos.

1. Haga clic en **Agregar intervalo de IP** y, a continuación, especifique la dirección IP o el intervalo de direcciones IP que desea que tengan acceso a Workfront.
1. (Opcional) Repita el paso anterior para agregar direcciones IP o intervalos de direcciones IP adicionales.

   Se pueden agregar hasta 45 direcciones o intervalos.

1. Haga clic en **Guardar.**
