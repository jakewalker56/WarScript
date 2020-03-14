# WarScript
Javascript framework for a scripting RTS strategy game

## Usage
Clone the git repo into a local folder, then open index.html in a browser, and the game should execute with the default Warrior1.js and Warrior2.js strategies competing against each other (as of now, they are identical)

To write your own Warrior, define a Warrior1 object and add an Execute function.  Execute takes a warplan object that describes the current state of the world.  Execute returns a warplan object that specifies the movements and actions each of its units and bases will take in the next step of the game.  See Warrior1.js for specifics.

## Bases
Bases can produce units, but have a cooldown period of 1 second after doing so.

## Units
There are currently 7 unit types that are spawnable at the base

#### BRAWLER
Brawlers are melee units.  They are not particularly fast, but they are reasonably strong

#### GUNNER
Gunners are basic ranged units.  They have a short firing range, but a fast firing rate

#### SNIPER
Powerful long distance ranged unit.  Low health, low speed, and low rate of fire

#### SCOUT
Scouts are cheap and fast.  They are best used to run around the battlefield collecting resources

#### TANK
Extremely powerful, slow, long range, and high damage units.  They offer an AOE attack

#### GATLING
Extremely high rate of fire unit.  Excellent against swarms, weak against snipers

#### SWARM
Extremely cheap and fast unit that spawns 3 at a time.  Excellent against Snipers, weak against Gattling and Tanks (if they clump together)

## Resources
There are two types of resources in WarScript- Money and Energy.  You will steadily gain both of these resources just for being alive.

Resources will also appear across the battlefield randomly.  Successful strategies will involve creating scouts to salvage resources, and controlling the middle of the game board to give your scouts access to as many materials as possible
