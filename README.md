# Flappy_Whale
Survival game depicting lives of sperm whales through the age of whaling.

Objective: Exploring the life of sperm whales living across a span of history including the whaling age, during which sperm whales were nearly hunted to extinction. The goal of the player is to survive this tumultuous age by hunting squid and avoiding whalers, so that they can manage various resources required for survival (breath, hunger, depth, etc.). Gameplay is essentially a survival roguelike, imagined via a side-scrolling perspective.
 
Possible Controls:
Control Scheme 1 (Keyboard)
W,S: Adjust angle of travel (controls the direction the head is facing)
A, D: Stop and move “forward” (in direction of orientation)
E: Context sensitive action (Bite, Tip, Initiate mating, etc.)
Space Bar: Echolocation click
 
Control Scheme 2 (Mouse + Keyboard*)
The direction of the mouse pointer determines angle of travel
Left Click: initiates a flap
Right Click: Echolocation click
 
Core resources:
Breath: Sperm whales cannot breathe underwater so they are required to surface in order to fill their lungs with air. An onscreen meter would show the player how much air they have left and reddened/blackened edges of the screen would indicate to the player when they were running dangerously low on air. Upon surfacing the whale automatically begins breathing, and an onscreen overlay of the breath meter will indicate how much air is being taken in. A period of several seconds will be required to take a full breath as sperm whales will often spend minutes at the surface in order to breath before diving again.
 
Hunger: Like all animals sperm whales must eat to survive. An onscreen meter would show the player the state of the whale’s hunger (view of the stomach with undigested squid beaks inside?). Satiating hunger prompts the player into pursuing one of the core gameplay loops, hunting. Without eating, the whale becomes more sickly overtime, causing Health to drop, until the whale eventually dies. Eating will prevent this process and can refill a small amount of lost Health, depending on what is eaten, with larger and more difficult prey garnering greater rewards (i.e. Giant Squid)
 
Depth: Sperm whales can are amongst some of the deepest diving animals on earth, but even they have their limits. As the player ventures further and further into the depths of the ocean the immense pressure of the water takes its effect on the whale. Venture too deep and the sperm whale will be crushed by the pressure. Depth will be indicated via an onscreen meter, the darkening of the surrounding water, as well as a helpful warning should the player begin to descend too far.
 
Health: Indicated through an HP bar or some other visual meter, health is required to survive, with hunger/food especially feeding into the management of this resource. Health mustn’t drop to zero in order for the player to survive, and eating prevents the loss of Health and refills Health slowly over time. Being damaged by whalers can cause serious wounds (represented by a covered overlay) preventing health from being recovered quickly after encounters with whaling ships. This ensures that ships are dangerous, especially as the number of whalers increases later in the game, as while one encounter might not kill the player, multiple encounters in succession very much could.
 
Core Gameplay Loops:
Hunting: In order to satiate hunger sperm whales must hunt. Most squid will exist deep below the surface waters, so the player must dive deep in order to access them. This presents a number of challenges to the player, as they must manage their breath and depth, as well as contend with increasing darkness as they descend ever deeper in pursuit of prey. By using echolocation the player can extend their range of perception, allowing them to track prey without light. The player emits an echolocating click by pressing the spacebar which will reveal the area in front of them at the point in time they had made the click. This might illuminate the area ahead of the player for an instant before fading away slowly over a brief period of time. 
Not only for navigation, echolocation is also used for slowing and stunning prey. Each click that is directed towards prey will momentarily slow it allowing the player to close distance and land more clicks. The intensity of the slowing effect scales with distance, allowing a player that is close enough to prey to essentially stun it, locking it in place as they go in for the kill.
On a technical level, pressing space bar initiates a sonar click. This creates a projectile (or series of projectiles) that travels out from the player’s whale based on the angle of orientation. Once the projectile makes contact with something it illuminates that object, and returns to the player. The player would be prevented from initiating another click while the sonar click is in travel, so that the click can’t be “spammed” unless the player has succeeded in getting close to their prey.
 
Avoiding Whalers: Whalers are the principle threat to the survival of the player. As the age of whaling begins Whalers will have a chance to spawn as the player surfaces, and as the age progresses will become more numerous and approach from more devious angles. Whaling ships will produce rowboats which will then row out and approach the player, shooting harpoons as they get close. Harpoons reduce the Health of the player and can cause lasting Health effects that persist long after the player has escaped from the Whalers. These harpoons could embed themselves into the player as a visual indicator for when and why their Health is reduced.
 
Required Core Assets:
HUD
Health meter
Breath meter
Hunger display
Depth indicator
Whale:
Swimming
Diving
Surfacing
Breaching (blowhole breath)
Bite
Whalers:
Ship (generates rowboat)
Rowboat
Shoots harpoons
Squid:
Swimming
 
Non Core Gameplay:
Whale on Whale romance: Mating with another whale would secure the player an extra life should. The actual process of mating could play out like a rhythm game, similar to guitar hero, where the player must match a series of clicks produced by the other whale in order to proceed to getting it on. Whales might have an inherent set of traits (i.e. +/- to breath capacity, +/- hunger Health degen rate, etc.) that could be passed down through their offspring.
 
Progression elements: Whale grows larger over the course of the game, allowing the player to dive deeper and hunt more difficult prey, while also increasing their hunger degen rate. This would allow the player to hunt Giant Squid, and might also grant the ability to tip the Whaler’s row boats.
