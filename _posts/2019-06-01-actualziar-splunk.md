---
layout: post
title: Actualziar Splunk
date: 2019-06-01
author: agarciaizquierdo
comments: true
categories: [Splunk, Splunk Español, Splunk Update]
---
<div class="separator" style="clear: both; text-align: center;">
<a href="https://1.bp.blogspot.com/-CvH25Xy90Kg/XQU7l2czU5I/AAAAAAABP_4/AUNgu5q8M3If4lxkmxiICpKnaEbhUpGtgCLcBGAs/s1600/Update-2018.jpg" imageanchor="1" style="margin-left: 1em; margin-right: 1em;"><img border="0" data-original-height="400" data-original-width="770" height="166" src="https://1.bp.blogspot.com/-CvH25Xy90Kg/XQU7l2czU5I/AAAAAAABP_4/AUNgu5q8M3If4lxkmxiICpKnaEbhUpGtgCLcBGAs/s320/Update-2018.jpg" width="320" /></a></div>
<br />
Unos de los momentos críticos y que deben ser planificados son las actualizaciones de versión. Hace unos días <b>Splunk</b> liberó la versión 7.3, la cual trae bastantes novedades, aunque en este post no voy a explicar estas novedades, sino algunas cosas que debemos tener en cuenta antes de actualizar.<br />
<br />
La idea de este post me vino a la cabeza después de leer <a href="https://www.splunk.com/blog/2019/06/13/kick-start-your-splunk-software-upgrade-with-a-few-best-practices.html" target="_blank">este</a> articulo del <b><a href="https://www.splunk.com/blog" target="_blank">blog</a></b> de <b>Splunk, </b>desde luego esta bien pasarse de forma regular a ojear los post.<br />
<br />
En este post explican algunas de las mejores practicas, como leerse primero siempre los siguientes enlaces:<br />
<ul>
<li>Leer las novedades y cambios en la versión, <a href="https://docs.splunk.com/Documentation/Splunk/7.3.0/Installation/AboutupgradingREADTHISFIRST" target="_blank">aqui</a>&nbsp;</li>
<li>Crear un plan detallado de la migración, identificando los componentes, <a href="https://answers.splunk.com/answers/750462/whats-the-order-of-operations-for-upgrading-splunk.html?childToView=750464#answer-750464" target="_blank">aquí</a> un ejemplo muy bueno, aqui me gustaria destacar dos puntos</li>
<ul>
<li>Backup, backup, backup, esto nunca sobra, <b>Splunk </b>tiene sus particularidades, ya lo explicaré en un futuro post</li>
<li>Entorno de pre-producción, no siempre es posible, pero cuanto mas compleja sea nuestra arquitectura más necesario es</li>
</ul>
<li>Revisar las compatibilidades es fundamental, crear una matriz de versiones y Apps instaladas, <a href="https://docs.splunk.com/Documentation/VersionCompatibility/current/Matrix/CompatMatrix" target="_blank">aqui</a> una tabla de ejemplo.</li>
</ul>
<br />
<br />
  
Unos de los momentos críticos y que deben ser planificados son las actualizaciones de versión. Hace unos días **Splunk** liberó la versión 7.3, la cual trae bastantes novedades, aunque en este post no voy a explicar estas novedades, sino algunas cosas que debemos tener en cuenta antes de actualizar.  
  
La idea de este post me vino a la cabeza después de leer [este](https://www.splunk.com/blog/2019/06/13/kick-start-your-splunk-software-upgrade-with-a-few-best-practices.html) articulo del **[blog](https://www.splunk.com/blog)** de **Splunk,** desde luego esta bien pasarse de forma regular a ojear los post.  
  
En este post explican algunas de las mejores practicas, como leerse primero siempre los siguientes enlaces:  

*   Leer las novedades y cambios en la versión, [aqui](https://docs.splunk.com/Documentation/Splunk/7.3.0/Installation/AboutupgradingREADTHISFIRST) 
*   Crear un plan detallado de la migración, identificando los componentes, [aquí](https://answers.splunk.com/answers/750462/whats-the-order-of-operations-for-upgrading-splunk.html?childToView=750464#answer-750464) un ejemplo muy bueno, aqui me gustaria destacar dos puntos

*   Backup, backup, backup, esto nunca sobra, **Splunk** tiene sus particularidades, ya lo explicaré en un futuro post
*   Entorno de pre-producción, no siempre es posible, pero cuanto mas compleja sea nuestra arquitectura más necesario es

*   Revisar las compatibilidades es fundamental, crear una matriz de versiones y Apps instaladas, [aqui](https://docs.splunk.com/Documentation/VersionCompatibility/current/Matrix/CompatMatrix) una tabla de ejemplo.
