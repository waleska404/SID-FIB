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
    <div id="doc" class="markdown-body container-fluid comment-enabled" data-hard-breaks="true"><h1 id="Origins" data-id="Origins"><a class="anchor hidden-xs" href="#Origins" title="Origins"><span class="octicon octicon-link"></span></a><span>Origins</span></h1><h6 id="tags-SID-teo" data-id="tags-SID-teo"><a class="anchor hidden-xs" href="#tags-SID-teo" title="tags-SID-teo"><span class="octicon octicon-link"></span></a><span>tags: </span><code>SID-teo</code></h6><p><span class="toc"><ul>
<li><a href="#Trends-in-Computer-Science" title="Trends in Computer Science">Trends in Computer Science</a><ul>
<li><a href="#Origins-of-MAS-Five-trends" title="Origins of MAS; Five trends:">Origins of MAS; Five trends:</a></li>
<li><a href="#Ambient-Intelligence" title="Ambient Intelligence">Ambient Intelligence</a></li>
<li><a href="#Edge-Computing" title="Edge Computing">Edge Computing</a></li>
<li><a href="#Computer-Science-Progression" title="Computer Science Progression">Computer Science Progression</a></li>
</ul>
</li>
<li><a href="#Agents-and-Multiagent-Systems" title="Agents and Multiagent Systems">Agents and Multiagent Systems</a><ul>
<li><a href="#Building-Agents-and-MAS" title="Building Agents and MAS">Building Agents and MAS</a></li>
<li><a href="#Influences" title="Influences">Influences</a></li>
</ul>
</li>
<li><a href="#Two-views-of-the-Field" title="Two views of the Field">Two views of the Field</a></li>
<li><a href="#Standards-FIPA-wwwfipaorg" title="Standards: FIPA (www.fipa.org)">Standards: FIPA (www.fipa.org)</a></li>
</ul>
</li>
</ul>
</span></p><hr><h2 id="Trends-in-Computer-Science" data-id="Trends-in-Computer-Science"><a class="anchor hidden-xs" href="#Trends-in-Computer-Science" title="Trends-in-Computer-Science"><span class="octicon octicon-link"></span></a><span>Trends in Computer Science</span></h2><h3 id="Origins-of-MAS-Five-trends" data-id="Origins-of-MAS-Five-trends"><a class="anchor hidden-xs" href="#Origins-of-MAS-Five-trends" title="Origins-of-MAS-Five-trends"><span class="octicon octicon-link"></span></a><span>Origins of MAS; Five trends:</span></h3><blockquote>
<p><em><span>Five ongoing trends have marked the history ofcomputing</span></em><span> -M. Wooldridge:</span></p>
</blockquote><ul>
<li><strong><span>Ubiquity</span></strong><span>: As processing capability spreads and costs go down, computation (and intelligence of a sort) becomes ubiquitous.</span></li>
<li><strong><span>Interconnection</span></strong><span>: Computer systems today are networked into large distributed systems. Some researchers are putting forward theoretical models that portray computing as primarily a </span><u><span>process of interaction</span></u><span>.</span></li>
<li><strong><span>Intelligence</span></strong><span>: The complexity of tasks that we are capable or delegate to computers has grown to the limits that we can identify those systems as </span><u><span>intelligent</span></u><span>.</span></li>
<li><strong><span>Delegation</span></strong><span>: We are </span><u><span>giving control</span></u><span> to computers. They are doing more for us without our intervention.</span></li>
<li><strong><span>Human orientation</span></strong><span>: from machine-oriented views of programming toward concepts and metaphors that more closely reflect the way we ourselves understand the world.</span></li>
</ul><p><u><span>Delegation and Intelligence</span></u><span> → The ability of computer systems to act </span><strong><span>independently</span></strong><span> and in a way that </span><strong><span>represents our best interests</span></strong><span> while </span><strong><span>interacting</span></strong><span> with other humans or systems.</span></p><p><u><span>Interconnection and Distribution</span></u><span> → Systems that can </span><strong><span>cooperate</span></strong><span> and </span><strong><span>reach agreements</span></strong><span> (or even compete) with other systems that have different interests.</span></p><blockquote style="border-left-color: rgb(55, 185, 191);">
<p><span>FROM:</span></p>
<ul>
<li><span>How can I build a system that produces the correct output given some input?</span></li>
</ul>
<p><span>TO:</span></p>
<ul>
<li><span>How can I build a system that can operate </span><strong><span>independently on my behalf in a networked, distributed, large-scale environment</span></strong><span> in which it will need to </span><strong><span>interact</span></strong><span> with different other components pertaining to other users?</span><br>
<span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><h3 id="Ambient-Intelligence" data-id="Ambient-Intelligence"><a class="anchor hidden-xs" href="#Ambient-Intelligence" title="Ambient-Intelligence"><span class="octicon octicon-link"></span></a><span>Ambient Intelligence</span></h3><ul>
<li><span>Aimed at seamless delivery of services and applications.</span></li>
<li><span>Relies on ubiquitous computing, ubiquitous communication and intelligent user interfaces.</span></li>
<li><span>User-centred goals and activity.</span></li>
<li><span>Autonomy, distribution, adaptation, responsiveness.</span></li>
<li><span>Requires agents to be able to interact with numerous other agents in the environment around them in order to achieve their goals.</span></li>
</ul><h3 id="Edge-Computing" data-id="Edge-Computing"><a class="anchor hidden-xs" href="#Edge-Computing" title="Edge-Computing"><span class="octicon octicon-link"></span></a><span>Edge Computing</span></h3><ul>
<li><span>Objective: to bring computation and data closer to the sources (i.e. to the end user).</span></li>
<li><span>Three layers of the </span><em><span>continuum</span></em><span>:</span>
<ul>
<li><strong><span>Edge</span></strong><span>: closest to the user. Wearables, smartphones, IoT sensors.</span></li>
<li><strong><span>Fog</span></strong><span>: low latency fixed nodes. Mobile cell towers, wireless routers, street cabinets.</span></li>
<li><strong><span>Cloud</span></strong><span>: specialised large-scale computing resources installments. Public clouds, private clouds, supercomputing facilities.</span></li>
</ul>
</li>
<li><span>Many challenges: Efficiency, security, privacy.</span></li>
</ul><h3 id="Computer-Science-Progression" data-id="Computer-Science-Progression"><a class="anchor hidden-xs" href="#Computer-Science-Progression" title="Computer-Science-Progression"><span class="octicon octicon-link"></span></a><span>Computer Science Progression</span></h3><ul>
<li><span>These issues were not studied in Computer Science until recently (less than 25 years).</span></li>
<li><span>All of these trends have led to the emergence of a new field in Computer Science: </span><strong><u><span>multiagent systems/computational Intelligence.</span></u></strong></li>
<li><span>Wooldridge says that programming has progressed through:</span>
<ul>
<li><span>machine code → assembly language → machine-independent programming languages → sub-routines → procedures &amp; functions → abstract data types → objects → </span><strong><u><span>agents</span></u></strong><span>.</span></li>
</ul>
</li>
</ul><hr><h2 id="Agents-and-Multiagent-Systems" data-id="Agents-and-Multiagent-Systems"><a class="anchor hidden-xs" href="#Agents-and-Multiagent-Systems" title="Agents-and-Multiagent-Systems"><span class="octicon octicon-link"></span></a><span>Agents and Multiagent Systems</span></h2><ul>
<li><span>An </span><strong><u><span>agent</span></u></strong><span> is a computer system that is capable of </span><strong><span>independent</span></strong><span> action on behalf of its user or owner (figuring out what needs to be done to satisfy design objectives, rather than constantly being told).</span></li>
<li><span>A </span><strong><u><span>multiagent system</span></u></strong><span> is one that consists of a number of agents, which interact with one-another.</span>
<ul>
<li><span>In the most </span><u><span>simple case</span></u><span>, all agents are programmed by the same team and they collaborate to complete a task.</span></li>
<li><span>In the most </span><u><span>general case</span></u><span>, agents will be acting on behalf of users with different goals and motivations.</span>
<ul>
<li><span>To successfully interact, they will require the ability to </span><strong><span>cooperate</span></strong><span>, </span><strong><span>coordinate</span></strong><span>, and </span><strong><span>negotiate</span></strong><span> with each other, much as people do.</span></li>
</ul>
</li>
</ul>
</li>
<h3 id="Building-Agents-and-MAS" data-id="Building-Agents-and-MAS"><a class="anchor hidden-xs" href="#Building-Agents-and-MAS" title="Building-Agents-and-MAS"><span class="octicon octicon-link"></span></a><span>Building Agents and MAS</span></h3><ul>
<li><u><span>Building Agents</span></u><span>, we address questions such as:</span>
<ul>
<li><span>How do you state your preferences to your agent?</span></li>
<li><span>How can your agent compare different deals from different vendors? What if there are many different parameters?</span></li>
<li><span>What algorithms can your agent use to negotiate with other agents (to make sure you get a good deal)?</span></li>
</ul>
</li>
<li><u><span>Building Multiagent Systems</span></u><span>, we address questions such as:</span>
<ul>
<li><span>How can cooperation emerge in societies of self-interested agents?</span></li>
<li><span>What kinds of languages can agents use to communicate?</span></li>
<li><span>How can self-interested agents recognize conflict, and how can they (nevertheless) reach agreement?</span></li>
<li><span>How can autonomous agents coordinate their activities so as to (cooperatively) achieve goals?</span></li>
</ul>
</li>
<li><u><span>Problems</span></u><span>:</span>
<ul>
<li><span>How do we build agents capable of independent, </span><strong><span>autonomous action</span></strong><span>, so that they can successfully carry out tasks we delegate to them?</span>
<ul>
<li><strong><span>Agent design</span></strong><span> problem.</span></li>
</ul>
</li>
<li><span>How do we build agents that are capable of interacting (</span><strong><span>cooperating, coordinating, negotiating</span></strong><span>) with other agents in order to successfully carry out those delegated tasks, especially when the other agents cannot be assumed to share the same interests/goals?</span>
<ul>
<li><strong><span>Society design</span></strong><span> (micro/macro) problem.</span></li>
</ul>
</li>
</ul>
</li>
</ul><h3 id="Influences" data-id="Influences"><a class="anchor hidden-xs" href="#Influences" title="Influences"><span class="octicon octicon-link"></span></a><span>Influences</span></h3><ul>
<li><span>The field of Multiagent Systems is influenced and inspired by many other fields:</span>
<ul>
<li><strong><span>Philosopy, Logic, Game Theory, Economics, Social Sciences, Ecology</span></strong><span>.</span></li>
</ul>
</li>
<li><span>This can be both a strength (infusing well-founded methodologies into the field) and a weakness (there are many different views as to what the field is about).</span></li>
</ul><hr><h2 id="Two-views-of-the-Field" data-id="Two-views-of-the-Field"><a class="anchor hidden-xs" href="#Two-views-of-the-Field" title="Two-views-of-the-Field"><span class="octicon octicon-link"></span></a><span>Two views of the Field</span></h2><ul>
<li><u><span>Agents as a paradigm for software engineering:</span></u>
<ul>
<li><span>Software engineers have derived a progressively better understanding of the characteristics of complexity in software. It is now widely recognized that </span><strong><span>interaction</span></strong><span> is probably the most important single characteristic of complex software.</span></li>
<li><span>Over the last two decades, a major Computer Science research topic has been the development of tools and techniques to model, understand, and implement systems in which </span><strong><span>interaction</span></strong><span> is the norm.</span></li>
</ul>
</li>
<li><u><span>Agents as a tool for understanding human societies:</span></u>
<ul>
<li><span>Multiagent systems provide a novel new tool for simulating societies, which may help shed some light on various kinds of social processes.</span></li>
<li><span>This has analogies with the interest in </span><strong><span>theories of the mind</span></strong><span> explored by some artificial intelligence researchers and cognitive scientists.</span></li>
</ul>
</li>
</ul><hr><h2 id="Standards-FIPA-wwwfipaorg" data-id="Standards-FIPA-wwwfipaorg"><a class="anchor hidden-xs" href="#Standards-FIPA-wwwfipaorg" title="Standards-FIPA-wwwfipaorg"><span class="octicon octicon-link"></span></a><span>Standards: FIPA (</span><a href="http://www.fipa.org" target="_blank" rel="noopener"><span>www.fipa.org</span></a><span>)</span></h2><ul>
<li><span>International Agent Standard.</span>
<ul>
<li><span>Started in 1996 to provide agent technology specifications.</span></li>
<li><span>Part of IEEE (since 2005) as 11th standards committee.</span></li>
</ul>
</li>
</ul></div>
    <div class="ui-toc dropup unselectable hidden-print" style="display:none;">
        <div class="pull-right dropdown">
            <a id="tocLabel" class="ui-toc-label btn btn-default" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false" title="Table of content">
                <i class="fa fa-bars"></i>
            </a>
            <ul id="ui-toc" class="ui-toc-dropdown dropdown-menu" aria-labelledby="tocLabel">
                <div class="toc"><ul class="nav">
</html>
