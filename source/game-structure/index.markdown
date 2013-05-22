---
layout: page
title: "Game Structure"
comments: false
sharing: false
footer: false
---

## Core Classes

In this section you will learn the basic concepts of any typical Cocos2D game which is the game structure and the best way to look at it is thinking that you are producing a Movie with actors, scenes and a director. Is very important to take your time to understand this concepts before jumping right into the code, but if you want to learn it the YOLO way: [start here]({{ root_url }}/sprites).

## Sprites

The term Sprite is commonly used in the game development industry to refer a two dimensional image like the image of a game character, background or menu item. The main purpose of sprites is allowing us to manipulate them independently, so they can be moved, rotated or animated without affecting any other sprite in the same scene.

Any two dimensional video game is composed by multiple sprites, so your game will not be the exception!

## Layers

The layers manage the sprite behaviour, basically they present the sprites on the screen, set their position and also can start the animations. In a more formal way they are responsible for drawing on the screen. Also they can handle the user interaction, like the touches on the screen or the accelerometer. For example: when the user touches the screen, the layer gets the call and tells the hero sprite to start the attack animation.

Layers have a lot of responsibilities so most of your video game code will be placed in subclasses of Layer.

## Scenes

These objects can represent menus, levels, cutscenes or any kind of screen. Their main purpose is to encapsulate functionality (like mini apps) and as stages in the game workflow. They are composed by one or more layers, stacked one behind another.

A single level of your game will be a scene and will contain one of more layers, with each layer containing one or more sprites.

## Director

The Director is responsible for managing all the video game behavior, like presenting one scene or another (also keeping a stack of them), managing the game loop: which is a loop of constant calls to update the drawing on the screen and the game logic and finally pause or stop the game when the device receives a phone call or a text message.

You don't have to worry a lot about the Director, it's almost like automagic!

For more information, see: [Cocos2D Basic Concepts](http://www.cocos2d-iphone.org/wiki/doku.php/prog_guide:basic_concepts)