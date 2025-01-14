[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-22041afd0340ce965d47ae6ef1cefeee28c7c493a6346c4f15d667ab976d596c.svg)](https://classroom.github.com/a/MjLLqDcN)
# HW1
## W1L2 In-Class Activity

Homework 1 Activity

I would describe the game world in objects as:
- UI
    - Seeds planted UI
    - Seeds remaining UI
- Player
    - Movement
- Plants
    - Placed by player

The attributes and actions these objects have are providing information about the game towards the player. In other words, the UI in regards to seeds planted/remaining informs the player whether they have planted a seed or not, as well as how many seeds they have left. The player object allows the individual player to precisely move towards a specific location of where they would like to plant a seed. Lastly, when a seed is planted and a flower is displayed, it represents that the player was successful in planting a seed.

These objects act on or affect each other by having the player move around and plant seeds until the “Seeds Remaining” UI says that there are zero seeds left. Each seed that is planted places a flower indicating the player has successfully planted a seed and reveals how many seeds are planted until the UI aspect shows that the player has reached the maximum number of planted seeds (5). When the "Seeds Planted" UI displays five, the player can no longer plant further. In summary, these objects act on and affect each other in a cause and effect manner. 


## Devlog

In regards to planning for UI, I wanted to maintain a simple yet straightforward way to display the planted and remaining seeds. I applied this to the PlantCountUI class, which directly uses the UpdateSeeds method to update the Seeds Planted and Seeds Remaining text GameObjects in the scene. The (_plantedText and _remainingText) in the script are explicitly revealed as serialized fields. As a result, the UpdateSeeds method properly displays the Seeds Planted and Seeds Remaining on the top left of the screen in white font and correctly update based on how the player plays the game. The coding process aligned with my break-down since I aimed for a simplisitic way to display seed usage for the player.

Additionally, for the Player object I considered the movement to remain simple like how Professor Reid did. In other words, to just have the player model be able to move anywhere and plant a seed anywhere the player decides to. The Player script includes the Update method for movement as well as the PlantSeed method for planting. By attaching the Player script to the Player GameObject in the scene and linking _plantPrefab to a prefab of a Plant GameObject I randomly selected from the many sprites provided, it not only represented the visual for a planted seed but also enabled the player to be able to plant the seeds anywhere in the scene. Although I did not think it would be a smooth process, I managed to keep the movement simple and was able to replicate the game with different sprites.

Lastly, the Plant object was much easier than I had assumed. By utilizing Unity's Instantiate function, the Player script spawns a copy of the Plant GameObject at the player's position. This step was short since I only needed to drag the Plant prefab into the _plantPrefab field in the Inspector. Although it does seem like the easiest step, I did struggle a bit figuring out how to connect the Plant prefab.

Upon reflection, my initial plan aligned very closely with how the coding process really turned out. My biggest takeaway was learning how Unity's prefab system simplifies managing and creating objects dynamically. 


## Open-Source Assets
If you added any other outside assets, list them here!
- [Sprout Lands sprite asset pack](https://cupnooble.itch.io/sprout-lands-asset-pack) - character and item sprites
