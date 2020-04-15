---
layout: post
title: ¿QUE ES EL BACK PRESURE?
date: 2011-10-08 10:36
author: agarciaizquierdo
comments: true
categories: [BACK PRESUPRE, EDGETRASNPORT.EXE.CONFIG, EXCHANGE, Sin categoría]
---
Buenas, hacia tiempo que quería hablar de un tema, pero no he encontrado tiempo. En esta ocasión os voy hablar del <b>Back Presure </b>de<b> Exchange 2010.</b><br />El <b>Edge Transport</b> y el<b> Hub Transport </b>monitorizan los recursos del sistema (espacio en disco, memoria RAM...)<br />En <b>Exchange 2007</b> ya existía, pero funcionaba de forma diferente a <b>Exchange 2010.</b><br />En <b>Exchange 2007</b> directamente rechazaba los mensajes entrantes, pero en<b> Exchange 2010</b> sin embargo no, empiezan a entrar mensajes de forma mucho mas lenta y algunos son rechazados, pero desde fuera, ya que los correos internos si suelen funcionar, ya que <b>Exchange </b>entiende que un correo interno no es una conexión externa.<br />Es muy útil, ya que evitara que perdamos o se corrompa nuestra BBD si no tenemos hecho un backup, pero en muchas ocasiones nos podemos volver locos buscando la razón de que no entren correos.<br />Para detectarlo lo mejor es buscar en eventos del <b>Hub transport</b> y <b>Edge transport</b> en nuestro visor de eventos, estos son los mas comunes:<br /><br /><br />Event Type: Error<br />Event Source: MSExchangeTransport<br />Event ID: 15004<br />Description: Resource pressure increased from Previous Utilization Level to Current Utilization Level.<br /><br /><br />Event Type: Information<br />Event Source: MSExchangeTransport<br />Event ID: 15005<br />Description: Resource pressure decreased from Previous Utilization Level to Current Utilization Level.<br /><br /><br />Event Type: Error<br />Event Source: MSExchangeTransport<br />Event ID: 15006<br />Description: The Microsoft Exchange Transport service is rejecting messages because available disk space is below the configured threshold. Administrative action may be required to free disk space for the service to continue operations.<br /><br /><br />Event Type: Error<br />Event Source: MSExchangeTransport<br />Event ID: 15007<br />Description: The Microsoft Exchange Transport service is rejecting message submissions because the service continues to consume more memory than the configured threshold. This may require that this service be restarted to continue normal operation.<br /><br />Lo que podemos hacer para evitar esto es:<br /><br /><ul><li>Como opción mas recomendable sin duda es liberar de espacio o carga de trabajo a nuestro <b>Exchange,</b> o aumentar sus recursos (aumentar disco,memoria, crear otro servidor de con el Rol de Mailbox...).</li><li>Luego tenemos la opción de editar el archivo de configuracion (C:\Program Files\Microsoft\Exchange Server\V14\Bin\ EdgeTransport.exe.config) y rebajar los valores de alerta</li><li>Por ultimo, y como peor opción y nada recomendable, podemos deshabilitarlo, en el mismo fichero de antes, buscando el valor "<b>EnableResourceMonitoring</b>" y poniéndolo igual a <b>False.</b></li></ul><div>Como siempre os dejo un poco de literatura del Technet:</div><div><br /></div><div><ul><li><b>Understanding Back Pressure</b></li></ul>          <a href="http://technet.microsoft.com/en-us/library/bb201658(EXCHG.140).aspx#File">http://technet.microsoft.com/en-us/library/bb201658(EXCHG.140).aspx#File</a></div><div><br /></div><div><br /></div><div>Un saludo</div><br /><br /><br /><br /><br /><br /><br /><div style="padding:0 0 1em 30px;"><br /></div>