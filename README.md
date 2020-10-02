# GAN(GENERATIVE ADVERSARIAL NETWORKS)

In an actual GAN, the counterfeit artist is represented by a generator network and the investigator by a discriminator network. The generator takes in a latent noise vector and attempts to generate an image (or sound, data, etc. — we say images because that’s what we used our GANs for but they can actually be used to model any kind of data), by attempting to model P(X|Y), where X represents the features, and Y represents a class. In other words, the generator attempts to model the distribution of an individual class. The generated image is then passed to the discriminator along with a stream of images from the ground-truth data set (non-generated images; i.e. real dogs). Ultimately, the discriminator models P(Y|X) and we expect the discriminator to accurately classify the ground-truth images as real and the generated images as fake. These two models exist in a double feedback loop. The discriminator is in a feedback loop with the ground-truth data set and the generated images, while the generator is in a feedback loop with the discriminator.

