# PocketPals
A mod for Caves of Qud adding various creatures and features from the hit franchise Pokémon.

PocketPals Version 0.29


// intro //

Hello dear friend!

Here is my first released mod. For anything! Ever!
It all began with a couple of screenshots I posted for funsies. Due to the warm reception (and getting stuck on my 'current' project) I have decided to continue and see how far I can get.
So far implementation is simple, there is some evolution, no (or few) proper moves implementation, no wild encounters, and no capturing.
That said, I hope you enjoy my work and find a valuable companion for your journeys.


// installation //

After extracting your download, place the new folder "PocketPals" in your Caves of Qud mod directory (you may need to create the folder):
"C:\Users\Username\AppData\LocalLow\Freehold Games\CavesOfQud\Mods\"


// implementation //

Included Pokémon:

#25 Pikachu^
#35 Clefairy^
#38a Alolan Ninetales
#280 Ralts^*
#281 Kirlia*
#282 Gardevoir
#286 Breloom
#306 Aggron
#359 Absol
#418 Buizel^*
#419 Floatzel
#495 Snivy^*
#496 Servine*
#497 Serperior
#498 Tepig^*
#499 Pignite*
#500 Emboar
#501 Oshawott^*
#502 Dewott*
#503 Samurott
#585 Deerling^
#586 Sawsbuck
#635 Hydreigon
#650 Chespin^*
#651 Servine*
#652 Serperior
#653 Tepig^*
#654 Pignite*
#655 Emboar
#656 Oshawott^*
#657 Dewott*
#658 Samurott
#709 Trevenant

^=Playable
*=Evolves
	Ralts evolution is currently bugged, it throws an error but does not seem to be game breaking

Pokémon with two stages evolve at 12 and 24
Pokémon with one stage evolve at 16

To SUMMON a pokeball of your chosen Pokémon simply use the following wish formula:

-bind Wish in the keybindings menu

-activate Wish:
"Your wish is my command:
[object:AzPx_YourPokémonCap]"

(add the suffix "Cap" (no quotes) to the end of "object:AzPx_Pokemon")
	*For Alolan Ninetales, add prefix "A": ie. AzPx_ANinetalesCap
	*For Deerling and Sawsbuck add the first two letters of a season as a suffix: eg. AzPx_DeerlingSpCap for spring Deerling, AzPx_SawsbuckWiCap for winter Sawsbuck

Notes: 
	-All capsule Pokémon start at Level 1
	-All innate melee attacks have unlimited strength cap, as per natural weapons in CoQ
	-Quadrupedal Pokémon gain a movement speed bonus (partially to make up for the lack of graspers)
	
Typing:
	-Steel and Ghost types do not bleed
	-Fire types do not burn
	-Ghost types gain at-will phasing

Moves:
	Moves considered "Mutations":
		Default Melee Weapons:
		15% attack chance when not primary, can be equipped over and still functions
			-Tackle: 2d4 natural cudgel using body
			-Quick Attack: same as tackle, but also increases maximum charge by 3
			-Flame Charge: as Quick Attack, but deals additional fire damage and deals fire damage on Charge
			-Vine Whip: 2d4 natural cudgel using "bines" (arms)
			-Needle Arm: 2d4 natural cudgel using arms
			-Bite: 2d4 + 1d4 Umbral natural short blade using face
			-Crunch: 2d6 + 1d6 Umbral natural axe using face
			-Leaf Blade: 2d8 long blade using hands
		
		Equipment Slot Melee Weapons:
			-Horn Leech: 2d6 long blade using head with 50% life drain
			-Razor Shell: 2d8 long blade using head (for Samurott)
			
		Ranged Mutations:
			Attacks scale with Ego
			-Bubble
			-Water Gun
			-Thunder Shock: Electric damage
			-Disarming Voice: targets MA
			-Ember: Fire damage, heats targets ala Flaming Ray
			-Psychic: targets MA
			-Flamethrower: Fire damage, heats targets ala Flaming Ray
			-Ice Beam: Cold damage, chills targets
			-Leech Seed: Life drains target based on their toughness
	

