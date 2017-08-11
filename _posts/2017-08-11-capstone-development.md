---
published: true
tags:
- Capstone
- Ecological Modelling
---

Today marks the day my capstone journey begins. After lengthy discussions with my capstone supervisor, my co-supervisors and the head of studies for MCS, I have finally reached a topic I can work on for the next 9 months.

Originally I wanted to work on parallelizing existing Agent Based Models, partially because I have always been interested in Agent Based Modelling for complex systems, and that seems to be an emerging field. However, talking to my supervisors, the type of model doesn't really matter as much. There are other questions that matter more: 
1. What kind of question am I trying to answer? 
2. What model best fits in the framework of my question? 
3. What do I want to get out of it? 

These gave me a lot of food for thought. In terms of what I want to get out of it, I realized that I joined MCS as a major not for the theoretical aspects, but rather what I could do with it. Coding up an agent based model is good, but it is too time consuming, and the amount of benefits (ecologically) I get from an agent based model is not as significant as what I would get out of the statistical model I had already been creating. Thus, on the MCS side, I will be creating an interface for a statistical ecological model for researchers / students of ecology to play around with and generate / test hypotheses.

On the ecological side, the main question I am answering is: *What is the relative importance of different factors driving successional patterns in secondary forests?* There are a few questions that follow: 

1. How are we measuring importance? 
2. What effects do those factors have on forests? 
3. What kind of hypotheses can we realistically test with it?
4. How are we extending the current work we're doing?

In a nutshell, at the moment, we have been looking at the relative importance of the size and structure of local species pools as well as species specific recruitment and mortalities on forest succession. The main problem is that empirical ecologists are constrained by their plots. They are only able to see the net effects of various factors on their plots but are unable to see which factors are more or less important. This is why by parameterizing those drivers of succession, researchers / students of ecology are able to play around with the model and test hypotheses as to which ones are more significant. 

To add more complexity to the model, we are presenting an opportunity to explore more complex patterns in isolation. Some ways include:

1. Varying the local species pool (LSP)
	> In terms of composition
	> Making LSP habitat specific 
2. Varying plot level dynamics
	> Limited Similarity (Toggle with degree of similarity of groups of trees): Link it to abundance - The more trees there are in the plot, the more likely it is to die off due to common enemies and similar resources used. These can be varied by functional groups i.e. Pioneer species attacked by more general pathogens, while non-pioneer species attacked by more specific pathogens. Varying pathogens could be a way to affect the probability of recruitment and mortality. 
	> Species specific recruitment probabilities on a scale from deterministic to stochastic (in space and in time). The stochasticity of pioneer species are important because they affect beta diversity to a greater degree. This is also a question of dominance. How dominant are pioneer species across the landscape? What causes this dominance? Question remains: What does varying the stochasticity actually accomplish? How can we link this to its ecological context?

All of these are significant additions to the model, and would take time to incorporate. The reality is that there is going to be a cyclical relationship in the development of the model. My professor astutely pointed out that there are 3 components:

1. Data Collection
2. Model development
	> Conceptual 
	> Programming
3. Interface

Within these components, the conceptual-interface, conceptual-programming, and programming-interface cycles will be time-consuming and a lot of time will be spent refining them and making them usable by the public. Thus, finding a balance between the complexity of the model and the development of the model will be critical to finishing the capstone on time.


