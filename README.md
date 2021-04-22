# MinimumValue_Using_GeneticAlgorithm
This Program will find the Minimum Value of some Dataset, using Genetic Algorithm Method to find the minimum value of the Formula

![Rumus](https://user-images.githubusercontent.com/42132479/115751498-71e95780-a3c3-11eb-8086-4065ea17a987.PNG)

# The Dataset
The Data is consist of some randomly generated binary encoding with a total length of 32 element/bit for each of its chromosomes

# Decode The Chromosome
to decode the chromosome of the binary type, I applied the following formula and broke it down into
Some parts in a Bgst() function to determine the x1, x2 phenotype of a
chromosomes which will later become parameters for other functions

![image](https://user-images.githubusercontent.com/42132479/115751975-de645680-a3c3-11eb-9e99-88f8d8e84cd8.png)

# Fitness Score
I calculated the Fitness of a chromosome after getting the x1, x2 phenotype of a
chromosome

# Parental Selection, Crossover & Mutation
The crossover was carried out after the selection of two parent candidates that I chose based on fitness scores
best in its generation, the probability of occurrence of crossovers that I use is 70% with
the single-point method is set to be in the middle of the total length of a chromosome ie
index to 16. The elements are cut into the front and back, then combined so that
L
produces new chromosomal offspring. If the probability is not met, the first parent will be copied to
become the new chromosome child.

# Alternation of Generations
The generational replacement method that I use is generational replacement in each generation
Elitism is carried out where the two chromosomes with the highest fitness value are ensured to be in the generation
Furthermore, the crossover & mutation results from the selected parent will fulfill the generational pool
I save it in an array variable. The alternation of generations will occur at the end of the iteration indicated by
The old population will be replaced by a new population containing elite chromosomes and children from the parent
the chosen.

# Termination of Evolution
Evolution was stopped after the maximum generation limit was reached, I applied this method so that
termination of evolution can be arranged easily by only changing the value of one variable

# The Output
![image](https://user-images.githubusercontent.com/42132479/115752499-5af73500-a3c4-11eb-8c78-6f58368b1376.png)
