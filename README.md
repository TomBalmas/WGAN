# WGAN
WGAN project for Machine Learning and Data mining course
# Some Notes About WGAN
### What IS GAN?
 - Generative Adversarial Network.
 - A network that learns to identify data and generate new data in the same fashion.
 ### GAN Architecture
- GAN consists of two neural networks</br>
Discriminator and Generator
### Discriminator (Critic)
 - The discriminator learns to distinguish the generator's fake data from real data.
 - The discriminator penalizes the generator for producing implausible results.
 ### Generator
 - The generator learns to generate plausible data.
 - The generated instances become negative training examples for the discriminator.
 ![GAN Architecture](https://i.ibb.co/K0pQZgb/Screenshot-2022-01-07-184140.png)
 
 ### Wasserstein Distance
 - Wasserstein  distance or Earth Mover’s(EM) - the minimum energy cost of transforming a pile of dirt from one probability distribution to the other distribution.
 - The cost is quantified by the amount of dirt moved.
 - Wasserstein metric provides a smooth measure, which is super helpful for a stable learning process using gradient descents.
 ### Kantorovich-Rubinstein duality
 - In WGAN, instead of using the EMD (the primary problem),we calculate the dual problem, due to high complexity.
### WGAN Elements
- In WGAN loss function is being used for computing gradient.
- In WGAN the model is more stable, and therefore prevents mode collapse.
- Vanishing gradients are less common.
#### Mode Collapse
The generator produces data from a small number of classes instead of all the classes.
## To Be Added
This implementation is on MNIST dataset, in the near future I will implement WGAN on a Pokémon images dataset 
## References
[WGAN article](https://arxiv.org/abs/1701.07875)</br>
[EMD duality](https://vincentherrmann.github.io/blog/wasserstein/)</br>
[WGAN implementation](https://machinelearningmastery.com/how-to-code-a-wasserstein-generative-adversarial-network-wgan-from-scratch/)</br>
[GAN](https://developers.google.com/machine-learning/gan/generator)</br>
[More about WGAN](https://medium.com/@sunnerli/the-story-about-wgan-784be5acd84c)</br>

 
 

