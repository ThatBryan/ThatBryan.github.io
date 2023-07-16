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
last-updated: 13-07-2023
---

<style>

* {box-sizing: border-box;}
/* body {font-family: Verdana, sans-serif;} */
.mySlides {display: none;}
img {vertical-align: middle;}

/* Slideshow container */
.slideshow-container {
  max-width: 1000px;
  position: relative;
  margin: auto;
}
/* Next & previous buttons */
.prev, .next {
  cursor: pointer;
  position: absolute;
  top: 50%;
  width: auto;
  padding: 16px;
  margin-top: -22px;
  color: white;
  font-weight: bold;
  font-size: 18px;
  transition: 0.6s ease;
  border-radius: 0 3px 3px 0;
  user-select: none;
}

/* Position the "next button" to the right */
.next {
  right: 0;
  border-radius: 3px 0 0 3px;
}
/* On hover, add a black background color with a little bit see-through */
.prev:hover, .next:hover {
  background-color: rgba(0,0,0,0.8);
}

/* Number text (1/3 etc) */
.numbertext {
  color: #f2f2f2;
  font-size: 12px;
  padding: 8px 12px;
  position: absolute;
  top: 0;
}

/* The dots/bullets/indicators */
.dot {
  height: 8px;
  width: 8px;
  margin: 0 2px;
  background-color: #bbb;
  border-radius: 50%;
  display: inline-block;
  transition: background-color 0.6s ease;
}

.active, .dot:hover {
  background-color: #717171;
}

