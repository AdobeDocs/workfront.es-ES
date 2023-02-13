---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: get-started-with-workfront-fusion-2-0
title: Términos básicos en Adobe Workfront Fusion
description: Adobe Workfront Fusion requiere una licencia de Adobe Workfront Fusion además de una licencia de Adobe Workfront.
author: Becky
feature: Workfront Fusion
exl-id: 2169dc2e-2135-47e0-a615-3de12cd120a9
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 0%

---

# Términos básicos en [!DNL Adobe Workfront Fusion]

>[!NOTE]
>
>[!DNL Adobe Workfront Fusion] requiere un [!DNL Adobe Workfront Fusion] además de una [!UICONTROL Adobe Workfront] licencia.


<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Acción</p> </td> 
   <td>Módulo que permite leer o escribir paquetes desde o en una aplicación o servicio seleccionados.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Aggregator]</p> </td> 
   <td> <p>Tipo de módulo que combina varios paquetes (varias matrices de datos) en un único paquete. Para obtener más información, consulte <a href="../../workfront-fusion/modules/aggregator-module.md" class="MCXref xref">Módulo [!UICONTROL Aggregator] en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Clave API</td> 
   <td>Código único que identifica al usuario, desarrollador o programa que llama a la API de un software y que se utiliza para la autenticación. Since [!DNL Adobe Workfront Fusion] Los módulos funcionan conectando API, las claves de API a veces son necesarias. Las claves de API se distribuyen mediante la aplicación que las requiere. Por ejemplo, si necesita una clave de API para [!DNL ActiveCampaign], lo solicitaría a través de su [!DNL ActiveCampaign] cuenta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Aplicación o servicio</td> 
   <td> <p>Una aplicación de software, normalmente.</p> <p>Una aplicación también puede ser una función especial que manipula datos, como un iterador o un agregador. </p> <p>Un servicio es una fuente de paquetes que pueden incluir una API web, una página web, diferentes tipos de servidores (FTP, SMTP, IMAP), etc. </p> <p> <img src="assets/apps-350x420.jpg" style="width: 350;height: 420;"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Conector de la aplicación</td> 
   <td>Aplicación que se conecta a otro sistema.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Paquete</p> </td> 
   <td> <p>Un paquete es una unidad básica que los módulos devuelven o reciben. Un paquete consta de elementos.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Al añadir una aplicación o servicio a un escenario, lo más probable es que primero tenga que crear una conexión entre [!DNL Workfront Fusion] y la aplicación o servicio para recuperar o enviar los datos seleccionados. Para obtener más información, consulte <a href="../../workfront-fusion/connections/about-connecting-wf-fusion-to-app-or-service.md" class="MCXref xref">Acerca de la conexión [!DNL Adobe Workfront Fusion] a una aplicación o servicio</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Ciclo</p> </td> 
   <td> <p>Un ciclo hace referencia a dos fases de la ejecución del escenario: operación y confirmación. El escenario puede consistir en uno o más ciclos. Para obtener información más detallada, consulte <a href="../../workfront-fusion/scenarios/scenario-execution-cycles-phases.md" class="MCXref xref">Ejecución del escenario, ciclos y fases en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Almacén de datos</p> </td> 
   <td> <p>Herramienta que almacena datos de escenarios o que permite transferir datos entre escenarios o situaciones individuales. Para obtener más información, consulte <a href="../../workfront-fusion/modules/data-stores.md" class="MCXref xref">Almacenes de datos en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transferencia de datos</p> </td> 
   <td> <p>Cantidad de datos transferidos a través del escenario. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/scenario-detail.md" class="MCXref xref">Detalles del escenario en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Filtro</p> </td> 
   <td> <p>Funciones adicionales que se pueden aplicar entre dos módulos. Un filtro le permite trabajar solo con paquetes que se ajusten a ciertos criterios. Puede aplicar varios filtros diferentes. Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/add-a-filter-to-a-scenario.md" class="MCXref xref">Añadir un filtro a un escenario en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Identificador</p> </td> 
   <td> <p>Nombre que se utiliza para identificar un paquete de forma única. Un ID se utiliza generalmente para diferenciar un paquete que se va a actualizar o eliminar de un servicio determinado.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Elementos</p> </td> 
   <td> <p>Una parte de un paquete. Los paquetes pueden constar de varios elementos. Existen varios tipos de elementos: texto, número, booleano (sí/no), fecha, hora, búfer (datos binarios), colecciones, seleccionar menú, matriz y validación.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Iterator]</p> </td> 
   <td> <p>Tipo de módulo que le permite tomar un paquete de datos (una matriz de datos) y dividirlo en paquetes separados. Para obtener más información, consulte <a href="../../workfront-fusion/modules/iterator-module.md" class="MCXref xref">Módulo [!UICONTROL Iterator] en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Módulo</p> </td> 
   <td> <p>Un solo paso dentro de un escenario que realiza una función, como crear un registro, dentro de la aplicación o servicio asociado.</p> <p>Cada aplicación o servicio tiene varios módulos que definen la forma en que responde a una solicitud.</p> <p>Existen 4 tipos de módulos: acciones, déclencheur, iteradores y agregadores.</p> <p> <img src="assets/module.jpg"> </p> <p>Para obtener más información, consulte <a href="../../workfront-fusion/modules/module-types.md" class="MCXref xref">Tipos de módulos</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Operación</p> </td> 
   <td> <p>Tarea realizada por un módulo. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Claves públicas/privadas</td> 
   <td>Las claves pública y privada se utilizan para cifrar y descifrar datos. La clave pública se puede distribuir y cualquier persona con la clave pública puede cifrar datos, pero solo la clave privada puede descifrarla. Del mismo modo, un usuario con una clave privada puede cifrar datos que cualquiera que tenga la clave pública puede descifrar. El cifrado de clave privada garantiza que los datos provengan del propietario de la clave privada y sirve como validación de la fuente de los datos.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Router]</p> </td> 
   <td>Permite duplicar datos o agregar nuevas rutas a un escenario, para reenrutar datos y gestionar diferentes grupos de datos por separado. Para obtener más información, consulte <a href="../../workfront-fusion/modules/router-module.md" class="MCXref xref">Módulo [!UICONTROL Router] en [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Escenario</p> </td> 
   <td> <p>Una serie creada por el usuario de pasos automatizados, cada uno representado y realizado por un módulo. El propósito de un escenario es mover y manipular datos.</p> <p> <img src="assets/scenario-350x178.jpg" style="width: 350;height: 178;"> </p> <p> Para obtener más información, consulte <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Crear un escenario en[!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Transacciones</p> </td> 
   <td> <p>[!DNL Workfront Fusion] utiliza el procesamiento transaccional para capturar el ciclo vital del escenario. Una transacción consta de varias fases durante las cuales los datos se transforman de un estado coherente a otro estado coherente. Hay 4 fases: inicialización, operación (lectura o escritura), confirmación/reversión y finalización.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Déclencheur</p> </td> 
   <td> <p>Un módulo que le permite obtener paquetes que se añadieron o actualizaron desde la última ejecución de un escenario. Existen dos tipos de déclencheur: sondeo e instantáneo (webhooks). Para obtener más información, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Déclencheur instantáneos (enlaces web) en [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Weblock</p> </td> 
   <td> <p>Un tipo especial de déclencheur que le permite ejecutar un escenario inmediatamente después de que un nuevo paquete esté disponible. Para obtener más información, consulte <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Déclencheur instantáneos (webhooks) en [!UICONTROL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
