<!DOCTYPE html>

<html lang="en">

<head>
    <meta charset="utf-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
    <meta name="apple-mobile-web-app-capable" content="yes">
    <meta name="apple-mobile-web-app-status-bar-style" content="black">
    <meta name="mobile-web-app-capable" content="yes">
</head>

<body>
    <div id="doc" class="markdown-body container-fluid comment-enabled" data-hard-breaks="true"><h1 id="Introducción" data-id="Introducción"><a class="anchor hidden-xs" href="#Introducción" title="Introducción"><span class="octicon octicon-link"></span></a><span>Introducción</span></h1><h6 id="tags-SID-lab" data-id="tags-SID-lab"><a class="anchor hidden-xs" href="#tags-SID-lab" title="tags-SID-lab"><span class="octicon octicon-link"></span></a><span>tags: </span><code>SID-lab</code></h6><p><span class="toc"><ul>
<li><a href="#Introducción" title="Introducción">Introducción</a><ul>
<li><a href="#Ejercicio-Introductorio" title="Ejercicio Introductorio">Ejercicio Introductorio</a><ul>
<li><a href="#Definición-del-problema" title="Definición del problema">Definición del problema</a></li>
<li><a href="#Toma-de-decisiones" title="Toma de decisiones">Toma de decisiones</a></li>
<li><a href="#Posibles-ampliaciones" title="Posibles ampliaciones">Posibles ampliaciones</a></li>
</ul>
</li>
<li><a href="#Tecnología-actual" title="Tecnología actual">Tecnología actual</a></li>
<li><a href="#JADE-Java-Agent-DEvelopment-framework" title="JADE: Java Agent DEvelopment framework">JADE: Java Agent DEvelopment framework</a></li>
</ul>
</li>
</ul>
</span></p><hr><h2 id="Ejercicio-Introductorio" data-id="Ejercicio-Introductorio"><a class="anchor hidden-xs" href="#Ejercicio-Introductorio" title="Ejercicio-Introductorio"><span class="octicon octicon-link"></span></a><span>Ejercicio Introductorio</span></h2><h3 id="Definición-del-problema" data-id="Definición-del-problema"><a class="anchor hidden-xs" href="#Definición-del-problema" title="Definición-del-problema"><span class="octicon octicon-link"></span></a><span>Definición del problema</span></h3><ul>
<li><span>Sistema distribuido formado por agentes con diferentes capcidades:</span>
<ul>
<li><u><span>Agente termómetro:</span></u><span> mide la temperatura.</span></li>
<li><u><span>Agente termostato:</span></u><span> obtiene las mediciones del termometro y actúa en base a la temperatura.</span></li>
</ul>
</li>
</ul><h3 id="Toma-de-decisiones" data-id="Toma-de-decisiones"><a class="anchor hidden-xs" href="#Toma-de-decisiones" title="Toma-de-decisiones"><span class="octicon octicon-link"></span></a><span>Toma de decisiones</span></h3><ul>
<li><span>¿Cómo recibe el agente termostato la información? (pull o push).</span></li>
<li><span>¿Cómo se comunican los agentes? (TCP, UDP…).</span></li>
<li><span>¿En qué formato se envía la información? (Strings, objetos…)</span></li>
<li><span>Significado: ¿Cómo se interpreta la información?</span></li>
<li><span>Protocolo: ¿petición y respuesta? ¿sincronía o asincronía?</span></li>
<li><span>¿Cómo se encuentran los demas agentes?</span></li>
<li><span>¿Qué pasa si algún agente falla?</span></li>
</ul><h3 id="Posibles-ampliaciones" data-id="Posibles-ampliaciones"><a class="anchor hidden-xs" href="#Posibles-ampliaciones" title="Posibles-ampliaciones"><span class="octicon octicon-link"></span></a><span>Posibles ampliaciones</span></h3><ul>
<li><span>Las 8 falacias de los sistemas distribuidos (Deutsch, Gosling).</span></li>
<li><span>Todo lo que puede ir mal, irá mal.</span></li>
</ul><hr><h2 id="Tecnología-actual" data-id="Tecnología-actual"><a class="anchor hidden-xs" href="#Tecnología-actual" title="Tecnología-actual"><span class="octicon octicon-link"></span></a><span>Tecnología actual</span></h2><ul>
<li><span>Plataformas/Infraestructura (con descubrimiento de servicios).</span>
<ul>
<li><span>Kubernetes, Mesos, Consul, Zookeeper.</span></li>
</ul>
</li>
<li><span>Microservicios.</span>
<ul>
<li><span>Spring Boot, Akka, Axon, Erlang/OTP, websockets.</span></li>
</ul>
</li>
<li><span>Bases de datos distribuidas.</span>
<ul>
<li><span>Redis, Riak, Cassandra, Hbase, MongoDB, ElasticSearch.</span></li>
</ul>
</li>
<li><span>Colas de mensajes y gestión de eventos.</span>
<ul>
<li><span>Kafka, RabbitMQ, EventStore.</span></li>
</ul>
</li>
<li><span>Monitorización.</span>
<ul>
<li><span>Grafana, Prometheus, Datadog, Kibana.</span></li>
</ul>
</li>
<li><span>Sistemas basados en agentes (no distribuidos).</span>
<ul>
<li><span>Agentes simples: Repast, Repast-HPC, NetLogo, MASON, Pandora, Pogamut.</span></li>
<li><span>Agentes con razonamiento lógico: 2-APL, 3-APL, OperettA, GOAL.</span></li>
</ul>
</li>
<li><span>Plataformas distribuidas de agentes.</span>
<ul>
<li><span>JADE</span></li>
<li><span>Jason (AgentSpeak)</span></li>
<li><span>Jadex</span></li>
<li><span>JACK</span></li>
<li><span>SPADE</span></li>
</ul>
</li>
</ul><hr><h2 id="JADE-Java-Agent-DEvelopment-framework" data-id="JADE-Java-Agent-DEvelopment-framework"><a class="anchor hidden-xs" href="#JADE-Java-Agent-DEvelopment-framework" title="JADE-Java-Agent-DEvelopment-framework"><span class="octicon octicon-link"></span></a><span>JADE: Java Agent DEvelopment framework</span></h2><ul>
<li><span>Software LGPL mantenido por Telecom Italia.</span>
<ul>
<li><a href="https://jade.tilab.com/" target="_blank" rel="noopener"><span>https://jade.tilab.com/</span></a></li>
</ul>
</li>
<li><span>¿Por qué JADE?</span>
<ul>
<li><span>Plataforma realmente distribuida y totalmente asíncrona.</span></li>
<li><span>Descubrimiento de agentes por nombre, tipo o capacidades.</span></li>
<li><span>Abstracción para la comunicación entre agentes (cola de mensajes).</span></li>
<li><span>Abstracción para definir el comportamiento de los agentes.</span></li>
<li><span>Compatible con estándares de la comunidad multi-agente (especificaciones FIPA).</span></li>
<li><span>Portabilidad de agentes a través de contenedores y plataformas.</span></li>
</ul>
</li>
<li><span>Libro (copia en la biblioteca):</span>
<ul>
<li><em><span>Developing Multi-Agent Systems with JADE</span></em><span> (Bellifemine et al., 2007)</span></li>
</ul>
</li>
</ul><p><img src="https://i.imgur.com/lwEgaXw.png" alt="" loading="lazy"></p></div>
    <div class="ui-toc dropup unselectable hidden-print" style="display:none;">
        <div class="pull-right dropdown">
            <a id="tocLabel" class="ui-toc-label btn btn-default" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false" title="Table of content">
                <i class="fa fa-bars"></i>
            </a>
            <ul id="ui-toc" class="ui-toc-dropdown dropdown-menu" aria-labelledby="tocLabel">
                <div class="toc"><ul class="nav">