/* On smaller screens, decrease text size */
@media only screen and (max-width: 300px) {
  .text {font-size: 11px}
}
    body {
        color: white; /* Change the text color to red */
        background-image: url("/images/Iconoclasm/bg2.jpg");
        background-attachment: fixed;
        background-position: 50% 100%;
        background-repeat: no-repeat;
        background-size: cover;
        position: relative;
    }

    a{
        color: #5c75f9;
    }
    a:visited {
        color: #5c75f9;

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

## <b>Table of Contents
- [Gameplay Showcase](#gameplay_showcase)
- [Gameplay Development Showcase](#development_showcase)
- [Engine Showcase](#engine_showcase)
- [Development](#development)
    - [Introduction](#introduction)
    - [Features](#features)
    - [Tools](#tools)
    - [Libraries](#libraries)
- [Contributions](#contributions)
    - [Editor](#editor)
    - [Others](#others)
- [Post mortem](#post_mortem)
    - [TiMi Studio: Networking & Demo session](#TiMi)
    - [Ubisoft Singapore Studio Visit](#Ubi)
    - [Final Words](#final_words)
    
## <b>Gallery:
<div class="slideshow-container">
    <div class="mySlides">
        <div class="numbertext">1 / 15</div>
        <img src="/images/Iconoclasm/Gallery/1.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">2 / 15</div>
        <img src="/images/Iconoclasm/Gallery/2.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">3 / 15</div>
        <img src="/images/Iconoclasm/Gallery/3.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">4 / 15</div>
        <img src="/images/Iconoclasm/Gallery/4.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">5 / 15</div>
        <img src="/images/Iconoclasm/Gallery/5.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">6 / 15</div>
        <img src="/images/Iconoclasm/Gallery/6.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">7 / 15</div>
        <img src="/images/Iconoclasm/Gallery/7.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">8 / 15</div>
        <img src="/images/Iconoclasm/Gallery/8.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">9 / 15</div>
        <img src="/images/Iconoclasm/Gallery/9.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">10 / 15</div>
        <img src="/images/Iconoclasm/Gallery/10.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">11 / 15</div>
        <img src="/images/Iconoclasm/Gallery/11.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">12 / 15</div>
        <img src="/images/Iconoclasm/Gallery/12.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">13 / 15</div>
        <img src="/images/Iconoclasm/Gallery/13.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">14 / 15</div>
        <img src="/images/Iconoclasm/Gallery/14.png" style="width:100%">
    </div>
    <div class="mySlides">
        <div class="numbertext">15 / 15</div>
        <img src="/images/Iconoclasm/Gallery/15.png" style="width:100%">
    </div>
    <a class="prev" onclick="plusSlides(-1)">❮</a>
    <a class="next" onclick="plusSlides(1)">❯</a>
</div>

<div style="text-align:center">
  <span class="dot" onclick="currentSlide(1)"></span> 
  <span class="dot" onclick="currentSlide(2)"></span> 
  <span class="dot" onclick="currentSlide(3)"></span>
  <span class="dot" onclick="currentSlide(4)"></span> 
  <span class="dot" onclick="currentSlide(5)"></span> 
  <span class="dot" onclick="currentSlide(6)"></span> 
  <span class="dot" onclick="currentSlide(7)"></span> 
  <span class="dot" onclick="currentSlide(8)"></span> 
  <span class="dot" onclick="currentSlide(9)"></span> 
  <span class="dot" onclick="currentSlide(10)"></span> 
  <span class="dot" onclick="currentSlide(11)"></span> 
  <span class="dot" onclick="currentSlide(12)"></span> 
  <span class="dot" onclick="currentSlide(13)"></span>  
  <span class="dot" onclick="currentSlide(14)"></span>  
  <span class="dot" onclick="currentSlide(15)"></span>  
</div>

## <b>Gameplay Showcase: <a name="gameplay_showcase"></a>
<iframe width="100%" height="450" src="https://www.youtube.com/embed/BCFzNFtZF_E" title="Iconoclasm Gameplay Video" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<div style="text-align: center;">
    <i>Credit: Gavin Lim, Product Manager of Team GodKillers.</i>
</div>

## <b>Gameplay Development Showcase: <a name="development_showcase"></a>
<iframe width="100%" height="450" src="https://www.youtube.com/embed/r3cLJztAMaQ" title="Iconoclasm - Development Showcase" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<div style="text-align: center;">
    <i>Credit: Joel Hoon, Design Lead of Team GodKillers.</i>
</div>

## <b>Engine Showcase: <a name="engine_showcase"></a>
<iframe width="100%" height="450" src="https://www.youtube.com/embed/90ZM4lTItI8" title="GodKillers - Engine² Showcase" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>


## <b>Development: <a name="development"></a>
### <b>Introduction: <a name = "introduction"></a>

The creation of this entire project took two trimesters (~8 months). As a student of the Computer Science track, my focus was on building the custom engine (Engine²) 
that would support the application. The tight deadlines and milestone set by the school, pushed me to design and build the finest solutions I could in the 
least amount of time. In retrospect, there is much that could have been done to improve the engine, particularly with more foresight given that this was only 
my second attempt at building an engine.

### <b>Features: <a name = "features"></a>
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

### <b>Tools: <a name = "tools"></a>
Tools that we used during development:
- C++ 
- GitHub for version control.
- Visual Studio choice of IDE for development.
- Discord/Trello for communication and task tracking.

### <b>Libraries: <a name = "libraries"></a>

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

## <b>Contributions: <a name="contributions"></a>

### <b>Editor: <a name="editor"></a>

<i>Note: Maybe add more ss and some writeup on development process, challenges, 
success/regrets, etc. </i><br>

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

The designers were also kind enough to present me with mockups for some of the features they desired 
and how they should function. I tried my hardest to replicate the mockups and am pleased with the results.

<div style="display: flex;">
    <img src="/images/Iconoclasm/Editor/animation_mockup.jpg" width="50%" height="auto%">
    <img src="/images/Iconoclasm/Editor/animation_viewer.jpg" width="50%" height="auto%">
</div>

<div style="text-align: center;">
    <i>(Left) Feature design document, (Right) Implementation.</i>
</div>

# <b>Some pictures and gifs of the Engine² editor:

<div class = "no-padding-bottom;">
    <img src="/images/Iconoclasm/engine.png" width="100%" height="100%">
    <div style="text-align: center;">
        <i> Level 1 of Iconoclasm inside the Engine² Editor.</i>
    </div>
</div>

<div class = "no-padding-bottom;">
    <img src="/images/Iconoclasm/Editor/editor.gif" width="100%" height="100%">
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
    <img src="/images/Iconoclasm/Editor/properties.gif" width="100%" height="100%">
    <div style="text-align: center;">
        <i> Property inspector.</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Iconoclasm/Editor/filtering.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>Entity filtering.</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Iconoclasm/Editor/copy_paste.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>Copy paste values.</i>
    </div>
</div>

### <b>Others: <a name="others"></a>

Aside from the editor, I also helped out with some tools development, engine features and the usual debugging and optimization.

# <b> Asset Packer:

This feature was inspired by a [video](https://www.youtube.com/watch?v=VjlKwQoKluI) I saw on YouTube. An asset packer compiles all of the game's assets (such as models, textures, audio, animation, level data, and so on) into a single file. This provides a plethora of advantages, such as compressing files to an efficient engine-specific format and protecting one's intellectual property.

Because the asset pack was designed to be used primarily when releasing games, I chose to make it binary. This allows for a more computer-friendly reading of the file during deserialization. I did some load time tests and was pleasantly surprised to see that using the asset pack accelerated our loading time up to three folds.

Despite the successes, there were parts of the asset packer I did not manage to attempt. These are compression and obfuscation. As a result, the Iconoclasm asset pack size came in at just under 1.4GB. While I considered working on obfuscation by incorporating some simple encryption, such as the Caesar cipher, I ultimately decided against it in favor of doing less work during runtime for a smoother experience. If I ever have to work on another asset packer, these are two main areas I'd like to focus on. 

# <b> Root motion:

This was a feature that the designers requested be supported by the engine's skeletal animation. You may refer to unreal engine's documentation on root motion [here](https://docs.unrealengine.com/4.27/en-US/AnimatingObjects/SkeletalMeshAnimation/RootMotion/) to learn more.

<div class = "no-padding-bottom">
    <img src="/images/Iconoclasm/Others/root_motion.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>Side by side comparison (Model further back does not have root motion on).</i>
    </div>
</div>


# <b> Dirty flag optimization:

I also worked on optimization using the dirty flag pattern described in a famous book titled "Game Programming Patterns". The impetus for this optimization came from a profiling session that indicated a significant bottleneck in the way we first handled our scene graph. This optimization strategy increased our frame rate from roughly 27 to 66 frames per second. More information on this optimization technique can be found [here](https://gameprogrammingpatterns.com/dirty-flag.html).


<div class="no-padding-bottom" style="display: flex; justify-content: center;">
    <img src="/images/Iconoclasm/game-programming-patterns.jpg" width="40%" height="40%">
</div>

<div class="centered-text">
    <i>The book that disscusses the dirty flag optimization pattern.</i>
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

### <b>TiMi Studio: Networking & Demo session:  <a name = "TiMi"></a>

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

### <b>Ubisoft Singapore Studio Visit: <a name = "Ubi"></a>

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

## <b>Final words: <a name="final_words"></a>

This was my first time working on a project that received such excellent reviews and considering that 
this was the final major project module at DigiPen, I couldn't have asked for a better finish. 
Perhaps it was the satisfaction of knowing I had a hand in the accomplishment that prompted me to consider 
a career in the games industry, something I had never considered before.

Moving foward, I'll be starting an internship as a Gameplay Programmer at Ubisoft Singapore in August 2023, 
and I'm still in disbelief that I've been accepted into South East Asia's largest AAA studio. 
I'm looking forward to having a good time and learning a lot while I'm there.

<script src = "/scripts/projects.js"></script>