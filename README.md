# chatbrains
![Test](https://github.com/MattChubb/chatbrains/workflows/Go/badge.svg?branch=master&event=push)
![CodeQL](https://github.com/MattChubb/chatbrains/workflows/CodeQL/badge.svg?branch=master&event=push)

Brains for use in chatbots

# Usage
Each "brain" type implements the following 3 methods
## Init
Initialise the brain with config
## Train
Train using the provided input
## Generate
Generate a response to the input

# Brain types
## Markov
A basic markov chain. Will attempt to figure out a relevant subject from the input, and generate from there using the chain
## Double Markov
Similar to Markov, but uses a backwards-propagating Markov chain in addition to a forward-propagating one to generate text either side of the subject.
