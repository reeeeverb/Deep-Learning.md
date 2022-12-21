#### Resources
- [[An Introduction to Reinforcement Learning]]: Sutton and Barto 
	- big ideas overarching ideas 
- [[Algorithmns for Reinforcement Learning]]: Szepesvari
	- less than 100 pages, mathematical understanding

#### What is Reinforcement Learning
- the sceince of decision making
- there is no supervisor, only a reward signal
- feedback is delayed, not instantaneously 
- time is very important, sequential 
	- actions affect future data it recieves

**Reward Hypothesis** all goals can be described by the maximisation of expected cumulative reward
**State** is the information used to detertmine what happens next, a function of the history

#### Markov States
- contains all useful information from the history 
- the future is indepedent of the past given the present
- past gives you no more information than the Markov State
	- aka information state

#### Full vs Partial Observability 
- Full Observability Agent state = enviorment state = information sttate 
	- this is a  makrov decision process
- partial ovservability: agent indirectly ovserves enviornment
	- isnt told its absolute state 
	- agent state != enviorment state
	- beliefs(proabablity) of current state

## The Agent

#### Policy 
- the agents behavior 
- it is a map from state to action 
	- deterministic policy a =  p(s)
	- stochastic policy: probability of taking certain action 

#### Value Function 
- predicition of future reward 
- used to evaluate the goodness/badness of a state 

#### Models 
- predicts what the enviorment will do next 
- *transition models* predicts the next state (dynamics)
- *reward models* predicts the next immediate reward

Value based agents have no policty, just value fns
Model free agents have no models, just policy and/or value function