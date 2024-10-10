# Anti Aliasing

**Technical Art**  

**Syed Hashim Hussain**  

**2108002**  

# 

### **Research**

#### Anti Aliasing

Anti Aliasing is the technique used to remove the problem of jagged and uneven edges caused by colours being rendered incorrectly because of a pixel containing more or less information.

## Types of AA
### Super Sampling Anti-Aliasing 

This is the proccess of the GPU calculating the current scene in a higher resolution, and then correcting it to the resolution it should be. This will then allow the GPU to collect more samples of each pixel. Unfortunately, it isn't considered a good practice as it is taking extra work for the GPU to produce these samples and would affect the frame rate negatively compared to how much work it takes to produce the scene.

### Mutli Sample Anti-Aliasing

This technique is very similar to *Super Sampling AA*. It still takes a higher resolution than normal, *However*, it only takes the sample in the rasterisation phase (when a 3D object is processed into a 2D image). It in essense is performing Super Sampling in a more efficient way by focusing just the edges of the scene, where the Anti-Aliasing is needed the most.




### Testing different Anti Aliasing Methods
https://github.com/user-attachments/assets/caa605af-b0c9-4281-aaac-7994dc63250b

https://github.com/user-attachments/assets/bd8a7613-ab16-4858-bd9a-a2207d3e1a7b

https://github.com/user-attachments/assets/4c12e6eb-fd11-4011-974a-15b3cf5c6390

https://github.com/user-attachments/assets/b901810a-5f21-4ca4-9767-84a19e668c20
