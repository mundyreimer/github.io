---
title: Notes on the Free Energy Principle
date: 2020-11-15 00:00:00
featured_image: '/images/post_pics/free_energy_principle/causality_book_cover.jpg'
excerpt: A collection of my thoughts, resources, and related ideas regarding the Free Energy Principle
---
*Updated: 2020-12-13*  
*Topics: [Biology](https://mundyreimer.github.io/archive), [Cognitive Science](https://mundyreimer.github.io/archive), [Physics](https://mundyreimer.github.io/archive), [Mathematics](https://mundyreimer.github.io/archive), [Philosophy](https://mundyreimer.github.io/archive), [History](https://mundyreimer.github.io/archive)*  
*Confidence: Uncertain*  
*Status: Still in progress* 

TL;DR - A collection of my thoughts, resources, and related ideas regarding the Free Energy Principle.  

I mainly work on this to help consolidate my memories and compile my evolving thoughts on the matter and catalog which resources I was influenced by.  Feel free to get in contact if I've missed something or you see an error somewhere.

---

## Motivation
- why care about the FEP
- Bring up intro to homeostasis & living systems, identity, maintain structural integrity within a limited range of configurations of the molecules and atoms that make up your body. What's important to note is that the number of possible configurations that are functional and work are very few when compared to the incredibly vast amount of combinatorial arrangements of molecules and atoms that don't (for instance, there are many more ways to be a puddle of molecular soup).  And why should a biological system like you stay in your configuration?  What gives that particular arrangement its structural integrity to *persist* through some arbitrary amount of time as a singular unit with *Identity* separate from the environment's molecules and atoms?  Why don't biological systems just disperse and dissipate into the environment as soon as the they are formed, like a wisp of smoke diffusing into nothing?

- who brings it up
    - bring up you first heard of the FEP in the context of Dr. Krichmar's cognitive robotics work at UCI
    - read Andy Clark's book
    - then bring up Scott's post here
    - then bring up some talk in the information and uncertainty group at UCBerkeley
    - then finally Mel Andrews stuff
- recent controversies
- Why it's famous and controversial now
    - Friston
    - What are all the fields that use it (see wikipedia)
        - Behavioral Psychology and generally the sciences surrounding *decision-making*. From [Friston](https://www.frontiersin.org/articles/10.3389/fpsyg.2013.00710/full):
        "...we look specifically at the normative implications for behavior in the context of classical (economic) decision-making problems. Our normative account argues that optimal decisions minimize the relative entropy between likely and desired outcomes. This means that—in some contexts—agents are compelled to seek novel states, whereas in other contexts they maximize expected utility. We hope to show that explorative behavior is not just in accordance with the principle of free energy minimization but is in fact mandated when minimizing surprise (or maximizing model-evidence) in the context of decision-making behavior. In brief, we argue that when a policy (i.e., an action selection rule that entails a sequence of actions) is selected—in a way that includes uncertainty about outcomes—there is necessarily an exploratory drive that accompanies the classical maximization of expected utility."

---

## Historical Background: The Origins of Teleology?

In tracing the origins of the FEP, a few people like Friston[3], Hohwy[5], and Andrews[6] make the connection between the Free Energy Principle and the [Principle of Maximum Entropy]((https://en.wikipedia.org/wiki/Principle_of_maximum_entropy)) by [E.T. Jaynes](https://en.wikipedia.org/wiki/Edwin_Thompson_Jaynes).

The former academics note that Jaynes took a very [scientific-materialist](https://en.wikipedia.org/wiki/Materialism) in origins, thermodynamic-based formalism and casted it into a more general, probabilistic theory of how we can arrive at some knowledge.  This was called the principle of maximum entropy and is a form of [Occam's Razor](https://en.wikipedia.org/wiki/Occam%27s_razor) when applied to the field of probability theory.  In the physics-based thermodynamics case, this acted as a preference for measuring the macroscopic variables of a system like the canonical pressure, temperature, and volume rather than a potentially vast number of underlying microscopic variables such as every particle's momentum, velocity, and kinetic energy, etc.  In the more general, *[epistemological](https://en.wikipedia.org/wiki/Epistemology)*, and probalistic interpretation by Jaynes, it states that we should strive to model the prior data using a probability distribution with the fewest number of assumptions than we have evidence for.  It is essentially a claim of epistemic modesty in that the "simplest explanation is usually the right one".  And indeed, this seems to be a principle that many scientists and statistical modelers put to use.[8]

It is key to note that the repurposing of this particular mathematical "simplification" apparatus or "minimization" formalism originating in the field of physics has not been isolated to Jaynes alone.  In fact, time and time again complex physical systems like those found in the field of thermodynamics with a vast number of interacting particles have been difficult to model using only classical [Newtonian mechanics](https://en.wikipedia.org/wiki/Classical_mechanics) due to the mathematics getting rather calculation heavy, sometimes even intractably so.  One of my favorite scientists of all time, German physicist and physician, [Hermann von Helmholtz](https://en.wikipedia.org/wiki/Hermann_von_Helmholtz) originally conceptualized in his 1881 lecture, *"On the thermodynamics of chemical processes"*, something called the thermodynamic potential that measures the useful work obtainable from a closed thermodynamic system at constant temperature and volume, which later became known as [Helmholtz free energy](https://en.wikipedia.org/wiki/Helmholtz_free_energy) (whereas a closely associated [Gibbs free energy](https://en.wikipedia.org/wiki/Gibbs_free_energy) or *free enthalpy* is most commonly convenient for systems at constant *pressure*).  

To help solve similar problems that Helmholtz faced with physical systems composed of an incredibly complex amount of interactions, alternative reformulations of classical mechanics were developed throughout the history of physics like that of [Lagrangian mechanics](https://en.wikipedia.org/wiki/Lagrangian_mechanics) that either treat constraints explicitly as extra equations or incorporates them directly via a particular choice of [generalized coordinates](https://en.wikipedia.org/wiki/Generalized_coordinates), and that of [Hamiltonian mechanics](https://en.wikipedia.org/wiki/Hamiltonian_mechanics) which conceptualizes something known as the Hamiltonian, which often corresponds to the total energy of the system (indeed it is quite useful for describing systems where energy keeps oscillating between kinetic and potential forms, and is essentially the [Legendre tranform](https://en.wikipedia.org/wiki/Legendre_transformation) of the Langragian (function) itself where the generalized coordinates q_i and time are fixed).  

Similar to the above, physicists like [Feynman](https://en.wikipedia.org/wiki/Richard_Feynman) were able to use a minimization technique (known as a [variational method](https://en.wikipedia.org/wiki/Calculus_of_variations)) applied to free energy (which originally was physically interpreted as Helmholtz free energy) to solve previous calculation intensive problems.  It is important to note that a *variational* principle in physics is a method for determining the state or dynamics of a physical system by identifying it as an *extremum* (ie - a minimum, maximum, or saddle point) of a function or [functional](https://en.wikipedia.org/wiki/Functional_(mathematics)) such as in the case of the previously mentioned time integral of the Lagrangian called the [action](https://en.wikipedia.org/wiki/Action_(physics)) which takes a trajectory, path, or history of a system as input and spits out a real number as output.  It is key to note the vocabularly of extremums of functions, functionals, paths, etc, which all presuppose a notion that there could be a multitude of possible paths where there is such a thing as the optimal path, and the baked-into need for a language like the *Calculus of Variations* which analyzes the variations of a functional / path (ie - by looking at the small changes in a functional's value due to small changes in the function that is its argument).  

<br/>

<center>
<a href="https://en.wikipedia.org/wiki/Brachistochrone_curve">
    <img src="/images/post_pics/free_energy_principle/brachistochrone.gif"
        width="400" 
        height="400"
        >
</a>
</center>

<br/>

And this is not only isolated to Jaynes, Feynman, or more modern day scientists.  Similar principles [throughout the history of physics](https://en.wikipedia.org/wiki/History_of_variational_principles_in_physics) can be found in refraction and optics in the 17th century by [Pierre de Fermat](https://en.wikipedia.org/wiki/Pierre_de_Fermat) (known as his technique of [adequality](https://en.wikipedia.org/wiki/Adequality) or Fermat's [principle of least time](https://en.wikipedia.org/wiki/Fermat%27s_principle) linking ray optics to wave phenomena), Peirre Maupertuis' 1746 quote "Nature is thrifty in all its actions", Euler's 1744 formulation of the action principle, Gauss' 1829 [principle of least constraint](https://en.wikipedia.org/wiki/Gauss%27s_principle_of_least_constraint), Hertz's [principle of least curvature](https://en.wikipedia.org/wiki/Gauss%27s_principle_of_least_constraint#Hertz's_principle_of_least_curvature), the 1915 [Einstein-Hilbert's principle of least action](https://en.wikipedia.org/wiki/Einstein%E2%80%93Hilbert_action), generalizations connecting underlying symmetries of physical systems with corresponding conservation laws given by [Noether in 1915](https://en.wikipedia.org/wiki/Noether%27s_theorem), etc.  And this is not only limited to the physical sciences.  The overarching appeal to an *economy of nature* or *Principle of Parsimony* can likewise be seen all throughout the philosophical world such as in the case of Leibniz's "best of all possible worlds" where he envisioned God as the great mathematician, 

> "As is well known, the theory of the maxima and minima of functions was indebted to him [Leibniz] for the greatest progress through the discovery of the method of tangents. Well, he conceives God in the creation of the world like a mathematician who is solving a minimum problem, or rather, in our modern phraseology, a problem in the calculus of variations – the question being to determine among an infinite number of possible worlds, that for which the sum of necessary evil is a minimum." 

Leibniz himself was following a lineage of similar thought generally going under the header of the *[Principle of Sufficient Reason](https://en.wikipedia.org/wiki/Principle_of_sufficient_reason)* extending from Anaximander, Parmenides, and [Plato](https://en.wikipedia.org/wiki/Theory_of_forms), etc.  In fact, I might be as bold to suspect that much of the philosophical problems surrounding the attitudes today of cognitive scientists, biologists, and philosophers regarding the FEP can be traced to the underlying *[teleogical](https://en.wikipedia.org/wiki/Teleology* or *purpose/goal-based* character of the action principle which in turn stem from the philosophical consequences between differential equations of motion and their [integral counterparts](https://en.wikipedia.org/wiki/History_of_variational_principles_in_physics#Apparent_teleology?). 

Whereas differential equations are statements about quantities localized to a single point in space or a single moment in time, action principles are not localized to points but rather involve summing over an interval of time or a region of space where it is required that you **fix a final state** of the system.  (Apparently, this seems to be eliminated in the quantum mechanical version of the action principle (*note to self to expand on this*)) And indeed, similar controversies were brought up against Fermat in 1662(!) because of this principle seemingly ascribing knowledge, purpose, and intent to nature.  As we can see, if we accept this historical tracing of lineage of thought, the averse reaction some may have going under the general banner of *"[A map is not the territory](https://en.wikipedia.org/wiki/Map%E2%80%93territory_relation)"* might be tempered a bit by knowledge that this concept and associated critics have been around for quite some time.  Whether or not the teleogical argument is solved seems to depend upon your underlying metaphysical assumptions of the world and potentially your particular philosophical thoughts surrounding the interaction of mathematics and reality.[^11]

---

## Mathematics:

### Sweeping problems underneath the Markov blanket?

To begin investigating how this teleology crops up, we need to figure out where it is being used and how.  To do that we first need to see how Friston mathematically captures the notion of a system of interacting parts that can be distinguished from its environment.  To do that we need to begin explain the mathematical object that seems to wrap up all our problems into nice little bundles--the Markov blanket.

A stochastic or random system/process can be said to exhibit something called the *[Markov property](https://en.wikipedia.org/wiki/Markov_property)* or *memoryless* property if, roughly speaking, its future state depends only upon the state that immediately came before it, not the whole sequence of events that precede it.  It reflects the statistical notion known as *conditional independence* where two events *a* and *b* are conditionally independent if and only if the probability of one event *a* given that the other event *b* occurred is equal to the probability that *a* occurred without any knowledge of *b* having occurred.  Basically, the knowledge of event *b* doesn't change anything, or in other words, knowing the current state we can't get any more information about the future by further knowledge of the past. This notion can be represented formally below:

<br/>

<center>
<a href="https://towardsdatascience.com/brief-introduction-to-markov-chains-2c8cab9c98ab">
    <img src="/images/post_pics/free_energy_principle/markovproperty.png"
        width="400" 
        height="400"
        >
</a>
</center>

<br/>

A *[Markov blanket](https://en.wikipedia.org/wiki/Markov_blanket)* is essentially a way of statistically demarcating the boundaries of a system of interest separate from its environment.  It is a statistical partitioning of a system into internal states and external states, where the blanket itself consists of the states that separate the two.  We can define a state to be any variable that locates the system at a particular point in [state space](https://en.wikipedia.org/wiki/State_space) (which itself is the set of all possible configurations of a system).[^12]  

<br/>

<center>
<a href="https://en.wikipedia.org/wiki/Markov_blanket">
    <img src="/images/post_pics/free_energy_principle/markovblanket.png"
        width="400" 
        height="400"
        >
</a>
</center>

<br/>

In the graphical language of modeling (ie - a Bayesian Network), a Markov blanket represents the set of nodes of all parents of A, children of A, and all the children's parents other than A.  Each node represents an event in time or particular state of the system.  Each arrow represents the *directed* causal influence one node or event has upon another.  In Friston's particular terminology (which deviates a small bit from [Judea Pearl](https://en.wikipedia.org/wiki/Judea_Pearl)'s [conception](https://www.goodreads.com/book/show/174277.Probabilistic_Reasoning_in_Intelligent_Systems)), he further distinguishes the parent nodes of A as *sensory states* and the children nodes of A as *active states*, where sensory states are causally influenced by *external states* and active states are only influenced by *internal states*.[^12]  This blanket is labeled *Markov* because the blanket separates out from the environment both the variables that do not depend on the central node A and the variables that the central node A itself doesn't depend on.  Each variable in the blanket exhibits the aforementioned *Markov property* and as such, is all the information we need to know about the system. You might begin to think that we can have nested blankets within blankets, potentially continuing on *ad infinitum* and you are correct.  This is where Pearl further defined an additional term called the *[Markov boundary](https://en.wikipedia.org/wiki/Markov_blanket#Markov_boundary)* which is the *minimal* or "smallest" such Markov blanket that we could have.  

So how do we go about encoding some Markov blanket into the language of mathematics?  It is common to encode graphs as mathematical objects called [adjacency matrices](https://en.wikipedia.org/wiki/Adjacency_matrix).  An adjacency matrix is a square matrix where each row header and column header represents a specific node and the cross-sectional entries or elements of the matrix indicate whether or not a pair of nodes in that particular row-column pair are adjacent / connected or not.  The value of this particular element of the matrix is the probability of one state or node *transitioning* to the next state or node.  This is why we sometimes specifically call this a *[transition matrix](https://en.wikipedia.org/wiki/State-transition_matrix)*.  

This adjacency matrix, which we can call *A*, represents the causal graph of the entire system.  We specifically would like to construct the matrix that represents the Markov blanket only.  Doing some linear algebraic manipulations to get there, Friston defines our new matrix,

$$ B = A + A^{T} + A^{T} \times A $$  

To further reduce our graph to only those nodes we care about (for instance, our *minimal* Markov blanket), we can then multiply this matrix B by a binary encoded vector V (a vector of 1s and 0s) representing the nodes we want, giving us [ B·V ].  If you've studied some [linear algebra](https://en.wikipedia.org/wiki/Linear_algebra), we can then recall that the *[eigenvector](https://en.wikipedia.org/wiki/Eigenvalues_and_eigenvectors)* of a matrix (where a matrix is just a [linear transformation/mapping](https://en.wikipedia.org/wiki/Linear_map) from one space to another) is the vector that maintains its direction under that transformation and only scales to some scalar amount λ.  This principal eigenvector now represents the strength of causal interaction between states, from which we then apply some educated pick of a threshold to group individual states.  

At this point, I think this is where I am maybe not as critical as someone like Andrews where they believe this thresholding to be a post-hoc, intuition-guided, individual researcher-based ascription, and most importantly not *"illuminating natural joints"*[^6].  In fact, the [spectral theory](https://en.wikipedia.org/wiki/Spectral_theory) underlying [eigendecomposition](https://en.wikipedia.org/wiki/Eigendecomposition_of_a_matrix) and thresholding methods is done all the time in [vibration analysis](https://en.wikipedia.org/wiki/Harmonic_analysis) (eg - ["Can One Hear the Shape of a Drum?"](https://en.wikipedia.org/wiki/Hearing_the_shape_of_a_drum)), dimensionality reduction / [Principle Component Analysis](https://en.wikipedia.org/wiki/Principal_component_analysis), [Google's Page Rank algorithm](https://en.wikipedia.org/wiki/PageRank), collaborative prediction, image compression, general clustering problems, and more.  I agree that there are many assumptions that go into the mathematics of all of this and indeed it might be wise to keep at the back of our minds the divide between the language we use to to describe reality and reality itself, but at the same time I don't think that this implies that the math itself does not elucidate *any* insight into the nature of the physical system in question. As mentioned in the previously examples, these representations definitely can provide real-world utility.  Whether or not mother nature has latched onto a similar causal mechanism in how biological organisms maintain integrity and govern themselves still seems up for debate. (*Note to self that this part of the notes will be updated accordingly*)  

---

### Introducing the language of Dynamical Systems

Okay, so Friston posits the claim that Markov blankets are pretty much everywhere.  From his paper[^12]:

> "Here we consider how a collective of Markov blankets can self-assemble into a global system that itself has a Markov blanket; thereby providing an illustration of how autonomous systems can be understood as having layers of nested and self-sustaining boundaries. This allows us to show that: (i) any living system is a Markov blanketed system and (ii) the boundaries of such systems need not be co-extensive with the biophysical boundaries of a living organism. In other words, autonomous systems are hierarchically composed of Markov blankets of Markov blankets—all the way down to individual cells, all the way up to you and me, and all the way out to include elements of the local environment."

And we can indeed see how our previously defined Markov blanket is a rather *broadly-encompassing* concept.  What isn't a Markov blanket?  I think to help answer that question we need to explore how a system is supposed to maintain its *"Markov-blanket-ness"*, or in other words, how is a system supposed to keep maintaining its *Identity* as a distinct set of interacting parts separate from the stuff composing its environment?  How does it maintain its integrity without losing its *self* and dissolving into the environment? How does it keep hold of its Markov blanket?

Friston explains that in order to possess a Markov blanket, a system must minimize something we hinted at before called *variational free energy*. It is here where someone like Andrews[^6] comments:

> "There is an unfortunate—though understandable—tendency for those first acquainting themselves with the FEP to interpret ‘free energy,’ and other, similarly confounding terminology from the framework, in physical terms. When we speak of heat, energetics, and entropy it can be difficult to shake the feeling that we are talking about some objective, measurable feature of a material system—particle motion, for example. I took the time at the outset of this paper to trace the history of the framework in Jaynes, Feynman, Hinton, and Beal because having a handle on this history is necessary in order to grasp the subtle turn away from statistical approximations of physical properties of physical systems to a pure, substrate-neutral method of statistical inference. When we speak of annealing a model in statistical mechanics, ratcheting the temperature of the system up and down in the hopes of bumping it out of local minima, this does not refer to an act of literally injecting energy into a physical system to increase the speed of particle motion. It is a statistical analogue of a physical process. Likewise, the energy and entropy of the FEP are formal analogues of concepts defined in thermodynamics and statistical mechanics with a long history of use in information theory, statistics, and machine learning, in which they have lost their correspondence to any measurable properties of physical systems." 

I can definitely sympathize with this criticism.  Adopting mathematics, analogies, metaphors, theories, and jargon from one field to the next doesn't always transfer over in perfect isomorphic fashion.  Some concepts fit.  Some stretch.  And some break.  But just because something breaks or doesn't perfectly map over from one domain to another doesn't necessarily mean we should abandon it.  Nor should we even jump to the conclusion that something *is* necessarily broken with the borrowed formalism or apparatus even if it looks like it from the surface (I am not necessarily accusing Andrews of any of these by the way), but maybe rather something doesn't align in our internal metaphysical beliefs to that of others. Furthermore, generally-speaking, maybe there is a lack of alignment in what we currently demand from mathematics and language itself.  I mean, I certainly have days where I'm a skeptical scientific [Materialist](https://en.wikipedia.org/wiki/Scientistic_materialism), most days where I'm a hardcore [Fictionalist](https://en.wikipedia.org/wiki/Fictionalism), and yes I admit, even some days where I'm a happy-go-lucky-everything-is-oh-so-beautiful-math [Platonist](https://en.wikipedia.org/wiki/Platonism).    

Anyway, the reason I question whether or not it really is a metaphysical deathblow that the FEP has lost its correspondence with physical systems is because in the philosophy of physics there are people even questioning our most primitive (and from what I previously thought) well-accepted terms and concepts.  Questions such as whether *Force* or *Energy* are more real bring up interesting thoughts and consequences[^13] and like before, can possibly act to temper some of our criticisms. 

So getting back to the main topic, what exactly is variational free energy and how is it being minimized? To explain this we need to learn about something called the [Fokker-Planck or Kolmogorov Forward Equation](https://en.wikipedia.org/wiki/Fokker%E2%80%93Planck_equation).  Just as how the *velocity* of a moving particle is the *rate of change* of the *displacement* at some time, the *probability density* of a continuous real-valued [random variable](https://en.wikipedia.org/wiki/Random_variable) is the *rate of change* of the *cumulative probability* at some *point*.  The *[probability density function](https://en.wikipedia.org/wiki/Probability_density_function)* is used to specify the probability of the random variable falling within a particular range of values as opposed to taking on any one value (in discrete as opposed to continous cases, this is instead called the [Probability Mass Function](https://en.wikipedia.org/wiki/Probability_mass_function) or PMF).  And it's key to note that this probability is given by the area or integral of the variable's PDF over that range.  Finally, the Fokker-Planck equation describes how this [probability density function](https://en.wikipedia.org/wiki/Probability_density_function) itself of the state of a system changes over time, in essence, a trajectory through some abstract space of a system's set of states.  

Our system here is assumed to be under the effect of random perturbations called [Brownian motion](https://en.wikipedia.org/wiki/Brownian_motion).  These random perturbations would eventually cause the system to undergo an irreversible process known as *[dissipation](https://en.wikipedia.org/wiki/Dissipation)* in which energy is transformed from some initial form to some final form, where the final form has less capacity to perform mechanical work (ie - although total energy is conserved, not all types of energy are spent equally).  So what's keeping the system from dissipating in its entirety?

Friston conceptualizes the underlying dynamical system as a vector field in three dimensions.  Assuming appropriate smoothness and decaying conditions, there's something called the *[Helmholtz decomposition]*(https://en.wikipedia.org/wiki/Helmholtz_decomposition), otherwise known as the *Fundamental Theorem of Vector Calculus*, which states that a rapidly decaying vector field in three dimensions can be broken up into the sum of two components, an [irrotational (curl-free)](https://en.wikipedia.org/wiki/Conservative_vector_field) vector field and a [solenoidal (divergence-free)](https://en.wikipedia.org/wiki/Solenoidal_vector_field) vector field.

<br/>

<center>
<a href="https://en.wikipedia.org/wiki/Solenoidal_vector_field">
    <img src="/images/post_pics/free_energy_principle/solenoidal_field.png"
        width="400" 
        height="400"
        >
</a>
</center>

<br/>

Whereas the latter *solenoidal* or *divergence-free field* is known for its property that the field has no sources or sinks (and hence the flow of the solenoidal field can't *diverge*), for the purposes of the FEP it is important to note the other former component.  The other component is called the *irrotational vector field* or dissipative flow. Furthermore, when given that the domain is a simply connected open region, a vector field represents forces of a physical system in which energy is conserved (ie - the reason why they are sometimes called *conservative* vector fields).  For such an irrotational system, the work done in moving along a path in [configuration space](https://en.wikipedia.org/wiki/Configuration_space_(physics)) (the space of [all possible positions](https://physics.stackexchange.com/questions/237278/what-is-the-difference-between-the-meaning-of-state-space-and-configuration-s#:~:text=In%20other%20words%2C%20the%20state,space%20of%20all%20possible%20positions)) depends only on the endpoints of the path, so it is possible to define a potential energy that is independent of the actual path taken (Note to self - Could this be where a portion of the teleology is initially baked-in?) 

A really great [intuitive explanation](https://en.wikipedia.org/wiki/Conservative_vector_field#Intuitive_explanation) of conservative vs. non-conservative vector fields can be given by M.C. Escher's lithograph print, *Ascending and Descending*:

> Ascending and Descending illustrates a non-conservative vector field, impossibly made to appear to be the gradient of the varying height above ground as one moves along the staircase. It is rotational in that one can keep getting higher or keep getting lower while going around in circles. It is non-conservative in that one can return to one's starting point while ascending more than one descends or vice versa. On a real staircase, the height above the ground is a scalar potential field: If one returns to the same place, one goes upward exactly as much as one goes downward. Its gradient would be a conservative vector field and is irrotational. The situation depicted in the painting is impossible.

<br/>

<center>
<a href="https://en.wikipedia.org/wiki/Ascending_and_Descending">
    <img src="/images/post_pics/free_energy_principle/escher_stairs.jpg"
        width="400" 
        height="400"
        >
</a>
</center>

<br/>

Friston points out that this dissipative, curl-free flow is the component responsible for counteracting the dissipation caused by the random perturbations of Brownian motion of the underlying vector field (representing the dynamical system).[^14]  This implies that the only remaining [probability current](https://en.wikipedia.org/wiki/Probability_current) is solenoidal, where the term *probability current* describes the flow of probability in terms of probability per unit time per unit area.    

Now this is where things get a bit fuzzy for me.  I don't quite see what is *driving* the system to be maintained in this state with the condition of a rapidly decaying vector field (our condition for the Helmholtz decomposition of the two different vector field components to occur).  

If I'm understanding Friston correctly, he states that the reason we have this system being maintained in this state is because the [non-equilibrium](https://en.wikipedia.org/wiki/Non-equilibrium_thermodynamics) (it is key to note that condition) long-term behavior of any random dynamical system when [weakly mixing](https://en.wikipedia.org/wiki/Mixing_(physics)) will after a sufficient amount of time converge to an invariant set of states called a *pullback* or *[random global attractor](https://en.wikipedia.org/wiki/Pullback_attractor)*.[^14] (I'll have to do more research into this since my understanding is fuzzy and my linguistic-physical intuition is fighting me over random sets even having attractors to begin with). 

### Is there an isomorphism in the inferential engine interpretation?


To cast the aforementioned dynamical systems interpretation into the language of probability and information theory we first have to explain how we capture epistemic notions such as belief, evidence, and the relationship between how we update our old beliefs with new evidence to get new beliefs.  We can see that relationship in the following:  

$$ \text{New Level of Belief} = \text{Strength of New Evidence} \times \text{Old Level of Belief} $$

$$ P(H \mid E) = \frac{P(E \mid H) \times P(H)} {P(E)} $$

where we let 

$$ P(H \mid E) $$

be read as, "Probability of our Hypothesis being true given that our Evidence is true".  And similarly we can fill in the other terms. 




Surprise = -ln(P(x)) ...ie - the lower the probability of the event, the more you should be surprised to have seen that event







*** Then connect this back with the dynamical systems perspective using Mel Andrew's explanations by distilling her quotes 














---

Resources:

[^1]: [Life as we know it](https://royalsocietypublishing.org/doi/pdf/10.1098/rsif.2013.0475) by [Karl Friston](https://en.wikipedia.org/wiki/Karl_J._Friston), perhaps most (in)famous for his contribution of the variational [Free Energy Principal](https://en.wikipedia.org/wiki/Free_energy_principle) to the field theoretical neuroscience and the foundations of biology. From the abstract: "This paper presents a heuristic proof (and simulations of a primordial soup) suggesting that life—or biological self-organization—is an inevitable and emergent property of any ([ergodic](https://en.wikipedia.org/wiki/Ergodicity)) random dynamical system that possesses a [Markov blanket](https://en.wikipedia.org/wiki/Markov_blanket). This conclusion is based on the following arguments: if the coupling among an ensemble of dynamical systems is mediated by short-range forces, then the states of remote systems must be conditionally independent. These independencies induce a Markov blanket that separates internal and external states in a statistical sense. The existence of a Markov blanket means that internal states will appear to minimize a free energy functional of the states of their Markov blanket. Crucially, this is the same quantity that is optimized in [Bayesian inference](https://en.wikipedia.org/wiki/Bayesian_inference). Therefore, the internal states (and their blanket) will appear to engage in active Bayesian inference. In other words, they will appear to model—and act on—their world to preserve their functional and structural integrity, leading to homoeostasis and a simple form of autopoiesis." 

[^2]: [Exploration, novelty, surprise, and free energy minimization](https://www.frontiersin.org/articles/10.3389/fpsyg.2013.00710/full) by Schwartenbeck, FitzGerald, Dolan, and Friston.  From the abstract: "This paper reviews recent developments under the free energy principle that introduce a normative perspective on classical economic (utilitarian) decision-making based on (active) Bayesian inference. It has been suggested that the free energy principle precludes novelty and complexity, because it assumes that biological systems—like ourselves—try to minimize the long-term average of surprise to maintain their homeostasis. However, recent formulations show that minimizing surprise leads naturally to concepts such as exploration and novelty bonuses. In this approach, agents infer a policy that minimizes surprise by minimizing the difference (or relative entropy) between likely and desired outcomes, which involves both pursuing the goal-state that has the highest expected utility (often termed “exploitation”) and visiting a number of different goal-states (“exploration”). Crucially, the opportunity to visit new states increases the value of the current state. Casting decision-making problems within a variational framework, therefore, predicts that our behavior is governed by both the entropy and expected utility of future states."  

[^3]: [A Free Energy Principle for Biological Systems](https://www.mdpi.com/1099-4300/14/11/2100/htm) by Friston. From the abstract, "This paper describes a free energy principle that tries to explain the ability of biological systems to resist a natural tendency to disorder. It appeals to circular causality of the sort found in synergetic formulations of self-organization (e.g., the slaving principle) and models of coupled dynamical systems, using nonlinear Fokker Planck equations. Here, circular causality is induced by separating the states of a random dynamical system into external and internal states, where external states are subject to random fluctuations and internal states are not. This reduces the problem to finding some (deterministic) dynamics of the internal states that ensure the system visits a limited number of external states; in other words, the measure of its (random) attracting set, or the Shannon entropy of the external states is small. We motivate a solution using a principle of least action based on variational free energy (from statistical physics) and establish the conditions under which it is formally equivalent to the information bottleneck method."

[^4]: [New directions in predictive processing](https://www.researchgate.net/publication/339621889_New_directions_in_predictive_processing) by Hohwy. 

[^5]: [Self-supervision, normativity and the free energy principle](https://www.researchgate.net/publication/339918179_Self-supervision_normativity_and_the_free_energy_principle)

[^6]: [The Math is not the Territory: Navigating the Free Energy Principle](http://philsci-archive.pitt.edu/18315/1/Andrews_25.10.20_TMINTT.pdf) by Mel Andrews, a PhD student working in the intersection of the philosophy of biology and cognitive science.  This is a, 
You can also often find them posting [their thoughts on Twitter](https://twitter.com/bayesianboy) :)

[^7]: [It’s Bayes All The Way Up](https://slatestarcodex.com/2016/09/12/its-bayes-all-the-way-up/) and [God Help Us, Let’s Try To Understand Friston On Free Energy](https://slatestarcodex.com/2018/03/04/god-help-us-lets-try-to-understand-friston-on-free-energy/) Blog posts by Scott from SlateStarCodex that one should read if you a tad math-averse as they help motivate why we might care about this topic from a neuroscience standpoint and they do this in a very intuitive way. Scott is a psychiatrist and famous blogger in online Rationalist community. 

[^8]: For example, [John Harte](https://en.wikipedia.org/wiki/John_Harte_(scientist)) at UC Berkeley is an ecologist doing fascinating work investigating the distribution and abundance of species in ecosystems using a general theory of maximum entropy.  I got to speak with him a few times as part of the [Information & Uncertainty discussion group](http://compdatascience.org/entropy/) led by [Gerald Friedland](https://bids.berkeley.edu/people/gerald-friedland), which in particular seems to take a very intertwined perspective on the formalisms of thermodynamic entropy and information. 

[^9]: [The free energy principle for action and perception: A mathematical review](https://arxiv.org/abs/1705.09156)

[^10]: [Friston's Free Energy Principle Explained](https://jaredtumiel.github.io/blog/2020/08/08/free-energy1.html) An excellent blog post from an even sharper autodidactic mind of Jared Tumiel.  Besides delving into academic papers, I think this is one of the best alternatives for understanding the *mathematics* behind the Free Energy Principle.  He also has an [entire syllabus](https://jaredtumiel.github.io/blog/2020/10/14/spinning-up-in-ai.html) for understanding the FEP, runs a podcast called [Bit of a Tangent](https://www.podtangent.com/) and posts his thoughts on Twitter [here](https://twitter.com/jnearestn).

[^11]: [The Unreasonable Effectiveness of Mathematics in the Natural Sciences](https://en.wikipedia.org/wiki/The_Unreasonable_Effectiveness_of_Mathematics_in_the_Natural_Sciences) is the title of an article published in 1960 by the physicist [Eugene Wigner](https://en.wikipedia.org/wiki/Eugene_Wigner).  In it he discusses the seeming miracle of the appropriateness of the language of mathematics for the formulation of the laws of physics.  I want to give a quick shoutout to [Mihály Bányai](https://www.researchgate.net/profile/Mihaly_Banyai), a former PhD student mentor of mine while I was studying at [Eötvös Loránd University](https://en.wikipedia.org/wiki/E%C3%B6tv%C3%B6s_Lor%C3%A1nd_University) and working at the Wigner Research Centre for Physics in Budapest, Hungary.  I thought the paper was rather simple and boring at the time, but have come to appreciate my mentor's prescience over the years for urging me to read it.

[^12]: [The Markov blankets of life: autonomy, active inference and the free energy principle](https://royalsocietypublishing.org/doi/10.1098/rsif.2017.0792) by Michael Kirchhoff, Thomas Parr, Ensor Palacios, Karl Friston and Julian Kiverstein. From the abstract: "This work addresses the autonomous organization of biological systems. It does so by considering the boundaries of biological systems, from individual cells to Home sapiens, in terms of the presence of Markov blankets under the active inference scheme—a corollary of the free energy principle. A Markov blanket defines the boundaries of a system in a statistical sense. Here we consider how a collective of Markov blankets can self-assemble into a global system that itself has a Markov blanket; thereby providing an illustration of how autonomous systems can be understood as having layers of nested and self-sustaining boundaries. This allows us to show that: (i) any living system is a Markov blanketed system and (ii) the boundaries of such systems need not be co-extensive with the biophysical boundaries of a living organism. In other words, autonomous systems are hierarchically composed of Markov blankets of Markov blankets—all the way down to individual cells, all the way up to you and me, and all the way out to include elements of the local environment."

[^13]: [Force and energy: which is more real?](https://gravityandlevity.wordpress.com/2009/04/13/force-and-energy-which-is-more-real/) is post from *On Gravity and Levity* by Brian Skinner, a professor in theoretical condensed matter physics. In it he discusses the question of whether *Force* or *Energy* is more real? He notes that the question "is one to which my answer has changed over the years.  The change was a difficult one: force and energy are such profoundly important concepts in physics that to change your view of them is to change your view of all topics that are built upon them (basically, everything).  But for me it has been extremely important.  Shifting my position from “force is more real” to “energy is more real” was essential for understanding and enjoying advanced topics in physics."  Another somewhat relevant post to the FEP's inherent teleology is his post on [The Universe is a giant energy minimization machine](https://gravityandlevity.wordpress.com/2010/01/30/the-universe-is-a-giant-energy-minimization-machine/).   

[^14]:  [A free energy principle for a particular physics](https://arxiv.org/abs/1906.10184) by Karl Friston.  This is probably the most informative write-up on Friston's theory, but as such it suffers from the fact that it is 148 pages long! From the abstract: "This monograph attempts a theory of every 'thing' that can be distinguished from other things in a statistical sense. The ensuing statistical independencies, mediated by Markov blankets, speak to a recursive composition of ensembles (of things) at increasingly higher spatiotemporal scales. This decomposition provides a description of small things; e.g., quantum mechanics - via the Schrodinger equation, ensembles of small things - via statistical mechanics and related fluctuation theorems, through to big things - via classical mechanics. These descriptions are complemented with a Bayesian mechanics for autonomous or active things. Although this work provides a formulation of every thing, its main contribution is to examine the implications of Markov blankets for self-organisation to nonequilibrium steady-state. In brief, we recover an information geometry and accompanying free energy principle that allows one to interpret the internal states of something as representing or making inferences about its external states. The ensuing Bayesian mechanics is compatible with quantum, statistical and classical mechanics and may offer a formal description of lifelike particles."


[^]: [Surfing Uncertainty: Prediction, Action, and the Embodied Mind](https://www.goodreads.com/book/show/25823558-surfing-uncertainty) is a book by [Andy Clark](https://en.wikipedia.org/wiki/Andy_Clark), a philosopher of logic, metaphysics, and cognitive science.  In it he explains the predictive processing framework and how it can be used to explain the role of the mind in the intersection of neuroscience, psychology, and robotics.   

[^]: [Vanilla PP for Philosophers: A Primer on Predictive Processing](https://predictive-mind.net/papers/vanilla-pp-for-philosophers-a-primer-on-predictive-processing) by Wanja Wiese & Thomas Metzinger.  "The goal of this short chapter, aimed at philosophers, is to provide an overview and brief explanation of some central concepts involved in predictive processing (PP). Even those who consider themselves experts on the topic may find it helpful to see how the central terms are used in this collection. To keep things simple, we will first informally define a set of features important to predictive processing, supplemented by some short explanations and an alphabetic glossary."

[^]:  [The Genius Neuroscientist Who Might Hold the Key to True AI](https://www.wired.com/story/karl-friston-free-energy-principle-artificial-intelligence/) by WIRED magazine did a special on Friston and his FEP.  