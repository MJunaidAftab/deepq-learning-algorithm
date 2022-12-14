# deepq-learning-algorithm

# A Comparison Between Recurrent and Non-recurrent Deep Q-Networks in a GridWorld Survival Game

## Description

This repository contains code we implemented as part of the couse project for CMSC 727: Neural Modelling taught by James Reggia at University of Maryland, College Park. 

We implemented the deep Q-learning algorithm to examine the the discrepancy between recurrent and non-recurrent neural
networks for the purpose of Q-learning in a survival-focused GridWorld game. Our study compared the two architectures’ ability to guarantee a
high rate of “survival” (subject to our definition of this objective) in randomly generated grid environments that share basic inherent properties.

A description of the various files uploaded is as follows:

1. The file ```grid.py``` generates a two-dimensional grid wolrd populated with the virtual agent, enemies, food and obstacles/walls. 
   The `grid.py` file takes in the following parameters:
   
   - `worldsize:` Dimensions of the grid world
   - `frac_fill:` Fraction filled with walls
   - `num_enemies:` Number of enemies
   - `num_food:` Number of food
   - `input_energy:` Agent's input energy
   - `food_energy:` Energy per food
   - `s_range:` Enemy sight range when vision not blocked by wall
   - `agent_s_range:` Agent sight range

   - `move_reward:` Reward for moving
   - `food_reward:` Reward for acquiring food
   - `wall_reward:` Reward for hitting wall
   - `death_reward:` Reward for dying
   - `survive_reward:` Reward for surviving
   - `enemy_reward:` Reward for being eaten by enemy

   Here is a sample [image](images/grid.png) of what the `gird.py` file geneates.
   

2. The file `network.py`uses `PyTorch` to both the forward pass of a feedforward and convolutional neural network.

## Getting Started

### Dependencies

* Describe any prerequisites, libraries, OS version, etc., needed before installing program.
* ex. Windows 10

### Installing

* How/where to download your program
* Any modifications needed to be made to files/folders

### Executing program

* How to run the program
* Step-by-step bullets
```
code blocks for commands
```

## Help

Any advise for common problems or issues.
```
command to run if program contains helper info
```

## Authors

Contributors names and contact info

ex. Dominique Pizzie  
ex. [@DomPizzie](https://twitter.com/dompizzie)

## Version History

* 0.2
    * Various bug fixes and optimizations
    * See [commit change]() or See [release history]()
* 0.1
    * Initial Release

## License

This project is licensed under the [NAME HERE] License - see the LICENSE.md file for details

## Acknowledgments

Inspiration, code snippets, etc.
* [awesome-readme](https://github.com/matiassingers/awesome-readme)
* [PurpleBooth](https://gist.github.com/PurpleBooth/109311bb0361f32d87a2)
* [dbader](https://github.com/dbader/readme-template)
* [zenorocha](https://gist.github.com/zenorocha/4526327)
* [fvcproductions](https://gist.github.com/fvcproductions/1bfc2d4aecb01a834b46)
