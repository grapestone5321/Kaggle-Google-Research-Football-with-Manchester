# Kaggle-Google-Research-Football-with-Manchester
Kaggle-Google-Research-Football-with-Manchester


### Final Submission Deadline: 
November 30, 2020 11:59pm UTC



### Final Games Played: 
December 1 - December 7, 2020

### End Date: 
December 7, 2020 11:59pm


In this competition, you’ll create AI agents that can play football. 

Teams compete in “steps,” where agents react to a game state. Each agent in an 11 vs 11 game controls a single active player and takes actions to improve their team’s situation. 

As with a typical football game, you want your team to score more than the other side. 

You can optionally see your efforts rendered in a physics-based 3D football simulation.


## GitHub: Google Research Football
https://github.com/google-research/football


## Getting Started with Gym
https://gym.openai.com/docs/#available-environments


## GFootball with Memory Patterns
https://www.kaggle.com/yegorbiryukov/gfootball-with-memory-patterns

### Explanation of The Architecture

- In agent function data of the current environment is modified and get_action_of_agent function is called to get the action that will be returned.

- In get_action_of_agent function list of memory patterns is provided by find_patterns function, then action of the first memory pattern in that list, whose constraints are met by current environment, is returned.

- All Groups of Memory Patterns and all Memory Patterns are just functions that are taking the same arguments: obs, player_x, player_y and return a dictionary with at least two functions.

- First function in that dictionary for both Groups of Memory Patterns and Memory Patterns is environment_fits, it returns True or False, in case constraints described in this function are met by current environment or not. If this function returns True, than the Group of Memory Patterns or Memory Pattern it belongs to is selected for future processing. If this function returns False, than search for appropriate Group of Memory Patterns or Memory Pattern continues.

- Second function is called only when this Group of Memory Patterns or Memory Pattern was selected for future processing. In any Group of Memory Patterns the second function is get_memory_patterns that return list of memory patterns. In any Memory Pattern the second function is get_action that return action of the memory pattern it belongs to.

- In all Groups of Memory Patterns and all Memory Patterns functions environment_fits, get_memory_patterns and get_action take obs, player_x, player_y as arguments.

### Install Required Tools

### Functions and Imports

### Offence Memory Patterns
I suggest keeping them in alphabetical order

### Memory Patterns Suitable for any Environment
I suggest keeping them in alphabetical order


### Memory Patterns of Special Game Modes
I suggest keeping them in alphabetical order


### Groups of Memory Patterns
I suggest keeping them in alphabetical order


### Global Variables
I suggest keeping them in alphabetical order

### Agent
Detailed description of the GFootball observations is available here.


### Play Game







