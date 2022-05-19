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
    <div id="doc" class="markdown-body container-fluid comment-enabled" data-hard-breaks="true"><h1 id="Introduction-to-Distributed-Intelligent-Agent-Systems" data-id="Introduction-to-Distributed-Intelligent-Agent-Systems"><a class="anchor hidden-xs" href="#Introduction-to-Distributed-Intelligent-Agent-Systems" title="Introduction-to-Distributed-Intelligent-Agent-Systems"><span class="octicon octicon-link"></span></a><span>Introduction to Distributed Intelligent Agent Systems</span></h1><h6 id="tags-SID-teo" data-id="tags-SID-teo"><a class="anchor hidden-xs" href="#tags-SID-teo" title="tags-SID-teo"><span class="octicon octicon-link"></span></a><span>tags: </span><code>SID-teo</code></h6><p><span class="toc"><ul>
<li><a href="#Introduction-to-Distributed-Intelligent-Agent-Systems" title="Introduction to Distributed Intelligent Agent Systems">Introduction to Distributed Intelligent Agent Systems</a><ul>
<li><a href="#Artificial-Intelligence" title="Artificial Intelligence">Artificial Intelligence</a></li>
<li><a href="#Cognitive-Architectures-I" title="Cognitive Architectures I">Cognitive Architectures I</a></li>
<li><a href="#Intelligent-Agent" title="Intelligent Agent">Intelligent Agent</a></li>
<li><a href="#Cognitive-AI-Paradigms" title="Cognitive AI Paradigms">Cognitive AI Paradigms</a></li>
<li><a href="#Cognitive-AI-Fundations" title="Cognitive AI Fundations">Cognitive AI Fundations</a><ul>
<li><a href="#George-Herbert-Mead-1863-1931-Mind-Self-and-Society" title="George Herbert Mead (1863-1931) Mind, Self, and Society">George Herbert Mead (1863-1931) Mind, Self, and Society</a></li>
</ul>
</li>
<li><a href="#MIND" title="MIND">MIND</a><ul>
<li><a href="#Analogy-An-ants-society" title="Analogy: An ants society">Analogy: An ants society</a></li>
<li><a href="#Stochastic-Neural-Analog-Reinforcement-Computer-SNARC-1951" title="Stochastic Neural Analog Reinforcement Computer (SNARC, 1951)">Stochastic Neural Analog Reinforcement Computer (SNARC, 1951)</a></li>
<li><a href="#Marvin-Minsky-The-Society-of-Mind" title="Marvin Minsky, The Society of Mind">Marvin Minsky, The Society of Mind</a></li>
</ul>
</li>
<li><a href="#Which-Kind-of-Cognitive-Architectures-are-we-Looking-for" title="Which Kind of Cognitive Architectures are we Looking for?">Which Kind of Cognitive Architectures are we Looking for?</a></li>
<li><a href="#Nature-of-the-Brain" title="Nature of the Brain">Nature of the Brain</a></li>
<li><a href="#Architectures-for-Reactive-Systems" title="Architectures for Reactive Systems">Architectures for Reactive Systems</a></li>
<li><a href="#Cognitive-Architectures-II" title="Cognitive Architectures II">Cognitive Architectures II</a><ul>
<li><a href="#Parameters" title="Parameters">Parameters</a></li>
<li><a href="#Open-issues" title="Open issues">Open issues</a></li>
<li><a href="#Functional-aspects" title="Functional aspects">Functional aspects</a></li>
</ul>
</li>
<li><a href="#Rational-Decisions" title="Rational Decisions">Rational Decisions</a></li>
</ul>
</li>
</ul>
</span></p><hr><h2 id="Artificial-Intelligence" data-id="Artificial-Intelligence"><a class="anchor hidden-xs" href="#Artificial-Intelligence" title="Artificial-Intelligence"><span class="octicon octicon-link"></span></a><span>Artificial Intelligence</span></h2><ul>
<li>
<p><span>Too many definitions:</span></p>
<blockquote style="border-left-color: rgb(55, 185, 191);">
<p><span>The theory and development of computer systems able to perform tasks normally requiring human intelligence, such as visual perception, speech recognition, decision-making, and translation between languages. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></p>
</blockquote>
<blockquote style="border-left-color: rgb(55, 185, 191);">
<p><span>Artificial intelligence is the ability of a digital computer or computer-controlled robot to perform tasks commonly associated with intelligent beings.</span><br><br><span>The term is frequently applied to the project of developing systems endowed with the intellectual processes characteristic of humans, such as the ability to reason, discover meaning, generalize, or learn from past experience. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></p>
</blockquote>
<blockquote style="border-left-color: rgb(55, 185, 191);">
<p><span>“Artificial intelligence (AI) refers to systems that display intelligent behaviour by analysing their environment and taking actions – with some degree of autonomy – to achieve specific goals." </span><em><span>-European Commission’s Communication on AI</span></em><span> </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></p>
</blockquote>
<blockquote style="border-left-color: rgb(55, 185, 191);">
<p><span>Artificial intelligence (AI) systems are software (and possibly also hardware) systems designed by humans that, given a complex goal, </span><strong><span>act in the physical or digital dimension by perceiving their environment through data acquisition</span></strong><span>, interpreting the collected structured or unstructured data, reasoning on the knowledge, or processing the information, derived from this data and </span><strong><span>deciding the best action(s) to take to achieve the given goal.</span></strong><span> AI systems can either use </span><strong><span>symbolic rules or learn a numeric model</span></strong><span>, and they can also adapt their behaviour by analysing how the environment is affected by their previous actions. </span><em><span>-(HLEG-AI)</span></em><span> </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></p>
</blockquote>
</li>
</ul><hr><h2 id="Cognitive-Architectures-I" data-id="Cognitive-Architectures-I"><a class="anchor hidden-xs" href="#Cognitive-Architectures-I" title="Cognitive-Architectures-I"><span class="octicon octicon-link"></span></a><span>Cognitive Architectures I</span></h2><ul>
<li><span>In this course we aim to have a </span><strong><span>holistic view</span></strong><span> of Artificial Intelligence: its methods, techniques, and how to combine them into intelligent systems.</span></li>
<li><span>But… what is an </span><strong><span>intelligent system</span></strong><span>?</span>
<ul>
<li><span>One way to characterize the behaviour we </span><strong><span>think</span></strong><span> as </span><em><strong><span>intelligence</span></strong></em><span> is through the study of the architectures providing such behaviour.</span></li>
</ul>
</li>
<li><span>We call </span><u><strong><span>Cognitive Architectures</span></strong></u><span> the ones that use </span><strong><span>symbols</span></strong><span> to represent the environment.</span>
<ul>
<li><u><span>Architectures</span></u><span> are described by the description of their foundations and the methods used to achieve an </span><em><strong><span>intelligent behaviour</span></strong></em><span>.</span></li>
<li><span>Cognitive architectures are based on computational entities, but this does not imply that intelligence should come always from the computer.</span></li>
<li><span>A metaphor typically used in Cognitive Architectures to cover both human and machine intelligence is the one of the </span><em><strong><span>intelligent agent</span></strong></em><span>.</span></li>
</ul>
</li>
</ul><hr><h2 id="Intelligent-Agent" data-id="Intelligent-Agent"><a class="anchor hidden-xs" href="#Intelligent-Agent" title="Intelligent-Agent"><span class="octicon octicon-link"></span></a><span>Intelligent Agent</span></h2><ul>
<li><u><span>An agent is a computer system capable of autonomous action in some environment in order to meet its design objectives.</span></u></li>
<li><span>An agent should be able to perceive and act in the environment.</span></li>
<li><span>Usually the environment is </span><em><strong><span>complex</span></strong></em><span> and </span><em><strong><span>dynamic</span></strong></em><span>, and agents should interact with it in real time.</span></li>
</ul><p><img src="./images/intro/1.png" alt="" loading="lazy"></p><hr><h2 id="Cognitive-AI-Paradigms" data-id="Cognitive-AI-Paradigms"><a class="anchor hidden-xs" href="#Cognitive-AI-Paradigms" title="Cognitive-AI-Paradigms"><span class="octicon octicon-link"></span></a><span>Cognitive AI Paradigms</span></h2><ul>
<li><span>In AI, paradigmas can be characterized by the metaphor used to model intelligence:</span>
<ul>
<li><span>Logics</span></li>
<li><span>Search in a State Space</span></li>
<li><span>Knowledge-Based (rules, patterns, experiences)</span></li>
<li><span>Evolutionary</span></li>
<li><span>Social</span></li>
</ul>
</li>
</ul><hr><h2 id="Cognitive-AI-Fundations" data-id="Cognitive-AI-Fundations"><a class="anchor hidden-xs" href="#Cognitive-AI-Fundations" title="Cognitive-AI-Fundations"><span class="octicon octicon-link"></span></a><span>Cognitive AI Fundations</span></h2><ul>
<li><span>PHILOSOPHY</span>
<ul>
<li><span>Can rules be used to extract valid conclusions? How mind emerges from the physical brain? Where does Knowledge come from? How can Knowledge lead to action?</span></li>
</ul>
</li>
<li><span>MATHEMATICS/LOGICS</span>
<ul>
<li><span>Which are the formal rules to extract valid conclusions? Which things are computable? How to reason with Knowledge that is uncertain and/or vague and/or incomplete?</span></li>
</ul>
</li>
<li><span>NEUROSCIENCES</span>
<ul>
<li><span>How is information processed by the brain?</span></li>
</ul>
</li>
<li><span>PSICOLOGY</span>
<ul>
<li><span>How do animals and humans think and act?</span></li>
</ul>
</li>
<li><span>SOCIOLOGY/ETOLOGY/ECONOMICS</span>
<ul>
<li><span>How collective (social/organizational) behaviour can be generated from individual (animal/human) behaviour?</span></li>
</ul>
</li>
<li><span>CONTROL THEORY</span>
<ul>
<li><span>How can self-controlled artifacts behave/act?</span></li>
</ul>
</li>
</ul><h3 id="George-Herbert-Mead-1863-1931-Mind-Self-and-Society" data-id="George-Herbert-Mead-1863-1931-Mind-Self-and-Society"><a class="anchor hidden-xs" href="#George-Herbert-Mead-1863-1931-Mind-Self-and-Society" title="George-Herbert-Mead-1863-1931-Mind-Self-and-Society"><span class="octicon octicon-link"></span></a><span>George Herbert Mead (1863-1931) Mind, Self, and Society</span></h3><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><span>The self is an object to itself.</span></li>
<li><span>The self is a social structure.</span></li>
<li><span>Self arises from social experience.</span></li>
<li><span>Self arises from language and interaction with others.</span></li>
<li><span>The conversation of gestures is the beginning of communication.</span></li>
<li><span>The inner conversation is the beginning of self (selfrealization). </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><span>One inevitably seeks communication with others.</span></li>
<li><span>Communication requires planning.</span></li>
<li><strong><span>Thinking</span></strong><span> becomes preparatory to social action.</span></li>
<li><span>The process of </span><strong><span>thinking is an inner conversation.</span></strong></li>
<li><u><span>Symbols are essential for communication and the development of the self.</span></u><span> </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><span>The </span><strong><span>complete self</span></strong><span> reflects the unity of the social process; and each of the elementary selves reflects the complete social process of self-reflection and interaction with others.</span></li>
<li><span>Stages of the development of the self:</span>
<ol>
<li><u><span>Play stage</span></u><span>: dyatic relationships.</span></li>
<li><u><span>Game stage</span></u><span>: multiple relationships.</span></li>
</ol>
</li>
<li><strong><span>Game playing</span></strong><span> requires a realization of the generalized other: assuming the statuses and roles of all involved. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><span>The self-conscious individual assumes the organized social attitudes of the social group.</span></li>
<li><span>The self is not so much a substance as a process, continually changing and adapting to social processes.</span></li>
<li><span>The </span><strong><span>“me”</span></strong><span> is the accumulated awareness of "</span><em><span>the generalized other.</span></em><span>”</span></li>
<li><span>The </span><strong><span>“I”</span></strong><span> is the more personal. It is the reflector or observer.</span></li>
<li><strong><span>The human mind arises solely through social experience.</span></strong><span> It represents the thinking process of internalized communication. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><hr><h2 id="MIND" data-id="MIND"><a class="anchor hidden-xs" href="#MIND" title="MIND"><span class="octicon octicon-link"></span></a><span>MIND</span></h2><ul>
<li><span>Motivation:</span>
<ul>
<li><span>What is human mind and how does it work? How do we recognize objects and scenes? How do we use words and languages? How do we achieve goals? How do we learn ? How does common sense work?</span></li>
</ul>
</li>
</ul><h3 id="Analogy-An-ants-society" data-id="Analogy-An-ants-society"><a class="anchor hidden-xs" href="#Analogy-An-ants-society" title="Analogy-An-ants-society"><span class="octicon octicon-link"></span></a><span>Analogy: An ants society</span></h3><ul>
<li><span>An individual ant is not very bright, but ants in a colony, operating as a collective, do remarkable things.</span></li>
</ul><blockquote style="border-left-color: rgb(55, 185, 191);">
<p><span>A single neuron in the human brain can respond only to what the neurons connected to it are doing, but all of them together can be Albert Einstein. </span><em><span>Deborah M. Gordon (Stanford University)</span></em><span> </span><span class="color" data-color="#37B9BF"></span></p>
</blockquote><ul>
<li><span>Some social systems in Nature can present an </span><em><span>intelligent collective behaviour</span></em><span> although they are composed by simple individuals.</span></li>
<li><span>The intelligent solutions to problems naturally emerge from the self-organization and </span><em><span>communication</span></em><span> of these individuals.</span>
<ul>
<li><span>Carrying large items, forming bridges, finding the shortest routes from the nest to a food source, prioritizing food sources based on their distance and ease of access…</span></li>
</ul>
</li>
<li><span>Individual ants are simple insects with </span><em><strong><span>limited</span></strong></em><span> memory and capable of performing </span><em><strong><span>simple</span></strong></em><span> actions. However, an ant colony expresses a </span><em><strong><span>complex</span></strong></em><span> collective behaviour.</span>
<ul>
<li><span>How do they know which task to perform? How can they manage to find the shortest path (Goal)? How did the Ants communicate with each other? How do they form such huge colonies?</span></li>
</ul>
</li>
<li><span>Ants have dealt with the same kind of questions which we have set out with.</span></li>
</ul><h3 id="Stochastic-Neural-Analog-Reinforcement-Computer-SNARC-1951" data-id="Stochastic-Neural-Analog-Reinforcement-Computer-SNARC-1951"><a class="anchor hidden-xs" href="#Stochastic-Neural-Analog-Reinforcement-Computer-SNARC-1951" title="Stochastic-Neural-Analog-Reinforcement-Computer-SNARC-1951"><span class="octicon octicon-link"></span></a><span>Stochastic Neural Analog Reinforcement Computer (SNARC, 1951)</span></h3><ul>
<li><u><span>Key idea</span></u><span>: producing machines which could learn by providing them with memory neurones connected to synapses; the machine would also have to possess past memory in order to function efficiently when faced with different situations.</span></li>
</ul><h3 id="Marvin-Minsky-The-Society-of-Mind" data-id="Marvin-Minsky-The-Society-of-Mind"><a class="anchor hidden-xs" href="#Marvin-Minsky-The-Society-of-Mind" title="Marvin-Minsky-The-Society-of-Mind"><span class="octicon octicon-link"></span></a><span>Marvin Minsky, The Society of Mind</span></h3><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><u><span>Background</span></u><span>: The functions performed by the brain are the products of the work of thousands of different, specialized sub-systems, the intricate product of hundreds of millions of years of biological evolution. We cannot hope to understand such an organization by emulating the techniques of those particle physicists who search for the simplest possible unifying conceptions. </span><strong><span>Constructing a mind is simply a different kind of problem</span></strong><span>—of how to synthesize organizational systems that can support a large enough diversity of different schemes, yet enable them to work together to exploit one another’s abilities. </span><em><span>[Minsky, M.: Logical vs. Analogical or Symbolic vs. Connectionist or Neat vs. Scruffy.]</span></em></li>
<li><u><span>Aim</span></u><span>: to create a theory of human cognition. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><u><span>Approach</span></u><span>: A Cognitive Architecture composed by thousands of individual agents.</span></li>
<li><u><span>Idea</span></u><span>: Human intelligence is built layer by layer from the interactions of simple parts called </span><strong><span>agents</span></strong><span>, which are themselves mindless.</span>
<ul>
<li><span>Theory covers processes </span><strong><span>such as language, memory, learning, consciousness, the sense of self, and free-will.</span></strong></li>
<li><span>Very flexible. Based on integration. Scalable.</span></li>
</ul>
</li>
<li><u><span>Point of view</span></u><span>: constructivist and organicist.</span></li>
<li><u><span>Technical perspective</span></u><span>: Parallelism, different types of Knowledge bases, compatibility between the symbolic and sub-symbolic levels. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</blockquote><blockquote style="border-left-color: rgb(55, 185, 191);">
<ul>
<li><u><span>The revolutionary proposal of The Society of Mind:</span></u>
<ul>
<li><span>It takes into account and tries to explain cognitive development.</span></li>
<li><span>It takes into account evolution.</span></li>
<li><span>It takes into account emotions.</span></li>
<li><span>Flexible behaviour depending on the environment.</span></li>
<li><span>Exhibiting some rationality. </span><span class="color fa fa-tag" data-color="#37B9BF" style="color: rgb(55, 185, 191);"></span></li>
</ul>
</li>
</ul>
</blockquote><hr><h2 id="Which-Kind-of-Cognitive-Architectures-are-we-Looking-for" data-id="Which-Kind-of-Cognitive-Architectures-are-we-Looking-for"><a class="anchor hidden-xs" href="#Which-Kind-of-Cognitive-Architectures-are-we-Looking-for" title="Which-Kind-of-Cognitive-Architectures-are-we-Looking-for"><span class="octicon octicon-link"></span></a><span>Which Kind of Cognitive Architectures are we Looking for?</span></h2><ul>
<li><span>Capable to operate in rich and complex environments.</span></li>
<li><span>Capable of using symbols and abstractions.</span></li>
<li><span>Use of natural and artificial languages.</span></li>
<li><span>Learn from the environment and the experience.</span></li>
<li><span>Get capabilities during execution time (adaptation).</span></li>
<li><span>Operate in an autonomous way, but being social.</span></li>
<li><span>Be self-conscious.</span></li>
<li><span>Be built from (artificial) neurons.</span></li>
<li><span>Emerge from evolution.</span></li>
</ul><hr><h2 id="Nature-of-the-Brain" data-id="Nature-of-the-Brain"><a class="anchor hidden-xs" href="#Nature-of-the-Brain" title="Nature-of-the-Brain"><span class="octicon octicon-link"></span></a><span>Nature of the Brain</span></h2><ul>
<li><span>Human minds are not perfect decision-makers, but by and large they are very good.</span></li>
<li><span>Brains are not as modular as software.</span></li>
<li><strong><span>Brains may are to </span><em><span>intelligence</span></em><span> as wings to </span><em><span>flying</span></em></strong><span>. Mimesis is not always the best idea.</span></li>
<li><span>Lessons learned: memory and simulation (planning) are good to decision making.</span></li>
</ul><hr><h2 id="Architectures-for-Reactive-Systems" data-id="Architectures-for-Reactive-Systems"><a class="anchor hidden-xs" href="#Architectures-for-Reactive-Systems" title="Architectures-for-Reactive-Systems"><span class="octicon octicon-link"></span></a><span>Architectures for Reactive Systems</span></h2><ul>
<li><span>These systems make decision at run time based on limited information and simple situation action rules.</span></li>
<li><span>These architectures were often called behaviour based, situated or reactive.</span></li>
<li><strong><span>Brooks with Subsumption architecture denied the need for symbolic representation of the world, instead the systems make their decisions based on the inputs.</span></strong></li>
<li><span>The decision of reactive architectures are partly guided by Simon’s hypothesis states that that the </span><em><span>complexity of the behaviour of the system can be a reflection of the complexity of the environment rather than the reflection of the system’s complex internal design.</span></em></li>
</ul><blockquote style="border-left-color: rgb(255, 191, 0);">
<p><strong><em><span>NOTE:</span></em></strong><span>  Cognitive architectures and neural networks are not the same. </span><span class="color" data-color="#FFBF00"></span></p>
</blockquote><hr><h2 id="Cognitive-Architectures-II" data-id="Cognitive-Architectures-II"><a class="anchor hidden-xs" href="#Cognitive-Architectures-II" title="Cognitive-Architectures-II"><span class="octicon octicon-link"></span></a><span>Cognitive Architectures II</span></h2><h3 id="Parameters" data-id="Parameters"><a class="anchor hidden-xs" href="#Parameters" title="Parameters"><span class="octicon octicon-link"></span></a><span>Parameters</span></h3><ul>
<li><span>Generality</span></li>
<li><span>Versatility</span></li>
<li><span>Rationality</span></li>
<li><span>Learning</span></li>
<li><span>Psychological Validation</span></li>
<li><span>Applicability</span></li>
<li><span>Scalability</span></li>
<li><span>Reactivity</span></li>
<li><span>Efficiency</span></li>
</ul><h3 id="Open-issues" data-id="Open-issues"><a class="anchor hidden-xs" href="#Open-issues" title="Open-issues"><span class="octicon octicon-link"></span></a><span>Open issues</span></h3><ul>
<li><span>Which is the best of all Architectures?</span></li>
<li><span>Will we ever get complete architectures?</span></li>
<li><span>Which kind of intelligence will we get?</span></li>
<li><span>How can agents solve problems?</span></li>
</ul><h3 id="Functional-aspects" data-id="Functional-aspects"><a class="anchor hidden-xs" href="#Functional-aspects" title="Functional-aspects"><span class="octicon octicon-link"></span></a><span>Functional aspects</span></h3><ul>
<li><span>Engineering methodology (how to develop them).</span></li>
<li><span>Capability to tackle a wide range of complex tasks.</span></li>
<li><span>Efficiency when acting on the environment.</span></li>
<li><span>Autonomy.</span></li>
</ul><hr><h2 id="Rational-Decisions" data-id="Rational-Decisions"><a class="anchor hidden-xs" href="#Rational-Decisions" title="Rational-Decisions"><span class="octicon octicon-link"></span></a><span>Rational Decisions</span></h2><ul>
<li><strong><span>Rational</span></strong><span>: maximally achieving pre-defined goals.</span></li>
<li><span>Rationality only concerns what decisions are made.</span></li>
<li><strong><span>Goals</span></strong><span> are expressed in terms of utility (of outcomes).</span></li>
</ul><figure>
<img src="./images/intro/2.png">
<figcaption><b>What kind of AI?</b></figcaption>
</figure><blockquote>
<p><em><span>I think the big problem is that we’re not smart enough to understand which of the problems we’re facing are good enough. Therefore, we have to build super intelligent machines like HAL.</span></em><span> -Marvin Minsky</span></p>
</blockquote></div>
    
</body>

</html>
