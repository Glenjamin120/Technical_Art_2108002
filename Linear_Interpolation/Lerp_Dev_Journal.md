# Linear Interpolation

**Technical Art**

**Syed Hashim Hussain**

**2108002**

### Research

The mathematical function Linear Interpolate is a very useful function when it comes to game development. Even though it is a very simple process of blending "between two input value(s)
based on a third input value used as a mask", it is widely used for many things such as smoothing the movement of a camera, blending between textures and colours, making movements smooth and a range of other applications.

#### Inputs

The lerp node takes three inputs: **Input A**, **Input B** and **Alpha** . All of these will be default 0.0 unless edited or has a connection. 

#### Basic Use

A very common framework use of this node will be adding two inputs and using the alpha to blend the two inputs together. By having the alpha at 0.0, you will have 100% of input A. By having the alpha at 1.0, you will have the 100% of input B. By adjusting the alpha, you can change how much of the result is blended between the two inputs. The following examples are two example that use different methods of controlling the Alpha to have two different outcomes.

```
https://dev.epicgames.com/documentation/en-us/unreal-engine/math-material-expressions-in-unreal-engine#linearinterpolate
source for lerp definition. Add to zotero

```
### Example 1
<iframe width="560" height="315" src="https://www.youtube.com/embed/iuozOQjvsVQ?si=xpK9H_-zGJxwbpNd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Example 2

<iframe width="560" height="315" src="https://www.youtube.com/embed/0sCndNcAG5I?si=aB4WS1ksf8Bs-drT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>
