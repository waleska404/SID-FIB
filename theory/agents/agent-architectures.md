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
    <div id="doc" class="markdown-body container-fluid comment-enabled" data-hard-breaks="true"><h1 id="Agent-Architectures" data-id="Agent-Architectures"><a class="anchor hidden-xs" href="#Agent-Architectures" title="Agent-Architectures"><span class="octicon octicon-link"></span></a><span>Agent Architectures</span></h1><h6 id="tags-SID-teo" data-id="tags-SID-teo"><a class="anchor hidden-xs" href="#tags-SID-teo" title="tags-SID-teo"><span class="octicon octicon-link"></span></a><span>tags: </span><code>SID-teo</code></h6><p><span class="toc"><ul>
<li><a href="#Abstract-Architecture-for-Agents" title="Abstract Architecture for Agents">Abstract Architecture for Agents</a><ul>
<li><a href="#Reactive-Agents" title="Reactive Agents">Reactive Agents</a></li>
<li><a href="#Purely-Reactive-Agents" title="Purely Reactive Agents">Purely Reactive Agents</a></li>
<li><a href="#Reactive-Agents-with-Internal-State" title="Reactive Agents with Internal State">Reactive Agents with Internal State</a></li>
<li><a href="#AdvantagesDisadvantages-of-Reactive-Agents" title="Advantages/Disadvantages of Reactive Agents">Advantages/Disadvantages of Reactive Agents</a></li>
<li><a href="#Situated-Automata-Components-RULER-and-GAPPS" title="Situated Automata Components: RULER and GAPPS">Situated Automata Components: RULER and GAPPS</a></li>
<li><a href="#Delliberative-Agents-with-expected-utilities" title="Delliberative Agents (with expected utilities)">Delliberative Agents (with expected utilities)</a></li>
<li><a href="#Delliberative-Agents-with-explicit-goals" title="Delliberative Agents (with explicit goals)">Delliberative Agents (with explicit goals)</a></li>
<li><a href="#Agents’-Interactions" title="Agents’ Interactions">Agents’ Interactions</a></li>
</ul>
</li>
<li><a href="#Architectures-for-Multiagent-Systems" title="Architectures for Multiagent Systems">Architectures for Multiagent Systems</a><ul>
<li><a href="#MAS---many-agents-in-the-same-environment" title="MAS - many agents in the same environment">MAS - many agents in the same environment</a></li>
<li><a href="#Agent-Platform" title="Agent Platform">Agent Platform</a></li>
<li><a href="#Components-of-an-Agent-Platform" title="Components of an Agent Platform">Components of an Agent Platform</a></li>
<li><a href="#Communication-methods" title="Communication methods">Communication methods</a></li>
<li><a href="#FIPA-Architecture-for-Agent-Platforms" title="FIPA Architecture for Agent Platforms">FIPA Architecture for Agent Platforms</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</span></p><hr><h2 id="Abstract-Architecture-for-Agents" data-id="Abstract-Architecture-for-Agents"><a class="anchor hidden-xs" href="#Abstract-Architecture-for-Agents" title="Abstract-Architecture-for-Agents"><span class="octicon octicon-link"></span></a><span>Abstract Architecture for Agents</span></h2><ul>
<li><span>An </span><u><span>agent architecture</span></u><span> proposes a particular </span><strong><span>methodology for building an autonomous agent.</span></strong></li>
<li><span>How the construction of the agent can be decomposed into the construction of a set of </span><strong><span>component modules</span></strong><span>.</span>
<ul>
<li><span>How these modules should be made to </span><strong><span>interact</span></strong><span>.</span></li>
</ul>
</li>
<li><span>These two aspects define how the </span><strong><span>sensor data</span></strong><span> and the </span><strong><span>current internal state</span></strong><span> of the agent determine the </span><strong><span>actions</span></strong><span> (effector outputs) and future internal state of the agent.</span></li>
</ul><h3 id="Reactive-Agents" data-id="Reactive-Agents"><a class="anchor hidden-xs" href="#Reactive-Agents" title="Reactive-Agents"><span class="octicon octicon-link"></span></a><span>Reactive Agents</span></h3><ul>
<li><span>Simple processing units that perceive and react to changes in their environment.</span></li>
<li><span>Do not have a symbolic representation of the world and do not use complex symbolic reasoning.</span></li>
<li><span>The advocates of reactive agent systems claims that intelligence is not a property of the active entity but it is distributed in the system, and steams as the result of the interaction between the many entities of the distributed structure and the environment.</span></li>
</ul><h3 id="Purely-Reactive-Agents" data-id="Purely-Reactive-Agents"><a class="anchor hidden-xs" href="#Purely-Reactive-Agents" title="Purely-Reactive-Agents"><span class="octicon octicon-link"></span></a><span>Purely Reactive Agents</span></h3><ul>
<li><u><span>Purely reactive agents</span></u><span>: agents that decide what to do without reference to their  history — they </span><strong><span>base their decision making entirely on the present</span></strong><span>, with no reference at all to the past.</span></li>
</ul><p><img src="./../images/agents/architectures/1.png" alt="" loading="lazy"></p><p><img src="./../images/agents/architectures/2.png" alt="" loading="lazy"></p><h3 id="Reactive-Agents-with-Internal-State" data-id="Reactive-Agents-with-Internal-State"><a class="anchor hidden-xs" href="#Reactive-Agents-with-Internal-State" title="Reactive-Agents-with-Internal-State"><span class="octicon octicon-link"></span></a><span>Reactive Agents with Internal State</span></h3><p><img src="./../images/agents/architectures/3.png" alt="" loading="lazy"></p><p><img src="./../images/agents/architectures/4.png" alt="" loading="lazy"></p><h3 id="AdvantagesDisadvantages-of-Reactive-Agents" data-id="AdvantagesDisadvantages-of-Reactive-Agents"><a class="anchor hidden-xs" href="#AdvantagesDisadvantages-of-Reactive-Agents" title="AdvantagesDisadvantages-of-Reactive-Agents"><span class="octicon octicon-link"></span></a><span>Advantages/Disadvantages of Reactive Agents</span></h3><ul>
<li>
<p><u><span>Advantages:</span></u></p>
<ul>
<li><strong><span>Simplicity</span></strong><span> of individual agents.</span></li>
<li><strong><span>Flexibility</span></strong><span>, adaptability: Ideal in very dynamic and unpredictable environments.</span></li>
<li><strong><span>Computational tractability</span></strong><span>: Avoiding complex planning/reasoning. Avoiding continuous model update.</span></li>
<li><strong><span>Robustness</span></strong><span> against failure: No central planning component (e.g. ant colony).</span></li>
<li><strong><span>Elegance</span></strong><span>.</span></li>
</ul>
</li>
<li>
<p><u><span>Disadvantages:</span></u></p>
<ul>
<li><strong><span>Need for sufficient information</span></strong><span> from the local environment.</span></li>
<li><span>Unclear how to incorporate </span><strong><span>non-local information</span></strong><span>.</span></li>
<li><strong><span>No long-term planning</span></strong><span> or replanning capabilities.</span></li>
<li><strong><span>Applicability is limited</span></strong><span>.</span></li>
<li><span>Difficult to make reactive agents that </span><strong><span>learn</span></strong><span>.</span></li>
<li><span>Interactions with the environment can have </span><strong><span>unpredictable long-term consequences</span></strong><span>. Dynamics of interaction can become too complex to understand.</span></li>
</ul>
</li>
</ul><h3 id="Situated-Automata-Components-RULER-and-GAPPS" data-id="Situated-Automata-Components-RULER-and-GAPPS"><a class="anchor hidden-xs" href="#Situated-Automata-Components-RULER-and-GAPPS" title="Situated-Automata-Components-RULER-and-GAPPS"><span class="octicon octicon-link"></span></a><span>Situated Automata Components: RULER and GAPPS</span></h3><ul>
<li>
<p><span>An agent is specified in terms of two components: </span><strong><span>perception</span></strong><span> and </span><strong><span>action</span></strong><span>. Two programs are then used to synthesize agents:</span></p>
<ul>
<li><strong><span>RULER</span></strong><span> is used to specify the </span><u><span>perception component</span></u><span> of an agent.</span></li>
<li><strong><span>GAPPS</span></strong><span> is used to specify the </span><u><span>action component</span></u><span>.</span></li>
</ul>
</li>
<li>
<p><strong><u><span>RULER</span></u><span>:</span></strong></p>
<ul>
<li><span>RULER takes as its input three components:</span><br>
<strong><span>1.</span></strong><span> The </span><strong><span>semantics</span></strong><span> of the agent’s inputs (‘whenever bit 1 is on, it is raining’).</span><br>
<strong><span>2.</span></strong><span> A set of </span><strong><span>static facts</span></strong><span> (‘whenever it is raining, the ground is wet’).</span><br>
<strong><span>3.</span></strong><span> A specification of the </span><strong><span>state transitions of the world</span></strong><span> (‘if the ground is wet, it stays wet until the sun comes out’).</span></li>
<li><span>The programmer then specifies the </span><u><span>desired semantics for the output</span></u><span> (‘if this bit is on, the ground is wet’).</span></li>
<li><span>The compiler designs a circuit whose output will have the correct semantics.</span></li>
</ul>
</li>
<li>
<p><strong><u><span>GAPPS</span></u><span>:</span></strong></p>
<ul>
<li><span>GAPPS program takes as its input:</span><br>
<strong><span>1.</span></strong><span> A set of </span><strong><span>goal reduction rules</span></strong><span>: Rules that encode information about how goals can be achieved in a given state.</span><br>
<strong><span>2.</span></strong><span> A </span><strong><span>top level goal</span></strong><span>.</span></li>
<li><span>Then it generates a program that can be translated into a digital circuit in order to realize the goal.</span></li>
<li><span>The generated circuit does not represent or manipulate symbolic expressions; all symbolic manipulation is done at compile time.</span></li>
</ul>
</li>
</ul><h4 id="From-perception-to-action" data-id="From-perception-to-action"><a class="anchor hidden-xs" href="#From-perception-to-action" title="From-perception-to-action"><span class="octicon octicon-link"></span></a><span>From perception to action</span></h4><p><img src="./../images/agents/architectures/5.png" alt="" loading="lazy"></p><h3 id="Delliberative-Agents-with-expected-utilities" data-id="Delliberative-Agents-with-expected-utilities"><a class="anchor hidden-xs" href="#Delliberative-Agents-with-expected-utilities" title="Delliberative-Agents-with-expected-utilities"><span class="octicon octicon-link"></span></a><span>Delliberative Agents (with expected utilities)</span></h3><ul>
<li><span>We build agents in order to carry out tasks for us. The task must be specified by us… But we want to </span><strong><span>tell agents what to do without telling them how to do it</span></strong><span>.</span></li>
<li><span>One possibility: </span><strong><span>associate utilities with individual states</span></strong><span> — the task of the agent is then to bring about states that maximize utility.</span></li>
<li><strong><u><span>Utility Functions over States</span></u><span>:</span></strong>
<ul>
<li><span>A task specification is a function </span><code>u : E → #</code><span> which associates a </span><strong><span>real number with every environment state</span></strong><span>.</span></li>
<li><span>But what is the value of a </span><strong><span>run</span></strong><span>…</span>
<ul>
<li><span>minimum utility of state on run?</span></li>
<li><span>maximum utility of state on run?</span></li>
<li><span>sum of utilities of states on run?</span></li>
<li><span>average?</span></li>
</ul>
</li>
<li><strong><span>Disadvantage</span></strong><span>: difficult to specify a </span><strong><span>long term</span></strong><span> view when assigning utilities to individual states (One possibility: a </span><strong><span>discount</span></strong><span> for states later on).</span></li>
</ul>
</li>
<li><strong><u><span>Utilities over Runs</span></u><span>:</span></strong>
<ul>
<li><span>Another possibility: </span><code>u : R → #</code><span> </span><strong><span>assigning a utilities to a runs</span></strong><span>, instead of assigning them to individual states.</span></li>
<li><span>Such an approach takes an inherently </span><strong><span>long term view</span></strong><span>.</span></li>
<li><span>Other variations: incorporate probabilities of different states emerging.</span></li>
<li><strong><span>Difficulties</span></strong><span> with utility-based approaches:</span>
<ul>
<li><span>where do the numbers come from?</span></li>
<li><span>we (normally?) do not think in terms of utilities!</span></li>
<li><span>hard to formulate tasks in these terms.</span></li>
</ul>
</li>
</ul>
</li>
</ul><p><img src="./../images/agents/architectures/6.png" alt="" loading="lazy"></p><h3 id="Delliberative-Agents-with-explicit-goals" data-id="Delliberative-Agents-with-explicit-goals"><a class="anchor hidden-xs" href="#Delliberative-Agents-with-explicit-goals" title="Delliberative-Agents-with-explicit-goals"><span class="octicon octicon-link"></span></a><span>Delliberative Agents (with explicit goals)</span></h3><p><img src="./../images/agents/architectures/7.png" alt="" loading="lazy"><br>
<img src="./../images/agents/architectures/8.png" alt="" loading="lazy"></p><h3 id="Agents’-Interactions" data-id="Agents’-Interactions"><a class="anchor hidden-xs" href="#Agents’-Interactions" title="Agents’-Interactions"><span class="octicon octicon-link"></span></a><span>Agents’ Interactions</span></h3><ul>
<li><span>Interaction between agents is </span><strong><span>unavoidable</span></strong><span>.</span>
<ul>
<li><span>To achieve </span><strong><span>own goals</span></strong><span>.</span></li>
<li><span>To manage </span><strong><span>interdependencies</span></strong><span>.</span></li>
</ul>
</li>
<li><span>It should occur at </span><strong><span>Knowledge-level</span></strong><span>.</span>
<ul>
<li><span>Which goals?, When?, Who executes what?</span></li>
</ul>
</li>
<li><strong><span>Flexibility</span></strong><span> to start and to give answers.</span>
<ul>
<li><strong><span>Asynchronous</span></strong><span> communication.</span></li>
<li><span>Need for </span><strong><span>languages and protocols</span></strong><span>.</span></li>
</ul>
</li>
</ul><blockquote style="border-left-color: rgb(255, 0, 0);">
<p><span>This implies a radical change in the way programs usually interact.</span><span class="color" data-color="#ff0000"></span></p>
</blockquote><hr><h2 id="Architectures-for-Multiagent-Systems" data-id="Architectures-for-Multiagent-Systems"><a class="anchor hidden-xs" href="#Architectures-for-Multiagent-Systems" title="Architectures-for-Multiagent-Systems"><span class="octicon octicon-link"></span></a><span>Architectures for Multiagent Systems</span></h2><h3 id="MAS---many-agents-in-the-same-environment" data-id="MAS---many-agents-in-the-same-environment"><a class="anchor hidden-xs" href="#MAS---many-agents-in-the-same-environment" title="MAS---many-agents-in-the-same-environment"><span class="octicon octicon-link"></span></a><span>MAS - many agents in the same environment</span></h3><p><span>Interactions among agents. Interactions for: High-level interactions, Coordination, Communication and Organization.</span></p><ul>
<li><strong><span>Coordination</span></strong>
<ul>
<li><span>Collectively motivated / interested</span>
<ul>
<li><span>own goals / coalition</span></li>
</ul>
</li>
<li><span>Self interested</span>
<ul>
<li><span>own goals / indifferent</span></li>
<li><span>own goals / competition / competing for the same resources</span></li>
<li><span>own goals / competition / contradictory goals</span></li>
</ul>
</li>
</ul>
</li>
<li><strong><span>Communication</span></strong>
<ul>
<li><span>Communication protocol</span>
<ul>
<li><span>negotiation to reach agreement</span></li>
</ul>
</li>
<li><span>Communication language</span>
<ul>
<li><span>ontologies</span></li>
</ul>
</li>
</ul>
</li>
<li><strong><span>Organizational structures</span></strong>
<ul>
<li><span>centralized vs decentralized</span></li>
<li><span>hierarchical/markets</span></li>
</ul>
</li>
</ul><h3 id="Agent-Platform" data-id="Agent-Platform"><a class="anchor hidden-xs" href="#Agent-Platform" title="Agent-Platform"><span class="octicon octicon-link"></span></a><span>Agent Platform</span></h3><ul>
<li><span>Agents in a multiagent system tend to interact through a </span><strong><span>middleware layer</span></strong><span>.</span></li>
<li><span>This middleware provides connectivity between agents, solving low-level connectivity issues: Communication methods.</span></li>
<li><span>Sometimes this middleware is called </span><strong><span>agent platform</span></strong><span>.</span></li>
<li><span>Agent Platform </span><strong><span>tasks</span></strong><span>:</span>
<ul>
<li><span>Suspend temporally an agent execution</span></li>
<li><span>Stop an agent execution.</span></li>
<li><span>Resume/continue agent execution.</span></li>
<li><span>Start an agent.</span></li>
<li><span>Platform resource management.</span></li>
</ul>
</li>
</ul><h3 id="Components-of-an-Agent-Platform" data-id="Components-of-an-Agent-Platform"><a class="anchor hidden-xs" href="#Components-of-an-Agent-Platform" title="Components-of-an-Agent-Platform"><span class="octicon octicon-link"></span></a><span>Components of an Agent Platform</span></h3><ul>
<li><strong><span>Agent</span></strong><span>: a program providing a list of services.</span></li>
<li><strong><span>Directory Facilitator (DF)</span></strong><span> is an agent which provides a Yellow Pages service within the platform </span><u><span>(knows the services that agents within the platform provide)</span></u><span>.</span>
<ul>
<li><u><span>register, deregister, modify, search</span></u></li>
</ul>
</li>
<li><strong><span>Agent Management System (AMS)</span></strong><span> is an agent controlling access and usage of the agent platform. It knows the platform and agents’ </span><strong><span>addresses</span></strong><span> and provides a White Pages service (knows the routing addresses for agents within and in other platforms).</span></li>
<li><strong><span>Message Transport Service (MTS)</span></strong><span> is used to enable communication between agents in different platforms.</span></li>
</ul><h3 id="Communication-methods" data-id="Communication-methods"><a class="anchor hidden-xs" href="#Communication-methods" title="Communication-methods"><span class="octicon octicon-link"></span></a><span>Communication methods</span></h3><ul>
<li><strong><span>Blackboard systems</span></strong>
<ul>
<li><span>Agents communicate information through a common data structure, accessible by everybody.</span></li>
<li><span>Problem: if there is no middleware to provide some concurrency, it tends to become a bottleneck.</span></li>
</ul>
</li>
<li><strong><span>Message passing</span></strong>
<ul>
<li><span>Agents communicate directly by means of messages.</span></li>
<li><span>The agent platform usually acts as message router.</span></li>
<li><span>Common communication language (e.g. </span><strong><span>FIPA-ACL</span></strong><span>).</span></li>
<li><span>Common communication protocols (message format, steps in a communication).</span></li>
</ul>
</li>
</ul><h3 id="FIPA-Architecture-for-Agent-Platforms" data-id="FIPA-Architecture-for-Agent-Platforms"><a class="anchor hidden-xs" href="#FIPA-Architecture-for-Agent-Platforms" title="FIPA-Architecture-for-Agent-Platforms"><span class="octicon octicon-link"></span></a><span>FIPA Architecture for Agent Platforms</span></h3><p><img src="./../images/agents/architectures/9.png" alt="" loading="lazy"></p></div>
    <div class="ui-toc dropup unselectable hidden-print" style="display:none;">
        <div class="pull-right dropdown">
            <a id="tocLabel" class="ui-toc-label btn btn-default" data-toggle="dropdown" href="#" role="button" aria-haspopup="true" aria-expanded="false" title="Table of content">
                <i class="fa fa-bars"></i>
            </a>
            <ul id="ui-toc" class="ui-toc-dropdown dropdown-menu" aria-labelledby="tocLabel">
                <div class="toc"><ul class="nav">

</body>

</html>
