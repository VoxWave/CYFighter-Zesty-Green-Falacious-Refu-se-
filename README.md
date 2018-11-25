# CYFighter-Zesty-Green-Falacious-Refu-se-
CHOOOOOSE YOUR FIGHTEEEEEEEER!!!!!!!!!!!!!!!!

Goals
=====

The condenced goal of the game is to be "The Ultimate Customizable Poverty Anime Fighter". Lets break that up to see what that actually means and how it affects the design goals.

## Ultimate

The game should be the best of its kind. Its what everyone goes to when they want to play a customizable poverty anime fighter. The game should look, sound and feel good to play. It should also be available on a wide range of devices so that people have a less of a chance to miss out on the fun.

## Poverty

The game should be accessible to people of all kinds of monetary situations. That goal is already partially achieved since the engine code is available openly under MIT licence. Even if the game is available for free it still might not be accessible if it only runs on high-end hardware. Therefore the game should be configurable to run on lower-end hardware.

## Customizable
The engine should highly customizable. Users should be able to add new characters, stages and other assets with relative ease.

## Anime Fighter

It's a 2d anime fighting game. This means that to players that have played games such as melty blood, guilty gear, blazblue or under night in-birth the game should have a familiar feel to it.

Game Design
===========

Architecture
============

## ECS

Entity-Component-System(ECS) is a design pattern meant for games and other types of entity based simulations. We chosen to use it because it's well suited for video games and data driven design.    
The game is coded using the Specs Parallel ECS library. Specs was chosen because it's a well maintained and makes parallelisation fairly easy.

## Characters
The characters are the meat of fighting games as they are entities who do the fighting. Because we want the game to be easily customizable, characters should be decoupled from the engine code. This means that we want to treat characters as asset packages.

## Input
