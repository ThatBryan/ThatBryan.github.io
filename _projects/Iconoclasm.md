---
layout: project
name: "Iconoclasm"
title: "Iconoclasm: Fall of The False God"
permalink: "projects/iconoclasm/"
game-engine: "Engine²"
start-date: 2022-09-01
end-date: 2023-03-01
school-project: True
school: DigiPen Institute of Technology Singapore
module: Software Engineering Project 5-6
description: A 3D hack-n-slash action game.
last-updated: 02-07-2023
---

<style>
    body {
        color: white; /* Change the text color to red */
        background-image: url("/images/Iconoclasm/bg2.jpg");
        background-attachment: fixed;
        background-position: 50% 100%;
        background-repeat: no-repeat;
        background-size: cover;
        position: relative;
    }
</style>

<img src="/images/Iconoclasm/iconoclasm-logo.jpeg" width="100%" height="100%">

Iconoclasm is a 3D hack-n-slash action game powered by Engine², a custom C++ engine.
It was developed for the Software Engineering Project 5 and Software Engineering Project 6 modules at the DigiPen Institute of Technology Singapore
by Team GodKillers, a 10 men group.

<img src="/images/Iconoclasm/team_logo.png" width="100%" height="100%">
<div style="text-align: center;">
    <i>Team GodKillers logo.</i>
</div>

