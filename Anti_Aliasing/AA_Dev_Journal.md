# Anti Aliasing

**Technical Art**  

**Syed Hashim Hussain**  

**2108002**  

 

## **Research**

#### Anti Aliasing

Anti Aliasing is the technique used to remove the problem of jagged and uneven edges caused by colours being rendered incorrectly because of a pixel containing more or less information.

## **Types of AA**

### Fast Aprproximate Anti-Aliasing
FXAA can be considered the fastest AA method being used as it doesn't have a huge priority to image quality. This is why it is commonly used for lower end hardware. While using this performance has little issues, due to image after rendereing is changed, the image quality isn't considered 
### Super Sampling Anti-Aliasing 

This is the proccess of the GPU calculating the current scene in a higher resolution, and then correcting it to the resolution it should be. This will then allow the GPU to collect more samples of each pixel. Unfortunately, it isn't considered a good practice as it is taking extra work for the GPU to produce these samples and would affect the frame rate negatively compared to how much work it takes to produce the scene.

### Mutli Sample Anti-Aliasing

This technique is very similar to *Super Sampling AA*. It still takes a higher resolution than normal, *However*, it only takes the sample in the rasterisation phase (when a 3D object is processed into a 2D image). It in essense is performing Super Sampling in a more efficient way by focusing just the edges of the scene, where the Anti-Aliasing is needed the most.

### Post Proccessing Anti-Aliasing 

When it comes to performance, MSAA and SSAA is very costly, so this is where people can implenent Post Proccessing AA. It doesn't have as good quality as other types of Anti Aliasing but is greatly increases performance. This method goes about by using the final image of the rendered scene and uses different techniques to blur the aliasing.

### Temporal Anti-Aliasing 

This is a very commonly used Anti-Aliasing Technique in video games and real time applications. In simple terms, this techinique will blend the past frames with the current frame. This form of AA is very good when it comes to fast moving scenes

## **Source**

Luckily, I was able to find a range of sources for this task, all ranging from a comparison of techiniques and some examples that deep dive into a single technique. 

Starting off with the source that was used the most for all the definitions - (Comparison and Analysis between Different Versions of FXAA | IEEE Conference Publication | IEEE Xplore, s.d.) This was a great source for this topic, as the publisher is one of the biggest leading technilogical organisations. It provided me an insight on many different types of AA, inluding "Super Sampling Anti-Aliasing" and "Post Proccessing Anti-Aliasing".  


### Testing different Anti Aliasing Methods
<iframe width="560" height="315" src="https://www.youtube.com/embed/14xDcDIbAT0?si=hNmUY5O0YislzomT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/-KsjrGQ8Z44?si=JcJs7LZTrXAKQIhd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/5pfEjXz_YRs?si=p2ieM_pvpWxBXJzD" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

<iframe width="560" height="315" src="https://www.youtube.com/embed/YFO_xAyOVYY?si=6sBNenkIXFSmZSJu" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

## **Bibliography**

Caulfield, B. (2018) What’s the Difference Between Ray Tracing and Rasterization? At: https://blogs.nvidia.com/blog/whats-difference-between-ray-tracing-rasterization/ (Accessed  10/10/2024).

Comparison and Analysis between Different Versions of FXAA | IEEE Conference Publication | IEEE Xplore (s.d.) At: https://ieeexplore.ieee.org/abstract/document/9730249 (Accessed  10/10/2024).

Lottes, T. (s.d.) 'Version Date Responsible Reason for Change' | At: https://developer.download.nvidia.com/assets/gamedev/files/sdk/11/FXAA_WhitePaper.pdf (Accessed 11/10/2024)

Nah, J.-H., Ki, S., Lim, Y., Park, J. and Shin, C. (2016) 'AXAA: adaptive approximate anti-aliasing' In: ACM SIGGRAPH 2016 Posters. SIGGRAPH ’16: Special Interest Group on Computer Graphics and Interactive Techniques Conference. Anaheim California: ACM. pp.1–2. At: https://dl.acm.org/doi/10.1145/2945078.2945129 (Accessed  16/10/2024).

Yang, L., Liu, S. and Salvi, M. (2020) 'A Survey of Temporal Antialiasing Techniques' In: Computer Graphics Forum 39 (2) pp.607–621. | At: https://onlinelibrary.wiley.com/doi/pdfdirect/10.1111/cgf.14018 (Accessed 13/10/2024)

