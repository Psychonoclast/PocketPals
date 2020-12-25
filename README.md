# PocketPals
A mod for Caves of Qud adding various creatures and features from the hit franchise Pokémon.

PocketPals Version 0.11

// intro //

Hello dear friend!

Here is my first released mod. For anything! Ever!
It all began with a couple of screenshots I posted for funsies. Due to the warm reception (and getting stuck on my 'current' project) I have decided to continue and see how far I can get.
So far implementation is simple, there is no evolution, no (or few) proper moves implementation, no wild encounters, and no capturing.
That said, I hope you enjoy my work and find a valuable companion for your journeys.

// installation //

After extracting your download, place the new folder "PocketPals" in your Caves of Qud mod directory (you may need to create the folder):
"C:\Users\Username\AppData\LocalLow\Freehold Games\CavesOfQud\Mods\"


// implementation //

Included Pokémon:

#25 Pikachu
#35 Clefairy
#38a Alolan Ninetales
#280 Ralts
#286 Breloom
#306 Aggron
#359 Absol
#418 Buizel
#495 Snivy
#498 Tepig
#501 Oshawott
#585 Deerling
#586 Sawsbuck
#635 Hydreigon
#709 Trevenant

To SUMMON a pokeball of your chosen Pokémon simply use the following wish formula:

-bind Wish in the keybindings menu

-activate Wish:
"Your wish is my command:
[object:AzPx_YourPokémonCap]"

(add the suffix "Cap" (no quotes) to the end of "object:AzPx_Pokemon")

For Alolan Ninetales, add prefix "A": ie. AzPx_ANinetalesCap
For Deerling and Sawsbuck add the first two letters of a season as a suffix: eg. AzPx_DeerlingSpCap for spring Deerling, AzPx_SawsbuckWiCap for winter Sawsbuck

All innate melee attacks have unlimited strength cap, as per natural weapons in CoQ. Thunderbolt, Icebeam, etc. will scale with Ego. Physical projectiles will likewise use strength (When some are implemented).

// Playable Pokémon //

I've made a few of the Pokémon playable (the cute, startery ones).
Simply move the files "Genotype.xml" and "Subtype.xml" from the nested folder "Playable" into the base folder "PokePals" and a third genotype should appear at New Game

// to do (loosely by priority) //

-Add more Pokémon. Open to requests!
-Moves and Abilities. I'm planning moves as Mutations in various capacities, but I also enjoy that Pokémon can use their physical features for combat as well. I might not limit Pokémon to four moves, or cause certain moves to automatically upgrade to more powerful versions.
-EVOLUTION! Pokémon will change form (Tile, Stats, and Anatomy) once reaching a certain level. Both Trainers and Playable Pokémon will be able to choose whether or not to evolve.
-Flavor text. Just takes a while to write and make sound all fancy and poetic.
-Typing. Pokémon will recieve certain advantages based on type. Eg. Water types swim at full speed, Steel and Poison types cannot be poisoned, Dark types are immune to Psychic type moves, Ghost types gain innate phasing, etc. I may add my own typing effects based around CoQ mechanics.
-Fainting, capturing, storage, sending out Pokémon. I have some ideas on how to do this, but it may take a while to get it right.
-Conversations. Simple conversations with your pals.
-SFX. Edited sounds for all moves as well as Pokémon cries when sent out from a ball.
-Random encounters. Encounter wild Pokémon in their respective environments. 'Nuff said!

// early release notes //

Pokémon do not have conversations yet, to check their inventory or give them orders, use "Ctrl+Space" when adjacent to them.

I've given some Pokémon tackle or bite which normally do not have these moves. I have done so temporarily until I implement more moves. All Pokémon have Night Vision.

Pokémon and their attacks are not yet balanced. Just like CoQ itself, balance will be in a state of flux and some Pokémon will naturally have an advantage in-game.

Sprites are subject to change. If you are dissatisfied with a current sprite, please be patient, chances are I am too.

The scope of this project is quite large and will take time. That said, I'm open to feedback. Please let me know if you find any bugs or discrepencies.

// misc //

Feel free to contact me on the CoQ Discord about Pokémon requests and feature ideas. Find me @psychonoclast#8485

I have included the spreadsheet I used to convert stats from the Pokémon games to CoQ stats. Feel free to peruse! Maybe even add your own.

Spreadsheet explanation:
Stats scale linearly. 60 is consider baseline (16, or at +0 modifier). Pokémon gain a +1d8 (+1-8) boost to base stats to similute IV points. Playable Pokémon get +4 avg to each stat, but gain extra stats based on chosen species.
HP = Toughness
Attack = Strength
Defense = AV (0 below 53 Def) (May change to logarithmic, to cap off AV at high levels)
Sp. Attack = Ego
Sp. Defense = Willpower
Speed = Agility
Lore = Intelligence (11 (+1 = 12) for most Pokémon)

