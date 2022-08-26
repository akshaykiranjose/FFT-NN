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

If ![x in R](https://latex.codecogs.com/gif.latex?x%20%5Cin%20%5Cmathbb%20R%5En) is an image in image space, and is ![K](https://latex.codecogs.com/gif.latex?K)-sparse in ![psi](https://latex.codecogs.com/gif.latex?%5CPsi),   then a measurement  ![y in Rp](https://latex.codecogs.com/gif.latex?y%20%5Cin%20%5Cmathbb%20R%5Ep) 
with   
![inequality](https://latex.codecogs.com/gif.latex?K%20%3C%20p%20%3C%3C%20n),  is given by ![equation](https://latex.codecogs.com/gif.latex?y%20%3D%20Cx).    
With knowledge of a sparse vector ![s](https://latex.codecogs.com/gif.latex?s) that satisfies the optimization problem  

![opt](https://latex.codecogs.com/gif.latex?%5Chat%7Bs%7D%20%3D%20%5Cunderset%7Bs%7D%7B%5Cmathrm%7Bargmin%7D%7D%5C%20%7C%7Cs%7C%7C_0%5C%20%5Ctextrm%7Bsubject%20to%7D%5C%20y%20%3D%20C%5CPsi%20s)  
can be used to reconstruct the original image.


View the HTML files by pasting the URL [here](https://htmlpreview.github.io/)
