---
layout: project
name: "Parcels"
title: "Parcels"
permalink: "projects/parcels/"
game-engine: "PogEngine"
start-date: 2021-09-01
end-date: 2022-04-01
school-project: True
school: DigiPen Institute of Technology Singapore
module: Software Engineering Project 3-4
description: A 2D Point and Click Adventure Game with Visual Novel elements.
last-updated: 02-07-2023
---

<style>
    body {
        color: white; /* Change the text color to red */
        background-image: url("/images/Parcels/bg.jpg");
        background-attachment: fixed;
        background-position: 0% 0%;
        background-repeat: no-repeat;
        background-size: cover;
        position: relative;
    }

      a{
        color: #ff0000;
    }
    a:visited {
        color: #ff0000;  
}
</style>

<img src="/images/Parcels/game-logo.jpg" width="100%" height="100%">

Parcels is a 2.5D point-n-click narrative adventure game that follows Greg, a deliveryman who has wound up in an unknown place. Deliver parcels and talk to your recipients to learn about the world that you woke up in and all the strange happenings around the world!

<div style="text-align: center;">
  <img src="/images/Parcels/team_logo.png" width="50%" height="50%">
  <div>
    <i>Pog Studios logo.</i>
  </div>
</div>

# <b>Table of Contents
- [Gameplay Showcase](#gameplay_showcase)
- [Engine Showcase](#engine_showcase)
- [Development](#development)
    - [Introduction](#introduction)
    - [Features](#features)
    - [Tools](#tools)
    - [Libraries](#libraries)
    - [Contribution](#contributions)
        - [Graphics](#)
        - [Editor](#)
        - [Gameplay](#)
- [Post mortem](#post_mortem)
    - [Final Words](#final_words)
    
    
### <b>Gameplay Showcase: <a name="gameplay_showcase"></a>
<iframe width="100%" height="450" src="https://www.youtube.com/embed/zEZMtG-oGwY" title="Iconoclasm Gameplay Video" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<div style="text-align: center;">
    <i>Credit: Recorded by Gavin Lim, Product Manager of Pog Studios.</i>
</div>

### <b>Engine Showcase: <a name="engine_showcase"></a>
<iframe width="100%" height="450" src="https://www.youtube.com/embed/XnWB3bPaswY" title="GodKillers - Engine² Showcase" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

## <b>Development: <a name="development"></a>
# <b>Introduction: <a name = "introduction"></a>

This entire endeavor took about three trimesters (12 months) to complete. 
It began as a two-man initiative during the school holidays by me and a close buddy 
in order for us to have a head start and gradually learn the ropes before the semester began.

We gradually grew the team to a total of eight people, including four programmers, two designers, and two artists.

# <b>Features: <a name = "features"></a>

A non-exhausitive list of features available in PogEngine are:
- Audio.
- Prefabs.
- 2D graphics.
- Level editor.
- Particle system.
- Spritesheet animation.
- C++ Scripting with hot reloading.

Check out some of the features offered by PogEngine <a href="https://www.youtube.com/embed/XnWB3bPaswY" target="_blank">here</a>. 

# <b>Tools: <a name = "tools"></a>
Tools that we used during development:
- C++ 
- GitHub for version control.
- Visual Studio choice of IDE for development.
- Discord/Trello for communication and task tracking.

# <b>Libraries: <a name = "libraries"></a>

This project made use of many third party libraries. The entire list of libraries used are:
- [DearImGui](https://github.com/ocornut/imgui): Building blocks for the engine's GUI.
- [FMOD](https://www.fmod.com/): Audio Engine.
- [FreeType](https://freetype.org/): Font rendering.
- [GLI](https://github.com/benikabocha/tinyddsloader): DDS texture loading library.
- [GLFW](https://www.glfw.org/): Creating and managing windows, as well as for creating the OpenGL rendering context.
- [GLM](https://github.com/g-truc/glm): Mathematics library.
- [ImGuizmo](https://github.com/CedricGuillemet/ImGuizmo): Gizmo tooling.
- [RapidJSON](https://rapidjson.org/): Serialization of data into JSON files.
- [stb](https://github.com/nothings/stb): Texture loading library.

# <b>Contributions: <a name="contributions"></a>

At the time, I was quite interested in computer graphics and tools programming. 
As a result, I volunteered to be the graphics programmer and level editor champion.
I also helped with the gameplay programming, concentrating on the game UI and dialogue system.

#### <b> Graphics: <a name="graphics"></a>

At the time, my sole exposure to computer graphics was an introductory module taught in the third trimester of my first year, 
which coincided with the early development stages of this project. 
The lesson also concentrated on foundations such as camera projections, building scale, rotation, and translation matrices, 
and developing a software renderer. 
This was in direct opposition to my goal of creating a high-performance hardware-accelerated graphics system. As a result,
there was a lot of self studying I had to do.

As a result, I started binging on my two main sources of information, that is: 
- [LearnOpenGL](https://learnopengl.com/) website.
- [TheCherno](https://learnopengl.com/) youtube channel.

Both the LearnOpenGL website and TheCherno helped a lot in laying the groundwork for this project such as setting up the OpenGL context, 
setting up and writing shaders, rendering textures. I also learnt some advanced rendering techniques from TheCherno such as batch rendering. 

By the end of the project, some key achievements of the graphics system are:
 - Basic primitives such as triangles, quads, circles.
 - Debug rendering using lines.
 - Batch rendering.
 - Font rendering (with font atlases and batching).
 - Sprite sheet animation.
 - Layering (Background, middleground, foreground, HUD)

#### <b> Editor: <a name="editor"></a>

We relied extensively on Dear ImGUI to construct the editor. Despite my lack of experience in creating a level editor, 
I had an end objective in mind. And that is to reproduce the editing experience in Unity. This turned out to be a far too ambitious aim, 
which I was not even close to achieving by the end of the project. 

However, given that this is my first try at creating an editor, I believe I did a fair job. Surprisingly, after 1.5 years after completion, 
I noticed UI&UX of the editor was a lot better in my recollection than it actually was, which I'll happily attribute this to growth. Furthermore, the 
experience I got from working on this editor was really beneficial while developing the level editor for my third year project, which I am far more proud of.

Here are some photographs and gifs of the engine as it evolved. 
There could be a significant difference between each picture as I did not make a habit of 
documenting the development on a regular basis. I wished I had taken more images to record this journey.

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Editor/1.png" width="100%" height="100%">
        <div class="centered-text">
        <i>Got a window up and running!</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Editor/2.png" width="100%" height="100%">
        <div class="centered-text">
        <i>Very first two texture object in PogEngine.</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Editor/3.png" width="100%" height="100%">
        <div class="centered-text">
        <i>Beginnings of the editor.</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Editor/4.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>Some basic editor features integrated (Scene graph, Content browser, Properties panel).</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Editor/6.png" width="100%" height="100%">
        <div class="centered-text">
        <i>Overhauled the UI of the editor!</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Editor/7.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>Got dragging and droping to create entities working!</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Editor/8.png" width="100%" height="100%">
        <div class="centered-text">
        <i>Prefab inspector.</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Editor/9.png" width="100%" height="100%">
        <div class="centered-text">
        <i>Some of PogEngine's features.</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Editor/10.png" width="100%" height="100%">
        <div class="centered-text">
        <i>PogEngine's editor layout.</i>
    </div>
</div>


#### <b> Proudest feature: 
If I had to pick an editor feature that I am most proud of, it would have to be the
animation viewer.

#### <b> Biggest regret: 
Tilemap editor?

#### <b> Gameplay: <a name="gameplay"></a>

Dialogue system

Journal

UI Animations (Easing functions, lerp, bezier curve, gdc talk)



#### <b> Challenges? 

Markup text formatting.
Lighting?


# <b>Post mortem: <a name = "tools"></a>
