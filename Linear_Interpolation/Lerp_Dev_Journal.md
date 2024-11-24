# Linear Interpolation

**Technical Art**

**Syed Hashim Hussain**

**2108002**

### Research

Lerp itself is a mathematical function that can be used in a wide variety of ways, below is the mathematical equation.
```
Lerp(A, B, Alpha) = A + (B - A) * Alpha
```
The mathematical function Linear Interpolate is a very useful function when it comes to game development. Even though it is a very simple process of blending "between two input value(s) based on a third input value used as a mask", it is widely used for many things such as smoothing the movement of a camera, blending between textures and colours, making movements smooth and a range of other applications. When using lerp, it is important to taken into consideration how impactful it will on your game.

There are ways to use interpolation in a way that optimizes performance, for example "In practice, interpolation polynomials are the most often used. The advantage is that polynomials are good in complex function approximations, easy to calculate and find derivatives." This example here uses linear interpolation and bilinear interpolation for their simplicity, which allows for quicker calculations which is ideal for real-time applications.

#### Inputs

The lerp node takes three inputs: **Input A**, **Input B** and **Alpha** . All of these will be default 0.0 unless edited or has a connection. 

#### Basic Use

A very common framework use of this node will be adding two inputs and using the alpha to blend the two inputs together. When the alpha is set to 0.0, you will have 100% of input A. if set to 1.0, you will have the 100% of input B. By adjusting the alpha, you can change how much of the result is blended between the two inputs. The following examples are two example that use different methods of controlling the Alpha to have two different outcomes.

### Example 1
<iframe width="560" height="315" src="https://www.youtube.com/embed/iuozOQjvsVQ?si=xpK9H_-zGJxwbpNd" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### Example 2
<iframe width="560" height="315" src="https://www.youtube.com/embed/0sCndNcAG5I?si=aB4WS1ksf8Bs-drT" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" referrerpolicy="strict-origin-when-cross-origin" allowfullscreen></iframe>

### **Implementation**

In Example 1, I have used a cosine value to demonstrate how a lerp can be used to change a texture in a material. The value is switching between two different noise nodes and the alpha is being controlled by a cosine node, which allows for a very cool looking material.
<iframe src="https://blueprintue.com/render/l2qe70sd/" scrolling="no" allowfullscreen></iframe>

In Example 2, I have created a texture which is similar to the First example, but it differs as it uses user input to change between textures and it also uses illumination.
<iframe src="https://blueprintue.com/render/nfirnlts/" scrolling="no" allowfullscreen></iframe>
