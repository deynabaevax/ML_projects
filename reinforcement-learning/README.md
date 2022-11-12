# The Snake Game with Reinforcement Learning
<p float="left">
    <img width="330px" src="https://media.geeksforgeeks.org/wp-content/uploads/20210611151042/Animation.gif"> 
    <img width="600px" src="https://miro.medium.com/max/1400/0*MvFeGltFQ3AHskQ2.jpg">
</p>

# Assignment Overview
The concept behind Reinforcement Learning (RL) is easy to grasp. An agent learns by interacting with an environment. The agent chooses an action, and receives feedback from the environment in the form of states (or observations) and rewards. This cycle continues forever or until the agent ends in a terminal state. Then a new episode of learning starts. I made a quick sketch to visualize it:

<img width="700px" src="https://user-images.githubusercontent.com/64732465/201480046-03f30710-843a-4ffa-80cb-62fb214c9521.jpg">

The goal of the agent is to maximize the sum of the rewards during an episode. In the beginning of the learning phase the agent explores a lot: it tries different actions in the same state. It needs this information to find the best actions possible for the states. When the learning continues, exploration decreases. Instead, the agent will exploit his moves: this means he will choose the action that maximizes the reward, based on his experience.

# Assignment Goal

> "Find a game you like and create a reinforcement agent that can play this game. This can be any game, but remember that you have to be able to access or being able to calculate the three main parameters of reinforcement learning: state, action and reward."

I will implement one of my favourite childhood games "the snake game". The goal is to grab as many apples as possible while not walking into a wall or the snake’s body. 

# Set-up

For this assignment I used VS Code as IDE. I installed **pygame**, which is a Python package for writing games.

# Observations
- Snake Played by the Agent
  It was very interesting to look at the agent learning to play the game. At first the agent had no clue what was happening and was going around the environment. It took more than 100 plays to get a "more satisfying" score of 30.

# Results

Below, a screenshot of how the training after few iterations looks like is provided.

![game-90](https://user-images.githubusercontent.com/64732465/196701290-408cd3db-40e0-4a38-830a-90d9d9a3ef18.png)

After training for some time, during the 251st game the record score increased to 68.
<img src="https://user-images.githubusercontent.com/64732465/201484835-b1b0955b-2ef4-443d-b1a5-90bcd9247dec.gif">


After training the agent for more than 469 games, the record was 90.
<img src="https://user-images.githubusercontent.com/64732465/201484770-185c89cd-6ed2-4ade-aa69-eaeca66ec482.gif">

# Conclusion

Reinforcement Learning is a very interesting part of AI because instead of using supervised or unsupervised learning to learn, it does this by being in a dynamic environment which is based on rewards and punishments. With this exercise, I was able to create a snake game, which was trained to obtain satisfying results in the end.

