## Generative Adversarial Networks (GAN) ##
The GAN architecture was first described in the 2014 paper by Ian Goodfellow, et al. titled “Generative Adversarial Networks.”
These are generative models that when trained upon real data can generate new 'fake' data
Consisting of 2 neural networks, namely - Generator and Dicriminator work in a constant adversarial loop with respect to each other, hence improving upon both.

The generator model takes a fixed-length random vector as input and generates a sample in the domain.
The vector is drawn from randomly from a **Gaussian distribution**, and the vector is used to seed the generative process. After training, points in this multidimensional vector space will correspond to points in the problem domain, forming a compressed representation of the data distribution.
This vector space is referred to as a latent space, or a vector space comprised of latent variables. **Latent variables**, or hidden variables, are those variables that are important for a domain but are not directly observable.

Discriminator judges this newly gen data to be real or fake
If one component makes a wrong descision(a desicion with negative output) it continues to improve upon whereas the other component stays unchanged
This results into a **zero-sum game**.

![GAN Model Image](https://github.com/ChiragRajput101/GAN-Image-Gen/assets/97492118/9382c294-d096-4854-b542-0c26c4333fbc)
