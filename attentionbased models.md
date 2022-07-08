### Today's tasks: 

- [ ] watch the tutorials about pytorch transformer
  - [ ] Make notes on the different types of attentions
  - [ ] set up a simple transformer based model
- [ ] Find the evaluation scripts for the generated lyrics
- [ ] (optional) ethics review docs
  - [ ] about how to set up the google forms 
  - [ ] make diagrams 

-----

## Attention 

### Classification

- self/cross 
- hard/soft

### self-attention

Given a sequence as follows:

$\{{x_i}\}^{t}_{i=1} = \{{x_1,x_2,...,x_t}\} \leadsto X \in \mathbb{R}^{n \times t }$

to get the linear combination of the items in the set

$\boldsymbol{h} = \alpha_{1}x_1 +\alpha_{2}x_2 +...+ \alpha_{t}x_t = Xa \in \mathbb{R}^{n}$ (Here is a dot product and the $\bf{a}$ is a vector consisting of $\alpha$s)

#### soft-attention: 

$||a||_{1}=1$ (which means the sum of all the absolute values of the items)

- similar to probability distribution, sum up to 1.

#### hard-attention:

$||a||_{0}=1$ (which means the number of non-zero values in a)

- similar to one-hot encoding, just has  one value is 1, others are 0s



User cases:

$\mathbf{a} = [soft] (arg) max_\beta(X^{T}x) \in \mathbb{R}^{n}$

















