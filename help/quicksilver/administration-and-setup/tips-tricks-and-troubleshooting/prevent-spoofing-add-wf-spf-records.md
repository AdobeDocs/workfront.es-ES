---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: Impedir la suplantación y agregar  [!DNL Adobe Workfront] registros SPF
description: Si los usuarios no reciben  [!DNL Adobe Workfront] notificaciones por correo electrónico, debe agregar [!DNL Workfront] registros SPF al firewall. Debe trabajar con su equipo de TI para añadir registros SPF.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: e93e3334-d72a-4f7b-9379-358f498c873b
source-git-commit: c389b4829f16bf82a5851a597f5dd358d9c96999
workflow-type: tm+mt
source-wordcount: '293'
ht-degree: 0%

---

# Evitar la suplantación de identidad y agregar [!DNL Adobe Workfront] registros SPF

## Problema

Si los usuarios no reciben [!DNL Adobe Workfront] notificaciones por correo electrónico, debe agregar [!DNL Workfront] registros SPF al firewall. Debe trabajar con su equipo de TI para añadir registros SPF.

## Requisitos de acceso

Debe tener el siguiente acceso para realizar los pasos de este artículo:

+++ Expanda para ver los requisitos de acceso para la funcionalidad en este artículo.

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
   <td>
   <p>Nuevo: estándar</p>
   <p>o</p>
   <p>Actual: plan</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Configuraciones de nivel de acceso</td> 
   <td>Debe ser administrador de [!DNL Workfront]. </td> 
  </tr> 
 </tbody> 
</table>

Para obtener más información sobre esta tabla, consulte [Requisitos de acceso en la documentación de Workfront](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Solución

Si ya agregó las direcciones IP a su lista de permitidos para su entorno de producción como se describe en [Configuración de la lista de permitidos del firewall](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md) y los usuarios siguen sin recibir correos electrónicos:

1. Añada el siguiente registro SPF al cortafuegos:

   *spf.workfront.com*

   Esto agrega automáticamente todas las direcciones IP de [!DNL Workfront] a la lista de permitidos en el firewall y permite que todos los filtros de correo no deseado (que usan registros SPF) validen los servidores de [!DNL Workfront] como remitentes válidos para su dominio.

   >[!NOTE]
   >
   > Un registro SPF es un registro TXT que forma parte de un archivo de zona DNS. No admitimos la modificación del archivo de zona DNS.

1. Debe especificar qué tipo de registro SPF se debe configurar. Estos son los tipos válidos de registros SPF:

   * todo (https://dmarcian.com/spf-syntax-table/#all)
   * ip4 (https://dmarcian.com/spf-syntax-table/#ip4)
   * ip6 (https://dmarcian.com/spf-syntax-table/#ip6)
   * a (https://dmarcian.com/spf-syntax-table/#a)
   * mx (https://dmarcian.com/spf-syntax-table/#mx)
   * ptr (https://dmarcian.com/spf-syntax-table/#ptr)
   * existe (https://dmarcian.com/spf-syntax-table/#exists)
   * include (https://dmarcian.com/spf-syntax-table/#include)

   Por ejemplo, &quot;v=spf1 a mx include: spf.workfront.com -all&quot;

Si no puede agregar registros SPF al firewall debido a la directiva de la compañía, comuníquese con el representante de soporte técnico de [!DNL Workfront].
