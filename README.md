# Game Theory

#### Intro

**Strategic** interactions between self-interested peoople. 

Two player game. TCP Backoff

**Self-interested** each agent has its own description of states of the world, and acts based on this description. 

**utility function.** 

- Quantifies degree of preference across alternatives
- explains the impact of uncertainty
- act to maximize expected utility

**Defining Game**

Players: N. 

Action set: Ai. 

Utility function: ui.

**Examples of games**

- Zero Sum game.

- Prison's delimma game (general form)
- Coordination

#### Nash Equilibrium Intro - Keynes Beauty Contest

**Pure Strategy Nash Equilibrium**  is a set of actions, one for each of the agents, such that each action is the **Best Response** against the equilibrium strategies of the other players. (such that no player would benefit by changing his own strategy (only **one** player changes at a time!), provided the other players don’t change their strategies.)

**Best response**.  an action ai is a best response, if for any other action, ai's utility is **greater** than utility of any other actions 

#### Strategy 

**dominant strategy**

``` asp
si strictly dominates s'i, if utility of si is strictly greater than utilities of all other possible strategies. 

A dominant strategy for a player is one that produces the highest payoff of any strategy available for every possible action by the other players.
```

**Very Weakly Dominate**

```brainfuck
si strictly dominates s'i, if utility of si is greater than or equal to utilities of all other possible strategies. 
```

**Dominant strategy**: if one strategy domiantes all others.

A stratey profile consisting of dominant strategies for every player must be a **Nash equilibrium**

#### Pareto Optimality

**Outcome**: a solve of the matrix game

**Pareto-dominate**: one outcome **O** is at least as good for every agent as another outcome **O' ((3,2) > (2,2)),**  and there's some agent who strictly prefers **O** to **O'**. We say that **O Pareto-dominates O'**

Definition of **Pareto Optimality**: An outcome is Pareto-optimal if there's no other outcome that Pareto-dominates it.

**Prisoner's Dilemma's Punch line:** The Nash equilibrium is the only non-Pareto-optimal outcome. 

## Paper Read: A Brief Introduction to the Basics of Game Theory Matthew O. Jackson, Stanford University

#### Framing the analysis: 

- Who are the players? 
- What actions are available to them? 

- what is the timing of the interactions? Are actions taken simultaneously or sequentially? Are interactions repeated? The order of play is also important. Moving after another player may give player i an advantage of knowing what the other player has done; it may also put player i at a disadvantage in terms of lost time or the ability to take some action. What information do different players have when they take actions?

- what are the payoffs to the various players as a result of the interaction?

#### Mixed Strategies

So a profile of mixed strategies is an equilibrium if no player has some strategy that would offer a better payoff than his or her mixed strategy in reply to the mixed strategies of the other players

#### Timing (Extensive Form)

**Use backward induction**



## Mixed Strategies and Nash Equilibrium

Strategy S for agent i is any probability distribution over the actions Ai.

- **Pure Strategy**: only one action is played with positive probability
- **Mixed Strategy**: more than one action is played with positive probability

**expected utility** of a mixed strategy is a weighted sum of all utilities times probability (Product of probabililties of each player playing their actions). 

**Best response**. A strategy s is a BR iff its utility is greater than utility of every other s'.

**(Mixed Strategy) Nash Equilibrium** (this is not Pure Strategy Nash Equilibrium) s = <s1,...sn> is a Nash equilibrium iff every other player is playing their best response

**Nash's Theorem**. Every **finite** (finite number of players, actions) game has a (Mixed Strategy) Nash equilibrium.

**Mixed Nash equilibrium** Compute the probability of each action so that it makes the other people indifferent about picking the actions. 

**Meaning of mixed strategies.** 

- Randomize to confuse your opponent (to be balanced)
- Randomize when uncertain about the other's action
- A concise description of what might happen in repeated play: count of pure strategies in the limit
- Describe population dynamics. 

 Computing Mixed Nash equilibrium is between P and NP. 

### Summary

**Pure Strategy Nash Equilibrium**  is a set of actions, one for each of the agents, such that each action is the **Best Response** against the equilibrium strategies of the other players. (such that no player would benefit by changing his own strategy (only **one** player changes at a time!), provided the other players don’t change their strategies.)

**Mixed Nash equilibrium** Compute the probability of each action so that it makes the other people indifferent about picking the actions. 