# Generative Adversarial Networks (GANs)

GANs can be used to generate synthetic (i.e., fake) images that are perceptually near identical to their ground-truth, authentic originals.

In order to generate synthetic images, two neural networks have been used during training:

* A generator accepting an input vector of randomly generated noise and produces an output `imitation` image that looks similar, if not identical to an authentic image
* A discriminator or adversary attempting to determine if a given image is an `authentic` or `fake`

GANs are notoriously hard to train due to an evolving loss landscape. At each iteration of the algorithm I am:

* Generating random images and then training the discriminator to correctly distinguish the two
* Generating additional synthetic images, but this time purposely trying to fool the discriminator
* Updating the weights of the generator based on the feedback of the discriminator, thereby allowing to generate more authentic images

## Developer

Baishali Dutta (<a href='mailto:me@itsbaishali.com'>me@itsbaishali.com</a>)

## License [![License](http://img.shields.io/badge/license-Apache-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)

This project is licensed under Apache License Version 2.0
