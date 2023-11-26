# ChamberCrawlingRPG
Engineered a RogueLike 2-player RPG game with a team of developers using objected oriented principles in C++

Due to university policy, the source code for this project is omitted, however below several screenshots illustrate the functionality of the game; I would be happy to provide the source code upon request.

The UML for the project is displayed below, the game implements the Incorporated Observer, Factory method, Decorator, and Model View Controller design patterns. Techniques such as Polymorphism, RAII and single responsibility principle are incorporated into the design as well. 
![UML Diagram](https://github.com/ypruthi/ChamberCrawlingRPG/assets/110852301/0ecc6d3f-aeb5-4530-a80e-abda272bef9a)

Upon the game's launch, a CLI prompts the player to pass a level file, or a random level is generated for them. Then, a player can select one of five races. 

<img width="637" alt="Screenshot 2023-11-25 at 6 49 32 PM" src="https://github.com/ypruthi/ChamberCrawlingRPG/assets/110852301/8ac8cfd1-20b1-431f-9159-33380cfcd042">

Players can execute a turn by moving in all eight ordinal directions by passing commands accordingly. (N,E,...NW) Alternatively, they can also attack a nearby enemy/utilize a potion, and specify a direction. In both cases, NPCs on the map will execute their turn after the player, which has been implemented with the Observer pattern. 

The screenshot below shows the command "a ea" [attack east] in action, along with the NPC's response. Over eight NPC enemies are implemented in the game, each with specific movement and attack pattern specifications. 

<img width="578" alt="Screenshot 2023-11-25 at 6 53 20 PM" src="https://github.com/ypruthi/ChamberCrawlingRPG/assets/110852301/07717385-5f29-4725-b08a-c2d8b5ce0025">

The screenshot below shows command "u nw" [use northwest] to use a potion. Potions are spawned during runtime by leveraging the strategy pattern. 

Player sees the potion:
<img width="576" alt="Screenshot 2023-11-25 at 6 55 44 PM" src="https://github.com/ypruthi/ChamberCrawlingRPG/assets/110852301/0340796d-ad2c-4da3-85ec-99fefd46f35b">

Player utilizes the potion: 
<img width="558" alt="Screenshot 2023-11-25 at 6 56 22 PM" src="https://github.com/ypruthi/ChamberCrawlingRPG/assets/110852301/e65e6abc-1f9f-4110-b633-03c31e97f63e">

Finally, a freeze command (to halt all enemies and their actions), a restart command, and a teleport command are implemented in the game as well.

