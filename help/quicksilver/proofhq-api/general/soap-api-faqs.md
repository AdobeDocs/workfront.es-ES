---
title: Preguntas frecuentes sobre API SOAP
description: Preguntas frecuentes sobre API SOAP
author: Becky
draft: Probably
feature: Workfront API, Workfront Proof
exl-id: fcf89bd6-0e07-42a7-9ae3-9a1309e51946
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '803'
ht-degree: 0%

---

# Preguntas frecuentes sobre API SOAP

## ¿Cómo creo mi primera prueba de archivo?

Se siguen tres pasos sencillos:

**Paso 1**: Cargue el archivo a Workfront Proof enviándolo a través de una solicitud de anuncio a  [https://soap.proofhq.com/upload.php](https://soap.proofhq.com/upload.php). Le devolveremos el hash del archivo - esto es muy importante! Tenga en cuenta que en este momento no verá nada en su cuenta, todo lo que ha hecho hasta ahora es enviarnos el archivo, pero no nos dijo qué hacer con él.

**Paso 2**: Si todavía no tiene un ID de sesión, obtenga uno de ellos utilizando los métodos doLogin() o getSessionID() . Utilice el primero para &quot;iniciar sesión&quot; con la dirección de correo electrónico y contraseña de un usuario, o el segundo método si tiene la dirección de correo electrónico y el token de autenticación del usuario.

**Paso 3:** Ahora es el momento de crear su prueba. Utilice el método createProof() y envíenos al menos los campos requeridos (actualmente solo hay 5 de ellos). Asegúrese de establecer el parámetro Hash en el hash de archivo devuelto durante el &quot;Paso 1&quot;, ya que esto nos permite determinar qué archivo utilizar al crear la prueba.

Si ahora inicia sesión en su cuenta, verá la prueba.

## ¿Cómo creo mi primera prueba de instantánea web?

Tiene dos pasos sencillos:

**Paso 1**: Si todavía no tiene un ID de sesión, obtenga uno de ellos utilizando los métodos doLogin() o getSessionID() . Utilice el primero para &quot;iniciar sesión&quot; con la dirección de correo electrónico y contraseña de un usuario, o el segundo método si tiene la dirección de correo electrónico y el token de autenticación del usuario.

**Paso 2:**Ahora es el momento de crear la prueba. Utilice el método createProof() y envíenos al menos los campos requeridos (actualmente solo hay 5 de ellos). Asegúrese de establecer el parámetro Hash en &quot;web&quot; y el parámetro SourceName como dirección URL de la página web que desea capturar.

Si ahora inicia sesión en su cuenta, verá la prueba.

## ¿Cuál es la diferencia entre una prueba y una versión?

En Workfront Proof, las versiones se muestran como una única prueba. Al hacer clic en una versión específica de la interfaz de usuario web, se mostrarán los detalles de esa versión. En realidad, cada versión es una prueba independiente y la interfaz de usuario web las muestra juntas.

Desde la perspectiva de la API, cada versión es una prueba independiente y las pruebas están vinculadas entre sí por sus ID.

**createProof()** siempre creará **versión 1** de la prueba. Supongamos que para nuestro ejemplo el ID devuelto para esta prueba &quot;100&quot;.

Al usar **createProofVersion()** envíe siempre el ID de la versión anterior. Si queremos crear **versión 2** en la prueba &quot;100&quot;, **pase &quot;100&quot; para ParentFileID** parámetro. Esto indica al sistema que esta prueba debe ser la versión 2 del conjunto. El método devolverá un ID de prueba único, por ejemplo, supongamos que es &quot;101&quot;.

Si se trata de una tercera versión, es decir, **versión 3** es obligatorio, llamará a **createProofVersion()** de nuevo y esta vez **pase &quot;101&quot; para ParentFileID** que garantizará que la lista de versiones vinculada se cree correctamente.

## ¿Debo obtener un nuevo ID de sesión antes de cada llamada a ?

Es importante señalar que cada ID de sesión es esencialmente un usuario que realiza las acciones. 

No es necesario obtener un nuevo ID de sesión antes de cada llamada a la API y este permanecerá válido durante 24 horas. La hora de caducidad se restablece cada vez que realiza una llamada a la API.

## ¿Qué es una prueba/URL personal?

**Equipo/público**: Cada versión de prueba tiene una URL de equipo (pública) única. Si está habilitada, se abrirá la prueba en modo de solo lectura. Puede obtener la dirección URL del equipo mediante el [getProofURL()](http://api.proofhq.com/home/proofs/getproofurl) método.

**Personal**: Una dirección URL personal es única para cada revisor y versión de prueba. Si un conjunto de pruebas contiene 3 versiones y un revisor está en todas las versiones, el revisor tendrá 3 direcciones URL personales únicas. Una URL personal abre la versión de prueba con el revisor ya identificado y, por lo tanto, debe mantenerse a salvo y no compartirse. Las direcciones URL personales se pueden obtener llamando a la función [getProofReviewers()](http://api.proofhq.com/home/proofs/getproofreviewers) método y, a continuación, iterando sobre cada  [SOAPRecepentObject](http://api.proofhq.com/home/objects/soaprecipientobject) y obtener el parámetro &quot;proof_url&quot;.

## >Cómo incluir parámetros personalizados al abrir miniproof?

La miniprueba permite incrustar la herramienta de prueba en su propia página. Se puede incluir un parámetro &quot;referer&quot; como parte de miniproof para proporcionar una URL de redireccionamiento cuando un usuario hace clic en el botón de cierre de miniproof. Puede incluir cualquier número de parámetros personalizados como parte de esta dirección URL de redireccionamiento adjuntándolos con el carácter &quot;&amp;&quot; de escape, por ejemplo %26.

Por ejemplo, la URL de prueba mínima
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com&customparam1=somevalue&customparam2=` debe estar codificado como 
`https://app.proofhq.com/viewer/proofingcode?referer=closingurl.com%26customparam1=somevalue%26customparam2=` para que se pasen los parámetros personalizados.

## ¿Cómo se crea un cliente de servicio web de Java?

[Este vídeo](http://screencast.com/t/xsSNrqs5b) muestra cómo puede crear un cliente de servicio web de Java mediante Eclipse y la definición WSDL de prueba de Workfront.
