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
    <div id="doc" class="markdown-body container-fluid comment-enabled" data-hard-breaks="true"><h1 id="Agent-Types-and-Architectures" data-id="Agent-Types-and-Architectures"><a class="anchor hidden-xs" href="#Agent-Types-and-Architectures" title="Agent-Types-and-Architectures"><span class="octicon octicon-link"></span></a><span>Agent Types and Architectures</span></h1><h6 id="tags-SID-teo" data-id="tags-SID-teo"><a class="anchor hidden-xs" href="#tags-SID-teo" title="tags-SID-teo"><span class="octicon octicon-link"></span></a><span>tags: </span><code>SID-teo</code></h6><p><span class="toc"><ul>
<li><a href="#Agent-Properties" title="Agent Properties">Agent Properties</a><ul>
<li><a href="#Agent-Definitions" title="Agent Definitions">Agent Definitions</a></li>
<li><a href="#Autonomy" title="Autonomy">Autonomy</a></li>
<li><a href="#Flexibility" title="Flexibility">Flexibility</a></li>
<li><a href="#Reactivity" title="Reactivity">Reactivity</a></li>
<li><a href="#Proactivness" title="Proactivness">Proactivness</a></li>
<li><a href="#Social-Ability" title="Social Ability">Social Ability</a></li>
<li><a href="#Balancing-Reactive-and-Goal-Oriented-Behaviour" title="Balancing Reactive and Goal-Oriented Behaviour">Balancing Reactive and Goal-Oriented Behaviour</a></li>
<li><a href="#Other" title="Other">Other</a></li>
</ul>
</li>
<li><a href="#Environment-Properties" title="Environment Properties">Environment Properties</a><ul>
<li><a href="#Accessible-vs-Inaccessible" title="Accessible vs. Inaccessible">Accessible vs. Inaccessible</a></li>
<li><a href="#Deterministic-vs-non-Deterministic" title="Deterministic vs. non-Deterministic">Deterministic vs. non-Deterministic</a></li>
<li><a href="#Episodic-vs-non-Episodic" title="Episodic vs. non-Episodic">Episodic vs. non-Episodic</a></li>
<li><a href="#Static-vs-Dynamic" title="Static vs. Dynamic">Static vs. Dynamic</a></li>
<li><a href="#Discrete-vs-Continuous" title="Discrete vs. Continuous">Discrete vs. Continuous</a></li>
</ul>
</li>
<li><a href="#Agent-Types" title="Agent Types">Agent Types</a><ul>
<li><a href="#Physical-Agents" title="Physical Agents">Physical Agents</a></li>
<li><a href="#Software-Agents" title="Software Agents">Software Agents</a></li>
</ul>
</li>
<li><a href="#Abstract-Architecture" title="Abstract Architecture">Abstract Architecture</a></li>
</ul>
</li>
</ul>
</span></p><hr><h2 id="Agent-Properties" data-id="Agent-Properties"><a class="anchor hidden-xs" href="#Agent-Properties" title="Agent-Properties"><span class="octicon octicon-link"></span></a><span>Agent Properties</span></h2><h3 id="Agent-Definitions" data-id="Agent-Definitions"><a class="anchor hidden-xs" href="#Agent-Definitions" title="Agent-Definitions"><span class="octicon octicon-link"></span></a><span>Agent Definitions</span></h3><blockquote>
<ul>
<li><span>Autonomous agents are computational systems that inhabit some </span><strong><span>complex dynamic environment</span></strong><span>, sense and </span><strong><span>act</span></strong><span> autonomously in this environment, and by doing so realize a set of </span><strong><span>goals or tasks</span></strong><span> for which they are designed.</span></li>
<li><span>An autonomous agent is a </span><strong><span>system situated within and a part of an environment that senses that environment and acts on it</span></strong><span>, over time, in pursuit of its </span><strong><span>own agenda</span></strong><span> and so as to affect what it senses in the future.</span></li>
</ul>
</blockquote><h3 id="Autonomy" data-id="Autonomy"><a class="anchor hidden-xs" href="#Autonomy" title="Autonomy"><span class="octicon octicon-link"></span></a><span>Autonomy</span></h3><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><span>An agent is a computer system capable of </span><strong><span>autonomous</span></strong><span> action in some environment in order to meet its design objectives. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><p><span>Usually the environment is </span><strong><span>complex</span></strong><span> and </span><strong><span>dynamic</span></strong><span>, and agents should interact with it in real time.</span><br>
<u><span>Main property</span></u><span>: </span><strong><span>Autonomy</span></strong><span> capable of acting independently, exhibiting control over their </span><strong><span>internal state</span></strong><span>.</span></p><p><img src="https://i.imgur.com/msjmjkL.png" alt="" loading="lazy"></p><h3 id="Flexibility" data-id="Flexibility"><a class="anchor hidden-xs" href="#Flexibility" title="Flexibility"><span class="octicon octicon-link"></span></a><span>Flexibility</span></h3><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><span>An intelligent agent is a computer system capable of </span><strong><span>flexible</span></strong><span> autonomous action in some environment. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><p><span>By flexible, we mean:</span></p><ul>
<li><span>Reactive (response capability).</span></li>
<li><span>Pro-active (taking initiative).</span></li>
<li><span>Social (interacting with others).</span></li>
</ul><h3 id="Reactivity" data-id="Reactivity"><a class="anchor hidden-xs" href="#Reactivity" title="Reactivity"><span class="octicon octicon-link"></span></a><span>Reactivity</span></h3><ul>
<li><span>A </span><strong><u><span>reactive system</span></u></strong><span> is one that maintains an ongoing interaction with its environment, and responds to changes that occur in it (in time for the response to be useful).</span></li>
<li><span>If a program’s environment is guaranteed to be fixed, the program need never worry about its own success or failure – program just executes blindly.</span>
<ul>
<li><span>Example of fixed environment: compiler.</span></li>
</ul>
</li>
<li><span>The real world is not like that: things change, </span><strong><span>information is incomplete</span></strong><span>. Many (most?) interesting environments are </span><strong><span>dynamic</span></strong><span>.</span></li>
<li><span>Software is hard to build for dynamic domains: program must take into account possibility of failure – </span><strong><span>ask itself whether it is worth executing!</span></strong></li>
</ul><h3 id="Proactivness" data-id="Proactivness"><a class="anchor hidden-xs" href="#Proactivness" title="Proactivness"><span class="octicon octicon-link"></span></a><span>Proactivness</span></h3><ul>
<li><u><strong><span>Pro-activeness</span></strong></u><span>: generating and attempting to achieve goals; not driven solely by events; </span><strong><span>taking the initiative</span></strong><span>.</span></li>
<li><span>Reacting to an environment is easy (stimulus → response rules), but we generally want agents to do things for us, hence </span><strong><span>goal directed behavior</span></strong><span>, </span><strong><span>recognizing opportunities.</span></strong></li>
</ul><h3 id="Social-Ability" data-id="Social-Ability"><a class="anchor hidden-xs" href="#Social-Ability" title="Social-Ability"><span class="octicon octicon-link"></span></a><span>Social Ability</span></h3><ul>
<li><strong><u><span>Social ability</span></u></strong><span> in agents is the ability to interact with other agents (and possibly humans) via some kind of </span><strong><span>agent-communication language</span></strong><span>, and perhaps cooperate with others.</span></li>
<li><span>The real world is a </span><strong><span>multi-agent</span></strong><span> environment: we cannot go around attempting to achieve goals without taking others into account.</span>
<ul>
<li><span>Some goals can only be achieved with the cooperation of others. Similarly for many computer environments: witness the Internet.</span></li>
</ul>
</li>
</ul><h3 id="Balancing-Reactive-and-Goal-Oriented-Behaviour" data-id="Balancing-Reactive-and-Goal-Oriented-Behaviour"><a class="anchor hidden-xs" href="#Balancing-Reactive-and-Goal-Oriented-Behaviour" title="Balancing-Reactive-and-Goal-Oriented-Behaviour"><span class="octicon octicon-link"></span></a><span>Balancing Reactive and Goal-Oriented Behaviour</span></h3><p><span>These two considerations can be at odds with one another:</span></p><ul>
<li><span>We want our agents to be reactive, responding to changing conditions in an appropriate (timely) fashion.</span></li>
<li><span>We want our agents to systematically work towards longterm goals.</span></li>
</ul><blockquote style="border-left-color: rgb(255, 0, 0);">
<p><strong><span>Reactiveness vs. Deliberation balance</span></strong><br>
<span>Designing an agent that can balance reactiveness and deliberation (reason about long term goals) remains an openresearch problem. </span><span class="color" data-color="#ff0000"></span></p>
</blockquote><h3 id="Other" data-id="Other"><a class="anchor hidden-xs" href="#Other" title="Other"><span class="octicon octicon-link"></span></a><span>Other</span></h3><p><span>(Desireable, not mandatory)</span></p><ul>
<li><strong><span>Mobility</span></strong><span>: the ability of an agent to move around an electronic network.</span></li>
<li><strong><span>Veracity</span></strong><span>: an agent will not knowingly communicate false information</span></li>
<li><strong><span>Benevolence</span></strong><span>: agents do not have conflicting goals, and that every agent will therefore always try to do what is asked of it.</span></li>
<li><strong><span>Rationality</span></strong><span>: agent will act in order to achieve its goals, and will not act in such a way as to prevent its goals being achieved — at least insofar as its beliefs permit.</span></li>
<li><strong><span>Learning/Adaption</span></strong><span>: agents improve performance over time.</span></li>
</ul><hr><h2 id="Environment-Properties" data-id="Environment-Properties"><a class="anchor hidden-xs" href="#Environment-Properties" title="Environment-Properties"><span class="octicon octicon-link"></span></a><span>Environment Properties</span></h2><h3 id="Accessible-vs-Inaccessible" data-id="Accessible-vs-Inaccessible"><a class="anchor hidden-xs" href="#Accessible-vs-Inaccessible" title="Accessible-vs-Inaccessible"><span class="octicon octicon-link"></span></a><span>Accessible vs. Inaccessible</span></h3><ul>
<li><span>An </span><strong><u><span>accessible environment</span></u></strong><span> is one in which the agent can obtain complete, accurate, up-to-date information about the environment’s state (the environment is </span><strong><span>fully observable</span></strong><span>).</span></li>
<li><span>Most moderately complex environments (including, for example, the everyday physical world and the Internet) are </span><strong><u><span>inaccessible</span></u></strong><span> (or </span><strong><span>partially observable</span></strong><span>).</span></li>
<li><span>The more accessible an environment is, the simpler it is to build agents to operate in it.</span></li>
</ul><h3 id="Deterministic-vs-non-Deterministic" data-id="Deterministic-vs-non-Deterministic"><a class="anchor hidden-xs" href="#Deterministic-vs-non-Deterministic" title="Deterministic-vs-non-Deterministic"><span class="octicon octicon-link"></span></a><span>Deterministic vs. non-Deterministic</span></h3><ul>
<li><span>A </span><strong><u><span>deterministic environment</span></u></strong><span> is one in which any action has a single guaranteed effect — there is no uncertainty about the state that will result from performing an action.</span>
<ul>
<li><span>If the environment is deterministic except for the actions of other agents, then the environment can be defined as </span><strong><span>strategic</span></strong><span>.</span></li>
</ul>
</li>
<li><span>The physical world can to all intents and purposes be regarded as </span><strong><u><span>non-deterministic (or stochastic)</span></u></strong><span> Non-deterministic environments present greater problems for the agent designer.</span></li>
</ul><h3 id="Episodic-vs-non-Episodic" data-id="Episodic-vs-non-Episodic"><a class="anchor hidden-xs" href="#Episodic-vs-non-Episodic" title="Episodic-vs-non-Episodic"><span class="octicon octicon-link"></span></a><span>Episodic vs. non-Episodic</span></h3><ul>
<li><span>In an </span><strong><u><span>episodic environment</span></u></strong><span>, the performance of an agent is dependent on a number of discrete episodes, with </span><strong><span>no link</span></strong><span> between an agent’s performance in different scenarios.</span>
<ul>
<li><span>Episodic environments are simpler from the agent developer’s perspective because the agent can decide what action to perform based </span><strong><span>only on the current episode</span></strong><span> — it need not reason about the interactions between this and future episodes.</span></li>
</ul>
</li>
</ul><h3 id="Static-vs-Dynamic" data-id="Static-vs-Dynamic"><a class="anchor hidden-xs" href="#Static-vs-Dynamic" title="Static-vs-Dynamic"><span class="octicon octicon-link"></span></a><span>Static vs. Dynamic</span></h3><ul>
<li><span>A </span><strong><u><span>static environment</span></u></strong><span> is one that can be assumed to remain </span><strong><span>unchanged</span></strong><span> except by the performance of actions by the agent.</span></li>
<li><span>A </span><strong><u><span>dynamic environment</span></u></strong><span> is one that has </span><strong><span>other processes operating on it</span></strong><span>, and which hence changes in ways beyond the agent’s control. Other processes can interfere with the agent’s actions (as in concurrent systems theory).</span></li>
<li><span>The physical world is a highly dynamic environment.</span></li>
</ul><h3 id="Discrete-vs-Continuous" data-id="Discrete-vs-Continuous"><a class="anchor hidden-xs" href="#Discrete-vs-Continuous" title="Discrete-vs-Continuous"><span class="octicon octicon-link"></span></a><span>Discrete vs. Continuous</span></h3><ul>
<li><span>An </span><strong><u><span>environment is discrete</span></u></strong><span> if there are a </span><strong><span>fixed, finite number of actions and percepts</span></strong><span> in it.</span>
<ul>
<li><span>Discrete environments could </span><strong><span>in principle</span></strong><span> be handled by a kind of </span><strong><span>lookup table</span></strong><span>.</span></li>
</ul>
</li>
<li><span>Continuous environments have a certain level of mismatch with computer systems.</span></li>
<li><span>Russell and Norvig give a chess game as an example of a discrete environment, and taxi driving as an example of a continuous one.</span></li>
</ul><hr><h2 id="Agent-Types" data-id="Agent-Types"><a class="anchor hidden-xs" href="#Agent-Types" title="Agent-Types"><span class="octicon octicon-link"></span></a><span>Agent Types</span></h2><h3 id="Physical-Agents" data-id="Physical-Agents"><a class="anchor hidden-xs" href="#Physical-Agents" title="Physical-Agents"><span class="octicon octicon-link"></span></a><span>Physical Agents</span></h3><ul>
<li><span>Physical agents or embodied agents: Interact with real world (sensors, actuators connected to real world).</span></li>
<li><span>Problems of perception and action.</span></li>
<li><span>Best known example: Robots.</span></li>
</ul><h3 id="Software-Agents" data-id="Software-Agents"><a class="anchor hidden-xs" href="#Software-Agents" title="Software-Agents"><span class="octicon octicon-link"></span></a><span>Software Agents</span></h3><ul>
<li><span>Software agents’ environment is a virtual one: single machine, intranet, internet.</span>
<ul>
<li><span>Interact with other software agents, with software modules, services.</span></li>
<li><span>Interact with humans through human interfaces.</span></li>
</ul>
</li>
<li><span>Types of software agents:</span>
<ul>
<li><strong><span>Internet agents</span></strong><span> search and information extraction/management from Internet.</span></li>
<li><strong><span>Collaborative</span></strong><span> agents they coordinate with other agents to solve a common task.</span>
<ul>
<li><span>To solve problems too complex for a single agent.</span></li>
<li><span>To solve problems distributed in nature.</span></li>
<li><span>To interconnect already existing, heterogeneous systems (→ </span><strong><span>Agentification</span></strong><span>).</span></li>
</ul>
</li>
<li><strong><span>Interface agents</span></strong><span> they collaborate with a human user to solve a task, or to act on behalf of the user.</span></li>
<li><strong><span>Mobile SW agents</span></strong><span> they can move from one computer to another.</span></li>
</ul>
</li>
</ul><hr><h2 id="Abstract-Architecture" data-id="Abstract-Architecture"><a class="anchor hidden-xs" href="#Abstract-Architecture" title="Abstract-Architecture"><span class="octicon octicon-link"></span></a><span>Abstract Architecture</span></h2><ul>
<li><span>Internal architecture:</span>
<ul>
<li><span>Purely Reactive Agents (with no internal state).</span></li>
<li><span>Reactive Agents with internal state.</span></li>
<li><span>Delliberative Agents (goal-oriented behaviour).</span></li>
<li><span>Hybrid Agents (combine reactive and delliberative behaviour).</span></li>
</ul>
</li>
<li><em><span>Example</span></em><span>: A Multi-Agent System (Trading Agent Competition)!</span></li>
</ul><p><img src="./../images/chapter2/chapter2image1.png" alt="" loading="lazy"></p></div>
    <div class="ui-toc dropup unselectable hidden-print" style="display:none;">
        <div class="pull-right dropdown">
            <a id="tocLabel" class="ui-toc-label btn btn-default" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false" title="Table of content">
                <i class="fa fa-bars"></i>
            </a>
            <ul id="ui-toc" class="ui-toc-dropdown dropdown-menu" aria-labelledby="tocLabel">
                <div class="toc"><ul class="nav">

</html>