<li><a href="#Introducción" title="Introducción">Introducción</a><ul class="nav">
<li><a href="#Ejercicio-Introductorio" title="Ejercicio Introductorio">Ejercicio Introductorio</a><ul class="nav">
<li><a href="#Definición-del-problema" title="Definición del problema">Definición del problema</a></li>
<li><a href="#Toma-de-decisiones" title="Toma de decisiones">Toma de decisiones</a></li>
<li><a href="#Posibles-ampliaciones" title="Posibles ampliaciones">Posibles ampliaciones</a></li>
</ul>
</li>
<li><a href="#Tecnología-actual" title="Tecnología actual">Tecnología actual</a></li>
<li><a href="#JADE-Java-Agent-DEvelopment-framework" title="JADE: Java Agent DEvelopment framework">JADE: Java Agent DEvelopment framework</a></li>
</ul>
</li>
</ul>
</div><div class="toc-menu"><a class="expand-toggle" href="#">Expand all</a><a class="back-to-top" href="#">Back to top</a><a class="go-to-bottom" href="#">Go to bottom</a></div>
            </ul>
        </div>
    </div>
    <div id="ui-toc-affix" class="ui-affix-toc ui-toc-dropdown unselectable hidden-print" data-spy="affix" style="top:17px;display:none;" null null>
        <div class="toc"><ul class="nav">
<li><a href="#Introducción" title="Introducción">Introducción</a><ul class="nav">
<li><a href="#Ejercicio-Introductorio" title="Ejercicio Introductorio">Ejercicio Introductorio</a><ul class="nav">
<li><a href="#Definición-del-problema" title="Definición del problema">Definición del problema</a></li>
<li><a href="#Toma-de-decisiones" title="Toma de decisiones">Toma de decisiones</a></li>
<li><a href="#Posibles-ampliaciones" title="Posibles ampliaciones">Posibles ampliaciones</a></li>
</ul>
</li>
<li><a href="#Tecnología-actual" title="Tecnología actual">Tecnología actual</a></li>
<li><a href="#JADE-Java-Agent-DEvelopment-framework" title="JADE: Java Agent DEvelopment framework">JADE: Java Agent DEvelopment framework</a></li>
</ul>
</li>
</ul>
</div><div class="toc-menu"><a class="expand-toggle" href="#">Expand all</a><a class="back-to-top" href="#">Back to top</a><a class="go-to-bottom" href="#">Go to bottom</a></div>
    </div>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jquery/3.1.1/jquery.min.js" integrity="sha256-hVVnYaiADRTO2PzUGmuLJr8BLUSjGIZsDYGmIJLv2b8=" crossorigin="anonymous"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/3.3.7/js/bootstrap.min.js" integrity="sha256-U5ZEeKfGNOja007MMD3YBI0A3OSZOQbeG6z2f2Y0hu8=" crossorigin="anonymous" defer></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/gist-embed/2.6.0/gist-embed.min.js" integrity="sha256-KyF2D6xPIJUW5sUDSs93vWyZm+1RzIpKCexxElmxl8g=" crossorigin="anonymous" defer>
</body>

</html>
