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

### Post Proccessing Anti-Aliasing 

When it comes to performance, MSAA and SSAA is very costly, so this is where people can implenent Post Proccessing AA. It doesn't have as good quality as other types of Anti Aliasing but is greatly increases performance. This method goes about by using the final image of the rendered scene and uses different techniques to blur the aliasing.

### TAA 

This is a very commonly used Anti-Aliasing Technique in video games and real time applications. In simple terms, this techinique will blend the past frames with the current frame. This form of AA is very good when it comes to fast moving scenes



### Testing different Anti Aliasing Methods
<iframe width="560" height="315" src="https://youtu.be/14xDcDIbAT0?si=hNmUY5O0YislzomT" 
title="FXAA" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" 
allowfullscreen></iframe>

<iframe src="https://youtu.be/-KsjrGQ8Z44?si=b8KJN0ZKKUv0-_0s" title="MSAA"></iframe>

<iframe src="https://youtu.be/5pfEjXz_YRs?si=Alnbu5g-y8Ts7UDr" title="No AA"></iframe>

<iframe src="https://youtu.be/YFO_xAyOVYY?si=E-O0Xx5x4RP7Rzbl" title="TAA"></iframe>
