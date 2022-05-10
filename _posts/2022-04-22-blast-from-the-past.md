---
layout: post
title: Blast from the past - 3D
categories: [C#, Blender]
imageLink: "/assets/images/posts/blast-from-the-past/Random_Color_Castle.gif"
---
I collected my 3D works from my past. Mostly those will be images from Unity and Blender.

### Color randomization
Circa November 2020. 

![](/assets/images/posts/blast-from-the-past/Random_Color_Castle.gif)

It was made for my first prototype of game, that was about building a castles from bricks. I finished currently on prototype where I can destroy the castle using mouse pointer, which spawns ball. For now... 

### Blender - Weapon
Circa late 2020. Did it as assigment for my studies. I wanted to recreate rifle that looked cool to me. From multiple weapons I took WW2 Gewehr43 rifle, due to its cool looks, simple iron sights and easy shape.
#### Model limitations 
![](/assets/images/posts/blast-from-the-past/animation1.gif)

#### Reload
After that I worked on some animations that I would use in Unity. Most of them were things like firing, movement or reload. I was trying dealing with one cartrigde and cartridge boat reload, but after few not pretty looking attempts just finished on basic one.
![](/assets/images/posts/blast-from-the-past/animation4.gif)

#### Firing
Note that bullet casing can be procedurally coded into game so I don't need to animate it, only ejection point, where would bullet casing would spawn from.
![](/assets/images/posts/blast-from-the-past/animation2.gif)
#### Movement
![](/assets/images/posts/blast-from-the-past/animation3.gif)


### Blender - Modular Models
Here I tried to create some modular assets. This was for game that I ditched early on. It was supposed to be scare-sim, like **Ghost Master**. I needed two types of walls, one in full size and another cropped. Nowadays I would probably tried doing that with shader but back then I didn't know how to deal with things like that.
#### First Try
Circa late 2019
![](/assets/images/posts/blast-from-the-past/blender-bfp2019.PNG)

#### Second Try
Circa Semptember 2020
I grouped multiple models and tried to write some basic script using Blender flavoured Python. This time I was creating models for painting esque prototype, that I've never finished. For that project I was using Built-in render pipeline, as it was easier to modify texture via shader using RenderTexture compared to likes of URP back then.
![](/assets/images/posts/blast-from-the-past/blender-bfp2020.PNG)

For this project I had multiple uv maps prepared for every single modular piece. Three in total, one main, one light and one paint UV.
![](/assets/images/posts/blast-from-the-past/multiple-uv-maps.gif)