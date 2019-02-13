# Input

For a fighting game and games in general, input handling can be separated in multiple phases. First the are various input devices that are hooked up to the computer that can create input events. The windowing library or some other input library creates enums or structs from these that we can then process.

These "raw" inputs then need to be mapped to the inputs of our game logic. We don't care if a button is pressed unless that button is associated with something that affects the game. For fighting games, the internal buttons for each player are generally the directional inputs and some amount of buttons for attacks and other mechanics.    

In fighting games the directional input usually emulate a traditional joystick. The stick can be pointed in 8 directions or it is in the neutral position. In fighting game notation these directions are called 1(down-left), 2(down), 3(down-right), 4(left), 6(right), 7(up-left), 8(up), 9(up-right) and 5 is the neutral position. This comes from the numpad layout.

The buttons usually have one or two letter names. Often they are just named after the alphabet but sometimes the names refer to the attacks they correspond to. For example in Melty Blood they are just called A, B and C for light, medium and heavy attacks and then D for shield whereas in Guilty Gear the buttons are called P, K, S, HS and D for punch, kick, slash, heavy slash and dust respectively.    


-internal buttons somehow cause character to do moves.

-the parse in to command and then send commands to characters approach

-how it breaks down

-parser combinator approach

-possible difficulties and differences depending on the character implementation.