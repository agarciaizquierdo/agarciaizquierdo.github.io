---
layout: post
title: REGISTRAR UNA DLL EN SISTEMAS 64 BITS
date: 2011-08-01 13:12
author: agarciaizquierdo
comments: true
categories: [AeXAgentDiagnostics.dll, ALTIRIS, REGISTRAR DLL, REGSVR32.EXE, Sin categoría, SYSWOW64]
---
Buenas, en este post os vamos a hablar como registrar una DLL 32 bits en windows 2K8R2, y en un sistema 64 bits(W7,VISTA...).<br />Es muy sencillo simplemente nos vamos a la ruta: <b>C:\Windows\SysWOW64</b> y desde aquí ejecutamos el mismo comando que ejecutábamos anteriormente <b>regsvr32.exe. </b>Un ejemplo seria el siguiente:<br /><br /><b>C:\Windows\SysWOW64&gt;regsvr32.exe "E:\Altiris\Altiris Agent\AeXAgentDiagnostics.dll" </b> y nos aparecia la siguiente ventana<br /><br /><div class="separator" style="clear:both;text-align:center;"><a href="https://alvarogarciahome.files.wordpress.com/2011/08/5a18b-regsrv.jpg" style="margin-left:1em;margin-right:1em;"><img border="0" height="130" src="https://alvarogarciahome.files.wordpress.com/2011/08/5a18b-regsrv.jpg?w=300" width="400" /></a></div><div class="separator" style="clear:both;text-align:center;"><br /></div><div class="separator" style="clear:both;text-align:left;">Por lo que ya tendriamos nuestra DLL registrada.</div><div class="separator" style="clear:both;text-align:left;">Ademas aqui justo he registrado la DLL de diagnostico de Altiris, de la que hablaremos seguramente en otros post ;)</div><div class="separator" style="clear:both;text-align:left;">Decir que en la carpeta <b>SysWOW64 </b>tenemos las version 32 bits de los complementos de Windows.</div><div class="separator" style="clear:both;text-align:left;">La explicacion aqui del <a href="http://technet.microsoft.com/es-es/library/cc749541.aspx">technet</a></div><div class="separator" style="clear:both;text-align:left;">Un saludo</div><b><br /></b>