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
description: 2.5D point-n-click narrative adventure game.
last-updated: 11-07-2023
download-link: https://drive.google.com/file/d/1yRHwQmvV3t3Yh7wBqhJjfE11Gl0Ddns1/view?usp=sharing
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
        color: #006fff;
    }
    a:visited {
        color: #006fff;  
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

## <b>Table of Contents
- [Gameplay Showcase](#gameplay_showcase)
- [Engine Showcase](#engine_showcase)
- [Development](#development)
    - [Introduction](#introduction)
    - [Features](#features)
    - [Tools](#tools)
    - [Libraries](#libraries)
- [Contributions](#contributions)
    - [Graphics](#graphics)
    - [Editor](#editor)
    - [Gameplay](#gameplay)
        - [Dialogue System](#graphics)
        - [User Interface](#ui)
        - [In-game Cheats](#cheats)
    - [Challenges](#challenges)
- [Post mortem](#post_mortem)
    - [Final Words](#final_words)
    
    
## <b>Gameplay Showcase: <a name="gameplay_showcase"></a>
<iframe width="100%" height="450" src="https://www.youtube.com/embed/zEZMtG-oGwY" title="Iconoclasm Gameplay Video" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>
<div style="text-align: center;">
    <i>Credit: Recorded by Gavin Lim, Product Manager of Pog Studios.</i>
</div>

## <b>Engine Showcase: <a name="engine_showcase"></a>
<iframe width="100%" height="450" src="https://www.youtube.com/embed/XnWB3bPaswY" title="GodKillers - Engine² Showcase" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

<br>

## <b>Development: <a name="development"></a>
### <b>Introduction: <a name = "introduction"></a>

This entire endeavor took about three trimesters (12 months) to complete. 
It began as a two-man initiative during the school holidays by me and a close buddy 
in order for us to have a head start and gradually learn the ropes before the semester began.

We gradually grew the team to a total of eight people, including four programmers, two designers, and two artists.

### <b>Features: <a name = "features"></a>

A non-exhausitive list of features available in PogEngine are:
- Audio.
- Prefabs.
- 2D graphics.
- Level editor.
- Particle system.
- Spritesheet animation.
- C++ Scripting with hot reloading.

Check out some of the features offered by PogEngine <a href="https://www.youtube.com/embed/XnWB3bPaswY" target="_blank">here</a>. 

### <b>Tools: <a name = "tools"></a>
Tools that we used during development:
- C++ 
- GitHub for version control.
- Visual Studio choice of IDE for development.
- Discord/Trello for communication and task tracking.

### <b>Libraries: <a name = "libraries"></a>

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

## <b>Contributions: <a name="contributions"></a>

At the time, I was quite interested in computer graphics and tools programming. 
As a result, I volunteered to be the graphics programmer and level editor champion.
I also helped with the gameplay programming, concentrating on the Parcel's UI and dialogue system.

### <b> Graphics: <a name="graphics"></a>

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

### <b> Editor: <a name="editor"></a>

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
animation inspector.

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Editor/animation_viewer.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>Example of using the animation inspector.</i>
    </div>
</div>

<br>
The inspiration for this feature actually came from an online source that I unfortunately do not
remember. I thought it was clue and decided to challenge myself to replicate it.
I am very happy with how it turned out.

#### <b> Biggest regret: 
My greatest regret has to be the tilemap system. It is, ironically, a feature that I am proud of. 
The regret originates from the mistaken idea that such a feature was required, which resulted in many hours spent. 
This feature was eventually removed because it was never used. It taught me a hard lesson about not jumping the gun 
and working on things that aren't necessary. Nonetheless, it still made for an excellent tools development exercise.

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Editor/tilemap_editor.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>Tilemap editor before it was removed.</i>
    </div>
</div>


### <b> Gameplay: <a name="gameplay"></a>

In the later phases of Parcels' development, my focus moved to assisting with gameplay development. 
<br><br>My role was largely focused on implementation, leveraging art assets created by PogStudio's artists and designs mockups drafted by our designers.

# <b> Dialogue system: <a name = "dialogue"></a>

One of the gameplay components I worked on was Parcel's dialogue system. It allows designers to control which dialogue <i>(stored in JSON files, see image below)</i> to run, what sprites to use, and many more parameters that are accessible via an interface from the scripting engine.

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Gameplay/dialogueJSON.jpg" width="100%" height="100%">
        <div class="centered-text">
        <i>Parcel's dialogue JSON format.</i>
    </div>
</div>

<br>

It took me many iterations with both the artists and designers to obtain a product that everyone was statisfied with. Here are some of the early iterations of the dialogue system which features various animations/designs:

#### <b> First iteration:
First iteration of Parcel's dialogue design. It was scrapped in favor of a different design.
<div class = "no-padding-bottom">
    <img src="/images/Parcels/Gameplay/dialogue_old.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>First iteration of Parcel's dialogue design. </i>
    </div>
</div>

#### <b> Second iteration:
Second iteration of Parcel's dialogue design. The designers and artists also decided that the game should have some of transition animation that indicates the start of a dialogue. We decided to keep the design, but continue working on the transition animation as the current linear interpolation approach looked boring. 

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Gameplay/lerp.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>Updated layout with transition in animation.</i>
    </div>
</div>

#### <b> Third iteration:
For this iteration, the team decided that we also wanted a transition out animation to indicate the end of a dialogue. For animation, I used a second degree polynomial ease out function this time, but our lead artist had a better idea.

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Gameplay/ease_out.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>Transition in and out using second degree polynomial.</i>
    </div>
</div>

<br>
Our lead artist decided the transition would look best with some <i>"anticipation"</i> to it. To achieve such a effect, I made use of a cubic bezier curve equation. It took some extra back and forth before the lead artist and I were able to fine-tune the control points of the bezier curve in order to achieve a satisfactory result.

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Gameplay/convo.jpg" width="100%" height="100%">
        <div class="centered-text">
        <i>Back and forth between me and our lead artist.</i>
    </div>
</div>

#### <b> Final:
The final look of Parcel's dialogue system:

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Gameplay/dialogue.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>Final iteration.</i>
    </div>
</div>

# <b> User Interface: <a name = "ui"></a>

I also worked on a handful of Parcel's UI such as:

#### <b> Main menu & transitions:
<div class = "no-padding-bottom">
    <img src="/images/Parcels/Gameplay/menu.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>A Parcel's main menu.</i>
    </div>
</div>

#### <b>Heads up display & pause menu:
<div class = "no-padding-bottom">
    <img src="/images/Parcels/Gameplay/hud.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>Parcel's HUD and pause menu.</i>
    </div>
</div>

# <b>Ingame cheats: <a name = "cheats"></a>
In the middle of development, the team noted that it was a bit tedious having to run
through early sections of the game in order to get to a further point that we are looking to test. To combat this, I developed a cheat system that allows real-time tweaking of variables which dictates the flow of the game, as well as skipping to key developments of the game.

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Gameplay/cheats.gif" width="100%" height="100%">
        <div class="centered-text">
        <i>Parcel's cheat menu.</i>
    </div>
</div>

### <b> Challenges: <a name="challenges"></a>

Because the game placed a strong emphasis on reading, one suggestion the team got from the faculty was to use font changes such as bolding and italics to enrich the experience. This was when the designer mentioned the wish for markup text formatting, i.e writing: "This is b>some text/b>" and rendering "This is" as standard text while bolding "some text."

My first thought was to somehow utilize linear algebra to manipulate the quads that the text were rendered on to achieve such effects. However, I didn't manage to get very far with this method and decided to go ahead with something more naive.

My naive solution was to make use of font familys that already had their own italics and bold fonts in truetype files. During rendering, I would go through the entire string of text and identify the presence of tags to switch between the regulat/bold/italic fonts.

Of course, the use of this naive solution meant that the team's choice of fonts were limited to fonts whom provided the entire variations of font family we were looking for. This was a difficult challenge that I regret not being able to fully complete.

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Gameplay/raw_text.jpg" width="100%" height="100%">
        <div class="centered-text">
        <i>Raw text.</i>
    </div>
</div>

<div class = "no-padding-bottom">
    <img src="/images/Parcels/Gameplay/bold_text.jpg" width="100%" height="100%">
        <div class="centered-text">
        <i>Rendered outcome ingame.</i>
    </div>
</div>


### <b>Post mortem: <a name = "Post mortem"></a>

This was a project of many firsts. First time working with artists and designers, first time working on a large scale project in terms of head count and duration, first time building a custom engine from scratch, first time building a graphics and editor system. 

Looking back, I had a lot of regrets and things I could have done better, from architecture to editing features/tools and even time management. I heard a statement that goes something like this: "You should always cringe when you look back at your previous work." If you didn't, you most likely stagnated and did not improve in the previous year." This sentiment seems to be resonating with me right now, 1.5 years after development.

I took the lessons I learned and the features I hoped I could have incorporated in this project and applied them to my third year project that I am very proud of. More information regarding my third-year project can be found [here](../iconoclasm).