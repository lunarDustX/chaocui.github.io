---
title: Final Project
# type: page
description: Forest In Room
# topic: career
weight: 1
---

### Final Showcase

{{< rawhtml >}} 
  <iframe width="560" height="315" src="https://www.youtube.com/embed/ebR6B5H1GUs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
{{< /rawhtml >}}

### Project Description
The idea of this project is to explore the forest in your own room with the help of HoloLens. You could catch fireflies and interact with mushrooms in this project.

### Development Process
#### Firefly Catch
This was the first thing I made for this project, because firefly is a very typical forest element.   
{{< rawhtml >}} 
  <img src="/images/bugNet.png" alt="HTML5 Icon" width="300" height="300">
{{< /rawhtml >}}
At the beginning, I planned to use a real bug net to catch fireflies. But I quickly dropped this idea after a simple mock test. There are two main reasons.

{{< rawhtml >}} 
    <iframe width="560" height="315" src="https://www.youtube.com/embed/7k6gUihZ5Cs" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe> 
{{< /rawhtml >}}

1. The FOV of HoloLens is very limited. Your hand is easily out of vision when holding the net pole. Once HoloLens lose track of your hand, the virtual net collision won't work, because it relies on real time hand position data.
2. Catching a firefly by hands directly will encourage more body movement, makes the catching behaviour more "embodied". 

#### Leaves Generation
HoloLens has an amazing feature called "Spatial Mapping", that means HoloLens could detect real-world surfaces in the environment around. So I fetch those surface data, and generate leaves on vertices. In order not to cause serious performance problem, I use a super low mesh for the leaf, the "quad" in Unity. A quad only has 2 triangles, it's cheap.

{{< rawhtml >}} 
    <iframe width="560" height="315" src="https://www.youtube.com/embed/LTRAFk_wu_0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
{{< /rawhtml >}}

Later, I watched the tutorial below and made a shader for the leaves to make it looks better.

{{< rawhtml >}} 
  <iframe width="560" height="315" src="https://www.youtube.com/embed/kkAcGUR7pjQ" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
{{< /rawhtml >}}


#### Color The World
In order to make the whole experience more immersive, I try to paint the walls and surfaces with color. Then I realized an issue, all the colors you see through HoloLens are totally different than what you see in Unity. For example, the pure black in Unity will become totally transparent in HoloLens. This makes things super difficult. I hadn't made the color looks good at the end of the development. 
{{< rawhtml >}} 
  <img src="/images/wall-color.png" alt="HTML5 Icon" width="585" height="330">
{{< /rawhtml >}}

#### Mushroom
Mushroom was another typical forest vibe element I added to this project.

{{< rawhtml >}} 
  <img src="/images/mushroom.png" alt="HTML5 Icon" width="585" height="330">
{{< /rawhtml >}}

I tried a detailed model first, it looked pretty good, but caused a serious performance issue. So I had to use a low-poly version instead.   

I also made mushrooms interactable, because I always wanna feel the beautiful mushrooms with my hands when I walking in a real forest. Feedbacks are super important when you interact with virtual objects in an AR experience. I did following things to make the mushroom touching experience feels good:
* mushroom shrinking animation
* particle effect
* sound feedback

{{< rawhtml >}} 
    <iframe width="560" height="315" src="https://www.youtube.com/embed/vJa5HkqZib0" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
{{< /rawhtml >}}

#### THE END
I am very happy to play with HoloLens for the first time during the development of this project. Unfortunately, I am not an expert in shader and don't have enough time to solve the color rendering problem.  

{{< rawhtml >}} 
  <img src="/images/ideal.png" alt="HTML5 Icon" width="535" height="335">
{{< /rawhtml >}}



 
