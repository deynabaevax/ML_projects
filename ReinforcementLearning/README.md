# The Snake Game with Reinforcement Learning
<p float="left">
    <img width="330px" src="https://media.geeksforgeeks.org/wp-content/uploads/20210611151042/Animation.gif"> 
    <img width="600px" src="https://miro.medium.com/max/1400/0*MvFeGltFQ3AHskQ2.jpg">
</p>

# Assignment Overview
The concept behind Reinforcement Learning (RL) is easy to grasp. An agent learns by interacting with an environment. The agent chooses an action, and receives feedback from the environment in the form of states (or observations) and rewards. This cycle continues forever or until the agent ends in a terminal state. Then a new episode of learning starts. Schematically, it looks like this:
<center><img width="400px" src="https://miro.medium.com/max/720/1*EAVTYNjkK7rgkryht5SQ0A.png"></center>
The goal of the agent is to maximize the sum of the rewards during an episode. In the beginning of the learning phase the agent explores a lot: it tries different actions in the same state. It needs this information to find the best actions possible for the states. When the learning continues, exploration decreases. Instead, the agent will exploit his moves: this means he will choose the action that maximizes the reward, based on his experience.

# Assignment Goal

> "Find a game you like and create a reinforcement agent that can play this game. This can be any game, but remember that you have to be able to access or being able to calculate the three main parameters of reinforcement learning: state, action and reward."

I will implement one of my favourite childhood games "the snake game". The goal is to grab as many apples as possible while not walking into a wall or the snake’s body. 

# Resuts
Below, a screenshot of how the training after few iterations looks like is provided.

![game-90](https://user-images.githubusercontent.com/64732465/196701290-408cd3db-40e0-4a38-830a-90d9d9a3ef18.png)


After training for some time, during the 271st game the record score increased to 67.

![271](https://user-images.githubusercontent.com/64732465/196701761-d89765f2-250a-43aa-8dd4-cba473dfda4d.png)