Abilities:
	-Swift Swim: large speed boost in pools of liquid
	-Static: 10% chance to paralyze melee attackers
	-Cute Charm: 10% chance to infatuate melee attackers
	-Chlorophyll: Single rank Photosynthetic Skin. Increases Quickness by +25 and Regeneration by 50% after basking

Lore and Physiology:
	-Spined Carapace: Quilladin and Chesnaught get their own variant of carapace. When tightening, AV goes way up, and melee attacks take 1/2 their own Strength in damage
	-Horn Leech and Samurott's Razor Shell add AV
	
	
// playable Pokémon //

I've made a few of the Pokémon playable (the cute, startery ones).
Simply move the files "Genotype.xml" and "Subtype.xml" from the nested folder "Playable" into the mod folder "PokePals" and a third genotype should appear at New Game

Playable Pokémon have only a meager 22 pts for character creation but gain ~22+ more points from their species, this leaves them at or above Mutated Human stats. They also gain stat points upon evolving.

Currently, Pokémon start with random junk in the hopes to give them meaning starting gear.

By default, Pokémon only have access to their own abilities and moves.
	To allow mutations:
		Open "Genotype.xml" now located in the "PokePals" folder.
			Find the item AllowedMutationCategories="" and replace "" with "*" then change MutationPoints="0" to MutationPoints="12" and change BaseMPGain="0" to BaseMPGain="1"
				This will give Pokémon Mutated Human defaults in addition to their natural abilities
				
				enjoy!
				
	To allow cybernetics:
		Open "Genotype.xml" now located in the "PokePals" folder.
			Find the item: IsMutant="true" and change to IsMutant="false"
			
				enjoy!
			
			
//							   //
// to do (loosely by priority) //
//							   //

Add more Pokémon. Open to requests!

Abilities:
	Introduce all abilities of Pokémon contained here. Any new Pokémon will have their abilities added as well. Pokémon with two abilities will have one randomly chosen. Players will be allowed to choose which ability.
			
	Lore:
		Pokémon will have additional abilities based on their biology and lore
	
More Moves and possible Move selection.

Flavor text. Just takes a while to write and make sound all fancy and poetic.

Typing:
	-Water types swim at full speed
	-Steel and Poison types cannot be poisoned
	-Electric types immune to paralysis
	-Type effectiveness
	-I may add my own typing effects based around CoQ mechanics
	
Fainting, capturing, storage, sending out Pokémon. I have some ideas on how to do this, but it may take a while to get it right.

Conversations. Simple conversations with your pals.

SFX. Edited sounds for all moves as well as Pokémon cries when sent out from a ball.

Random encounters. Encounter wild Pokémon in their respective environments. 'Nuff said!


// early release notes //

Pokémon do not have conversations yet, to check their inventory or give them orders, use "Ctrl+Space" when adjacent to them.

I've given some Pokémon tackle which normally do not have these moves. I have done so temporarily until I implement more moves. All Pokémon have Night Vision.

Pokémon and their attacks are not yet balanced. Just like CoQ itself, balance will be in a state of flux and some Pokémon will naturally have an advantage in-game.

Sprites are subject to change. If you are dissatisfied with a current sprite, please be patient, chances are I am too.

The scope of this project is quite large and will take time. That said, I'm open to feedback. Please let me know if you find any bugs or discrepencies.


// misc //


Feel free to contact me on the CoQ Discord about Pokémon requests and feature ideas. Find me @psychonoclast#8485

I have included the spreadsheet I used to convert stats from the Pokémon games to CoQ stats. Feel free to peruse! Maybe even add your own.

Spreadsheet explanation:
Stats scale linearly. 60 is consider baseline (16, or at +0 modifier) and stats go up 1 AP for each 10 (rounded) base stat points. Pokémon gain a +1d4-1 (0-3) boost to base stats to similute IV points. Playable Pokémon get +4 avg to each stat and then gain extra stats based on chosen species.
HP = Toughness
Attack = Strength
Defense = AV (0 below 53 Def, +1 each 10) ( Scales linearly will likely change to logarithmic or something)
Sp. Attack = Ego
Sp. Defense = Willpower
Speed = Agility
Lore = Intelligence (11 for most Pokémon)


// special thanks //

Thank you Freehold Games, The Pokémon Company, and GameFreak for making these great games.

Thank you to the Caves of Qud Discord community for helping me along with this project.
