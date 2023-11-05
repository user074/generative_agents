

# Demo of Generative Agents: Interactive Simulacra of Human Behavior for CSCI-GA.3033-102 Special Topic - Learning with Large Language and Vision Models


This repository is the demo code for the class. Please refer to "[Generative Agents: Interactive Simulacra of Human Behavior](https://github.com/joonspk-research/generative_agents)." for more documentation details. This repo modified the origional code for class demo purpose. It replaced the text-davinci-003 to gpt-3.5-turbo since it is cheaper — reduced cost like 10 times so it is feasible to run at a much acceptable cost. Running the demo for 1000-2000 steps might cost $1-$2 right now.
## Main Changes
- Replace the text-davinci-003 to gpt-3.5-turbo to reduce the cost
- Add a new memory to generate the classroom like environment
- Modified the map to trap everyone in the library
- Make agents to work 24/7 like robots

## Please follow the origional repo for Setting Up the Environment 

### During the step 2, please use the following file as the base if you want to generate the classroom like environment.
```
class_the_ville_isabella_maria_klaus
```
### Inject the memory from the agent_history_class.csv to the simulation by using the following command
First when prompt with 'Enter option: ', type the following command
```
run 1
```

So we can initialize the Personas objects. The origional code is a bit buggy and this is one way to work around it ("[Reference"](https://github.com/joonspk-research/generative_agents/issues/117)). 

Then after finishing running 1 step we can load our own injected memory into agents by using the following command
```
call -- load history the_ville/agent_history_class.csv
```

Then we can save and move on with the simulation.
 