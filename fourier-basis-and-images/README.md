# fourier basis: images and signals
## Image Reconstruction via Fourier Basis and Compressed Sensing

### Traditional Image Compression and Reconstruction

1.take a high resolution image and 2D fourier transform it;  
2.throw most of the transform data away;  
3.inverse 2D fourier it with the remaining data samples.    
4.a decent reconstruction of the original image is obtained.  

### Compressed sensing of images

Instead of collecting a high-dimensional measurement and then compressing,  
acquire compressed measurements and solve for the sparsest high-dimensional  
signal that is consistent with the measurements.  

If $x \in \mathbb{R}^{n}$ is an image in image space, and is $K$-sparse in $\Psi$, then a measurement $y \in \mathbb{R}^{p}$ with   
$K << p< n$,  is given by $y=Cx$.  
With knowledge of a sparse vector $s$ that satisfies the optimization problem

$\hat{s} = \underset{s}{{argmin}} ||s||_0 \ \text{subject to} \ y = C\Psi s$
can be used to reconstruct the original image.


## Signal Restoration by beating Nyquist Rate 

### An example from Wikipedia
![Alt Text](https://upload.wikimedia.org/wikipedia/commons/3/38/Orthogonal_Matching_Pursuit.gif)

### Original Signal and its random samples
<img src="figures/samples and PSD.png" >

### compressed sensing restoration via CoSaMP
<img src="figures/CoSaMP reconstruction samples and PSD.png" >

### compressed sensing restoration via Linear Program
<img src="figures/linprog reconstruction samples and PSD.png" >
