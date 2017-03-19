## Introduction

Sugarscape is an agent-based model that simulates the behavioral characteristics of a group of agents submitted to several predefined rules. This artificially inteligent model was first presented by Joshua M. Epstein & Robert Axtell in their book *Growing Artificial Societies*. This model was considered the first large scale agent model. 

The Sugarscape model consists of three basic elements: the environment (a 51x51 cell grid, where every cell can contain different amounts of sugar or spice), the agents (who inhabit the environment), and the rules that define the behavior of the agents with each other and with the environment. 

SugarScape simulation therefore can be seen as a metaphor for resources and inhabitants forming societies in an artificial world and the effects of social dynamics such as evolution, birth rates, death rates, population growth, inheritance on populations, social interaction, etc. can be studied.

## Algorithm

**1.** In every step each agent looks around and evaluates its depending on its range of vision.

**2.** The agent identifies the objects in its vecinity, which can be other agents with different intrinsic characteristics such as sex, tribe, maximum age, metablism rate, and vision rate, or sugars and spices, each with different energy contributions.

**3.** The agent then decides to which cell it's more convinient to move. The agent will move giving priority to the chance of reproducing sexually. The agent will be able to reproduce sexually only if it meets certain conditions:
1. The agent has to have energy enough and be old enough.
2. The agent can only reproduce sexually with an agent from a different sex and the same tribe.

If the agent can't reproduce sexually, it wil try to reproduce asexually if it has energy enough.
In case the agent can't do any of these two functions, it will try to move to a place where trading with another agent can take place. For this to be possible the agent has to have energy enough and can only trade with agents of a different tribe.
Finally, the agent will try to move to a cell where there's a sugar or a spice, assesing the quantity of energy each nearby good gives, to gain more energy.

**4.** Each cell the agent moves, the agent looses energy depending in its metabolism rate. 

**5.** Each step the agent has the possibity of dying if it runs out of energy, randomly (with a probability of .002%)  or if its age is surpasses its maximun age. 

## Conclusion

After analyzing the SugarScape model submitted to the rules and parameters we defined, we could make the following obsevations:

At first the population of agents in the environment is stable (it does not increase or decrease in a significant way). However, as the number of steps increases we can also observe that the number of agents in the environment also increases, due to the fact that the agents are constantly reproducing and the goods in the environment are constantly regenerating whenever the environment is about to run out of goods.

With the help of the Gini Index and the Lorenze Curve, we could observe that as the population increases, the distibution of goods among the agents in the environment becomes more unequal; the inequality increases as the population grows.

In the environment we can also observe that, due to the fact that each agent gives priority to sexual reproduction when deciding where to move, and considering that agents can only reproduce with agents that belong to their same tribe, agents will segregate in the environment into tribes. Consecuently, certain places in the world are mostly occupied by a specific tribe.

Finally, we could observe certain signs of evolution. Considering that the higher an agent's metabolism rate is, the faster it runs out of energy and dies, the surviving agents have mostly low metabolism rates. This same event happens with the agent's vision range. The agents with higher vision ranges are the ones surviving in the end because they are able to look for goods and other agents farther away in the environment.

Note: "Exact simulation of the original rules provided by J. Epstein & R. Axtell in their book can be problematic and it is not always possible to recreate the same results as those presented in Growing Artificial Societies."(*Replicating Sugarscape* — University of Leicester". Retrieved 18 January 2011)