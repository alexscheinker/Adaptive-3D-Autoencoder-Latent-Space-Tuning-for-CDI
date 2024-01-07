The goal of a CDI experiment is the reconstruction of the 3D electron density of a sample $d(\mathbf{r}) = \rho(\mathbf{r})e^{i\phi(\mathbf{r})}$, where $\rho(\mathbf{r})$ defines the object's shape and $\phi(\mathbf{r})$ is a phase field defining atomic dislocations, where $\mathbf{r} = (x,y,z)$. The object could be directly reconstructed by an inverse Fourier transform if it was possible to record the complex diffracted scalar wavefield $\psi(\mathbf{w}) = \left | \psi(\mathbf{w}) \right | \exp \left [ i \varphi(\mathbf{w}) \right ]$, which is related to the Fourier transform of the electron density of the sample, where $\mathbf{w} = (w_x,w_y,w_z)$ defines reciprocal space coordinates. In practice, what is recorded on a detector is the intensity of the diffracted light, given by
$$I(\mathbf{w}) = \iint \rho(\mathbf{r}_1)\rho^\star(\mathbf{r}_2)\exp\left [ i \mathbf{q} \left ( \mathbf{r}_1 - \mathbf{r}_2 \right ) \right ] d\mathbf{r}_1d\mathbf{r}_2$$
$$=\left | \psi(\mathbf{w}) \right |^2 \exp \left [ i \varphi(\mathbf{w}) \right ] \exp \left [ -i \varphi(\mathbf{w}) \right ]$$
$$=\left | \psi(\mathbf{w}) \right |^2.$$

We utilize a 3D convolutional neural network-based autoencoder to map intensities of coherent diffraction imaging (CDI) X-ray diffraction patterns to the 3D electron densities form which they were generated.

Movie of generated electron densities $d(\mathbf{r}) = \rho(\mathbf{r})e^{i\phi(\mathbf{r})}$ when moving through the autoencoder's latent space:


https://github.com/alexscheinker/Adaptive-3D-Autoencoder-Latent-Space-Tuning-for-CDI/assets/3331022/b0f572ca-b06c-491a-8f02-f9070a5bbba1


Another movie of generated electron densities $d(\mathbf{r}) = \rho(\mathbf{r})e^{i\phi(\mathbf{r})}$ when moving through the autoencoder's latent space:


https://github.com/alexscheinker/Adaptive-3D-Autoencoder-Latent-Space-Tuning-for-CDI/assets/3331022/72232b81-384f-4004-b194-21bfc62385af


Movie of adaptive tracking of a time-varying $d(\mathbf{r},t)$:


https://github.com/alexscheinker/Adaptive-3D-Autoencoder-Latent-Space-Tuning-for-CDI/assets/3331022/dd73dc7b-a4dd-4ed4-9a2d-29122c6f3b6f