# <b>Table of Contents
- [Gameplay Showcase](#gameplay_showcase)
- [Gameplay Development Showcase](#development_showcase)
- [Engine Showcase](#engine_showcase)
- [Development](#development)
    - [Introduction](#introduction)
    - [Features](#features)
    - [Tools](#tools)
    - [Libraries](#libraries)
    - [Contribution](#contributions)
- [Post mortem](#post_mortem)
    - [TiMi Studio: Networking & Demo session](#TiMi)
    - [Ubisoft Singapore Studio Visit](#Ubi)
    - [Final Words](#final_words)
    

### <b>Gameplay Showcase: <a name="gameplay_showcase"></a>
<iframe width="100%" height="450" src="https://www.youtube.com/embed/BCFzNFtZF_E" title="Iconoclasm Gameplay Video" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<div style="text-align: center;">
    <i>Credit: Gavin Lim, Product Manager of Team GodKillers.</i>
</div>

### <b>Gameplay Development Showcase: <a name="development_showcase"></a>
<iframe width="100%" height="450" src="https://www.youtube.com/embed/r3cLJztAMaQ" title="Iconoclasm - Development Showcase" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<div style="text-align: center;">
    <i>Credit: Joel Hoon, Design Lead of Team GodKillers.</i>
</div>

### <b>Engine Showcase: <a name="engine_showcase"></a>
<iframe width="100%" height="450" src="https://www.youtube.com/embed/90ZM4lTItI8" title="GodKillers - Engine² Showcase" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## <b>Development: <a name="development"></a>
# <b>Introduction: <a name = "introduction"></a>

The creation of this entire project took two trimesters (~8 months). As a student of the Computer Science track, my focus was on building the custom engine (Engine²) 
that would support the application. The tight deadlines and milestone set by the school, pushed me to design and build the finest solutions I could in the 
least amount of time. In retrospect, there is much that could have been done to improve the engine, particularly with more foresight given that this was only 
my second attempt at building an engine.

# <b>Features: <a name = "features"></a>
As our designers worked on the prototype in Unity, they provided the features that they used with us so that we know what tools they needed to produce this game. 

A non-exhausitive list of features available in Engine² are:
- 3D graphics with lighting and shadow.
- 3D spatial audio.
- Level editor.
- Physics simulation.
- Skeletal Animation with blending.
- C# Scripting with hot reloading.
- Particle system.
- Post processing.
- Prefabs.

Check out some of the features offered by Engine² <a href="https://www.youtube.com/embed/90ZM4lTItI8" target="_blank">here</a>. 

# <b>Tools: <a name = "tools"></a>
Tools that we used during development:
- C++ 
- GitHub for version control.
- Visual Studio choice of IDE for development.
- Discord/Trello for communication and task tracking.

# <b>Libraries: <a name = "libraries"></a>

This project made use of many third party libraries. The entire list of libraries used are:
- [Assimp](https://github.com/assimp/assimp) : Model importing.
- [DearImGui](https://github.com/ocornut/imgui): Building blocks for the engine's GUI.
- [EnTT](https://github.com/skypjack/entt): Entity Component System (ECS), for managing game entities and components.
- [FMOD](https://www.fmod.com/): Audio Engine.
- [FreeType](https://freetype.org/): Font rendering.
- [GLFW](https://www.glfw.org/): Creating and managing windows, as well as for creating the OpenGL rendering context.
- [GLM](https://github.com/g-truc/glm): Mathematics library.
- [ImGuizmo](https://github.com/CedricGuillemet/ImGuizmo): Gizmo tooling.
- [Mono](https://www.mono-project.com/): C# .NET Framework for gameplay scripting.
- [PhysX](https://developer.nvidia.com/physx-sdk): Physics engine.
- [RapidJSON](https://rapidjson.org/): Serialization of data into JSON files.
- [Spdlog](https://github.com/gabime/spdlog): Logging library.
- [stb](https://github.com/nothings/stb): Texture loading library.
- [TinyDDSLoader](https://github.com/benikabocha/tinyddsloader): DDS texture loading library.

# <b>Contributions: <a name="contributions"></a>

Because the designers came from a Unity background, I tried my hardest as the 
primary editor programmer to reproduce the experience of using Unity's editor. 
Some of the editor features which I have worked on are:

<ul>
  <li>Editor & game viewport.</li>
  <li>Scene Graph.</li>
  <li>Content browser panel.</li>
  <li>Searching/filtering.</li>
  <li>Entity property inspector.</li>
  <li>Adding/removing entities.</li>
  <li>Adding/removing components.</li>
  <li>Undo/redo changes.</li>
  <li>Copy/pasting values.</li>
  <li>Gizmo tools.</li>
  <li>Importing assets.</li>
  <li>Asset import settings.</li>
</ul>

Other contributions:
<ul>
  <li>Asset packer.</li>
  <li>Player preference (player data).</li>
  <li>Root motion for skeletal animation.</li>
  <li>Dirty flag optimization.</li>
  <li>Lots of debugging.</li>
</ul>

The designers were also kind enough to present me with mockups for some of the features they desired 
and how they should function. I tried my hardest to replicate the mockups and am pleased with the results.

<div class = "no-padding-bottom;">
    <img src="/images/Iconoclasm/animation_mockup.jpg" width="100%" height="100%">
    <div style="text-align: center;">
        <i> Animation component feature mockup by designers.</i>
    </div>
</div>

<div class = "no-padding-bottom;">
    <img src="/images/Iconoclasm/animation_feature.jpg" width="100%" height="100%">
    <div style="text-align: center;">
        <i> Result.</i>
    </div>
</div>
<br>

# <b>Some pictures and gifs of the Engine² editor:

<div class = "no-padding-bottom;">
    <img src="/images/Iconoclasm/engine.png" width="100%" height="100%">
    <div style="text-align: center;">
        <i> Level 1 of Iconoclasm inside the Engine² Editor.</i>
    </div>
</div>

<div class = "no-padding-bottom;">
    <img src="/images/Iconoclasm/b.gif" width="100%" height="100%">
    <div style="text-align: center;">
        <i> Running & testing the game from the editor.</i>
    </div>
</div>

<div class = "no-padding-bottom;">
    <img src="/images/Iconoclasm/adding_entities.gif" width="100%" height="100%">
    <div style="text-align: center;">
        <i> Instantiating prefabs.</i>
    </div>
</div>

<div class = "no-padding-bottom;">
    <img src="/images/Iconoclasm/content_browser.gif" width="100%" height="100%">
    <div style="text-align: center;">
        <i> Importing assets.</i>
    </div>
</div>

<div class = "no-padding-bottom;">
    <img src="/images/Iconoclasm/properties.gif" width="100%" height="100%">
    <div style="text-align: center;">
        <i> Property inspector.</i>
    </div>
</div>

## <b>Post mortem: <a name="post_mortem"></a>

It was a long journey, starting from inception all the way to completion. It started with the
designers pitching to us their vision for the game and they proved that they had what it takes
to see their idea through with a prototype. Since then the pressure was on the programmers, we knew 
we had to go above and beyond the scope of what was required from us and really push our skills to the limit. 
Overall, I am very proud of what our team has achieved collectively. 

During the final milestone of this project, the school invited guests from the industry 
to watch our presentation. And thankfully, it seemed like our hardwork had not gone unnoticed
as our team had the pleasure of being invited to two private networking sessions. 

#### <b>TiMi Studio: Networking & Demo session:  <a name = "TiMi"></a>

During the semester break, we were contacted by the school's career services and invited to a networking and 
demo session with TiMi Studio's Technical Director, Principal Audio Designer and other representatives!

<div class = "no-padding-bottom">
    <img src="/images/Iconoclasm/timi1.jpg" width="100%" height="100%">
</div>

<div class = "no-padding-bottom">
    <img src="/images/Iconoclasm/timi2.jpg" width="100%" height="100%">
    <div style="text-align: center;">
        <i>TiMi studio trying Iconoclasm!</i>
    </div>
</div>

#### <b>Ubisoft Singapore Studio Visit: <a name = "Ubi"></a>

We also had the pleasure of being invited by Ubisoft Singapore for a studio visit! We had the chance to 
showcase our projects to the Ubisoft team, receive feedback from professionals, and speak to some of their developers. 

<div class = "no-padding-bottom">
    <img src="/images/Iconoclasm/ubi1.jpg" width="100%" height="100%">
    <div style="text-align: center;">
        <i>Team GodKillers minus Ching Yin.</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Iconoclasm/ubi2.jpg" width="100%" height="100%">
    <div style="text-align: center;">
        <i>Team GodKillers minus Ching Yin.</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Iconoclasm/ubi3.jpg" width="100%" height="100%">
        <div style="text-align: center;">
        <i>Presenting our project.</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Iconoclasm/ubi4.jpg" width="100%" height="100%">
        <div class="centered-text">
        <i>Setting up playtest session.</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Iconoclasm/ubi5.jpg" width="100%" height="100%">
        <div class="centered-text">
        <i>Getting feedback from Ubisoft developers.</i>
    </div>
</div>

# <b>Final words: <a name="final_words"></a>

This was my first time working on a project that received such excellent reviews and considering that 
this was the final major project module at DigiPen, I couldn't have asked for a better finish. 
Perhaps it was the satisfaction of knowing I had a hand in the accomplishment that prompted me to consider 
a career in the games industry, something I had never considered before.

Moving foward, I'll be starting an internship as a Gameplay Programmer at Ubisoft Singapore in August 2023, 
and I'm still in disbelief that I've been accepted into South East Asia's largest AAA studio. 
I'm looking forward to having a good time and learning a lot while I'm there.
