# flappy_NN
Title: Evolution of Flappy Bird Playing Neural Networks using NEAT Algorithm

Introduction:
In the world of artificial intelligence and machine learning, one of the most fascinating applications is the development of intelligent agents that can learn and adapt to play video games. One such example is the popular game Flappy Bird, where players control a bird that must navigate through a series of pipes by jumping at the right time. While this may seem like a simple task for humans, it poses a significant challenge for AI-based agents. In this essay, we explore the implementation of a neural network-based AI agent that learns to play Flappy Bird using the NEAT (NeuroEvolution of Augmenting Topologies) algorithm.

The Flappy Bird Game:
Before delving into the technical details, let's first understand the Flappy Bird game itself. The game environment is created using the Pygame library, which handles graphics and rendering. The player controls a bird represented by a sprite and must avoid crashing into pipes that appear at varying heights on the screen. As the game progresses, the pipes move from right to left, creating an ever-increasing challenge for the player.

NEAT Algorithm Overview:
NEAT is a popular algorithm for evolving neural networks in artificial intelligence. It stands for NeuroEvolution of Augmenting Topologies, and it was proposed by Kenneth O. Stanley and Risto Miikkulainen in 2002. The algorithm allows neural networks to evolve by combining the principles of genetic algorithms and neuroevolution. NEAT achieves this by evolving both the structure (topology) and weights of the neural network.

The Bird Class:
In the Flappy Bird AI implementation, the Bird class represents the bird in the game. It has various attributes, including position, tilt, velocity, and animation. The `jump` method enables the bird to move upward when the player makes it jump. The `move` method is responsible for updating the bird's position based on the velocity and gravity of the game. The `draw` method renders the bird sprite on the game screen with animation, creating the illusion of flight.

The Pipe Class:
To create the challenging obstacles in the game, the Pipe class is introduced. It represents the pipes that the bird must navigate through. Pipes are initialized with a random height, and as the game progresses, they move from right to left. The `collide` method checks for collision between the bird and the pipes, determining if the bird has collided with them, resulting in a game over.

Base and Scoring:
The Base class represents the base of the game environment, which moves continuously from right to left, creating the illusion of movement. The scoring mechanism tracks the player's performance by incrementing the score whenever the bird successfully passes through a pair of pipes.

Evolving Neural Networks with NEAT:
The main part of the Flappy Bird AI implementation lies in the `main` function. It takes genomes (representing neural networks), configuration, and runs the game while evolving the neural networks using the NEAT algorithm. Each bird in the game is associated with a genome, representing a neural network. During gameplay, the neural networks are provided with inputs based on the bird's position and the distance to the pipes. The neural networks then output a decision to jump or not.

The NEAT algorithm works by evaluating the fitness of each neural network based on its performance in the game. Higher fitness is assigned to neural networks that achieve better scores or stay alive longer. The fittest neural networks are then selected for reproduction, and new generations of neural networks are created by applying genetic operators such as mutation and crossover. This process continues for multiple generations, gradually improving the neural networks' ability to play the game.

Conclusion:
The implementation of a Flappy Bird playing AI using the NEAT algorithm showcases the power of evolutionary algorithms in training neural networks to perform complex tasks. By combining genetic algorithms and neuroevolution, NEAT allows for the development of sophisticated AI agents that can learn to play games like Flappy Bird, where human-like intuition and reflexes are required. This project serves as an excellent example of how AI can be applied to the realm of entertainment and gaming, paving the way for even more exciting possibilities in the future.

[Link to Video Example of AI running flappy bird](https://youtu.be/tWGnCBuKjTA)
