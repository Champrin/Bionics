### The following contents are from youdao translation, which may not be correct, please understand
# Bionics -- -- -- -- -- - bionic

    Original RealLife series, and new features
    
## Function introduction

    BedLeaveXT-- players get up and get dizzy and weak
    When the player gets up, the odds are dizziness and weakness
    BedLeaveBX- players sleep for blood
    When the player is empty, fill the blood
    Break the fall
    KuShuZhi------ when you are out of the tree, you will drop the stick
    LuGrass- when you are out of the grass, you will drop the seeds
    LuWoodBlood- when the player drops the wood empty-handed, it will take half the blood
    LuVines- players fall off with their hands
    LuLeaves- players will fall off with their hands
    LuCactus- when the player knocks out the cactus, it will drop 1 to 10 water bottles
    CutIce-- players use swords (wood, stone, iron, gold, diamond swords) to clear the ice
    CutGlass- players use swords (wood, stone, iron, gold, diamond sword) or scissors to drop glass or glass
    CutWatermelon- players use swords (wood, stone, iron, gold, diamond sword) or scissors to drop the entire watermelon
    Adrenaline------ Adrenaline
    When the player USES the dragon breath (ID: 437), he points to the point where it is (equal to the epinephrine), the acceleration, the mining acceleration and the power effect (both of them are 4, 2 minutes).
    AltitudeStress- altitude sickness
    When the player goes to a place higher than 80 (i.e., the coordinates Y is greater than 80), you get the effect of a weak potion
    When a player goes to a place higher than 100 (i.e., Y is greater than 100), you get the vertigo effect.
    When the player goes to a place higher than 120 (i.e., Y is greater than 120), the player dies directly
    Borewood fire --- wood fire
    When the player has a stick of wood, there is a chance to shine a spark and set the bar
    Fallill--- sick system plug-in
    Symptoms of 1.
    * players are poisoned by eating potatoes
    * (when a player is chopped by a sword) the player is stabbed with a sword and the open wound is bleeding, weak and damaging
    * (when the player falls from high) the player has broken his leg and needs a bone.
    * (when the player is burned) the player dies directly from the fire
    * (when players drown) players are tired and drowsy, dizzy and tired
    * (when the player is suffocating) the player suffocates and can't breathe, and dies directly!
    * the player's blood glucose concentration is too low to cause hunger and dizziness when the player's hunger is zero
    2. Drug
    Cure for symptoms: vertigo treatment: food: apples
    * bone is suitable for symptoms: fracture treatment: site items: bones
    * pumpkin pie is suitable for symptoms: weak treatment: food items: pumpkin pie
    * snickers fit for symptoms: starvation treatment: food: bread
    * cookie suit for symptoms: fatigue treatment: food: cookies
    * vitamin A suitable for symptoms: blindness treatment: food: carrot
    Yunnan baiyao is suitable for symptoms: poisoning treatment method: point ground objects: paper
    Fart-- excretion of the plug-in
    When players switch stealth, the player farts, and the chance will be shit
    When players eat their own shit (cocoa beans, eat = point air), get the anti-stomach level of 60 second effect

## Configuration file description (true is open, false is off)
### Worlds. Yml

    Please click on this profile
    - the world
    - tie
    Add the open world as above
    
## The config. Yml

    "LuCactus"=>true, // cactus drop water bottle
    "WaterBottle"=>"1:10", // water bottle drop
    "LuWoodBlood"=>true, // hand pulled back to the blood
    "LuLeaves"=>true, // the leaves fall from the tree
    "CutGlass"=>true, // knife rolled glass drops
    "CutIce"=>true, // the knife is pulled out of the ice
    "LuVines"=>true, // hand pulled down
    "CutWatermelon"=>true, // cut out watermelon dropped
    "BoreWoodFire"=>true, // a log fire
    "FrictionProbability"=>"0:250",// the probability of fire is how much
    "Probability"=>30,// fire Probability
    "AltitudeStress"=>true,// altitude reaction
    "Fart" = > true, / / discharge
    "Fallill"=>true,// sick system
    "Adrenaline"=>true,// Adrenaline
    "LuGrass"=>true,// lu grass drops the seeds
    "KuShuZhi"=>true,// the branch dropped the stick
    "BedLeaveBX"=>true,// sleep for blood
    "BedLeaveXT"=>true,// the chance of getting out of bed is too low
    "Tip"=>true,// prompt message
    
## The Message. Yml configuration file is a custom prompt Message

    LuLeaves: § 6 hand rolled the leaves fall
    CutGlass: § 6 dao lu glass fall off
    CutIce: § 6 dao lu ice fall off
    LuVines: § 6 hand rolled vine fall off
    CutWatermelon: § 6 dao lu watermelon fall off
    BoreWoodFire: § 6 simulated flight light sticks
    LuGrass: § a hand lu grass drop wheat seeds
    KuShuZhi: § 5 hand rolled dead drop stick
    LuCactus:
    1: the positive heading of the headline
    2: § a you find in the cactus bottle {} § § e the subtitle of a bottle of water / / the headlines
    3:2 // the gradient of the headline
    4:2 // the gradient of the headline
    5:40 // the display time of the headline, notice that 20=1s if shown in 10 seconds, input 200
    LuWoodBlood:
    1: "/ / this is the same configuration as LuCactus
    2: § 7 hand lu wood, can damage hand oh ~ ~
    3:2
    4:2
    5:40
    AltitudeStress:
    A1: § b plateau response / / a1 to the a5 are player y coordinates in 80 here, like LuCactus configuration
    A2: § 6 began to make you weak, taller even dizziness could be happening again!
    A3:2
    A4:2
    A5:40
    B1: § plateau response / / b y 100 b1 to b5 are players here, like LuCactus configuration
    B2: § 6 has appeared dizziness, you can't go up again! It might just kill you!
    B3:2
    B4:2
    B5:40
    C1: § b plateau response / / c1 to c5 is y 120 players here, like LuCactus configuration
    C2: § 6 highland oxygen-starved death you!
    C3:2
    C4:2
    C5:40
    Fart:
    1: § § e l you put fart / / players switch stealth fart tip of the popup
    2: § § 6 l you shit/chance/players switch stealth shit popup hint
    3: § § a l you eat shit / / players click on the cocoa prompt information
    4: § § § 6 players b l} {player § § § 6 r actually eat a shit / / when players click cocoa, all take notice
    Adrenaline:
    Tip: § a > adrenaline § § 6 b to strengthen the speed and mining speed, the power / / here is the player with dragon's breath prompt information
    1: § a you hit on the kidney hormone / / 1 to 5 as LuCactus configuration
    2: § 6 to strengthen speed, speed, strength
    3:2
    4:2
    5:40
    BedLeaveBX:
    1: '/ / the same as the LuCactus configuration
    2: § c restore health ~ ~ you go to sleep
    3:2
    4:2
    5:40
    BedLeaveXT: // the same as the LuCactus configuration
    1: § a you just get up cause low blood sugar
    2: § e dizzy and weak effect there will be a short time
    3:2
    4:2
    5:40
    Fallill Interact:
    1: § 6 you have forever / / players click on the bone prompt information
    2: § e you have prompt information detox / / players click on the paper
    Fallill ItemTip: //Fallill is a message for players to hold all kinds of items
    Apple: § a > specific § § 3 b symptoms: dizziness § d treatment methods: § 6 items: apple
    Bones: § a > § § 6 bone b symptoms: § d fracture treatment methods: point to § 6 items: the bone
    Pumpkin pie: § a > pumpkin pie § § f b symptoms: weak § d treatment methods: point to § 6 items: pumpkin pie
    Bread: § a > § e snickers § b symptoms: hunger § d treatment methods: § 6 items: bread
    Cookie: § a > § § 9 cookies for b symptoms: fatigue, § d treatment methods: § 6 items: cookies
    Carrots: § a > b vitamin a § § b symptoms: blind § d treatment methods: § 6 items: carrots
    Paper: § a > yunnan baiyao § § c b symptoms: § d treatment methods: point to § 6 items: paper
    Fallill Consume: //Fallill here is the message that the player eats the item
    1: § a has dizziness ease!
    2: § e swept through hunger, be myself!
    3: § 2 has alleviate fatigue!
    4: § 6 strengthen physical health
    5: § 0 successfully treat blindness!
    6: § c raw potato will poisoning!
    Fallill Event is chopped: // the same as the LuCactus configuration
    1: § b are you sword cut and open wound infection
    2: § e bloodshed, weak and damage effects
    3:2
    4:2
    5:40
    Fallill Event fracture: // the same as the LuCactus configuration
    1: § a break your leg
    2: § 6 need bone!
    3:2
    4:2
    5:40
    Fallill Event burning: // the same as the LuCactus configuration
    Broadcasting: § § § a player b l {name} § § r a bath with fire, death / / take notice of all information directly
    1: § c you bath with fire
    2: § 6 death directly
    3:2
    4:2
    5:40
    Fallill Event drowning: // the same as the LuCactus configuration
    1: § e drowned you too tired
    2: § c have weakness, dizziness, fatigue effect!
    3:2
    4:2
    5:40
    Fallill Event suffocation: // the same as the LuCactus configuration
    Broadcasting: § § § a player b l {name} § § a r because choked, lead to can't breathe, direct death! // information on full service circulars
    1: § c you choked
    2: § 6 lead to can't breathe, direct death!
    3:2
    4:2
    5:40
    Fallill Event is exploded: // the same as the LuCactus configuration
    Broadcasting: § § § a player b l {name} § § r by TNT blown sky-high, a direct death! // information on full service circulars
    1: § c you by TNT blown sky-high
    2: § 6 death directly!
    3:2
    4:2
    5:40
    Fallill Event hunger: // the same as the LuCactus configuration
    1: § 6 your blood glucose is too low
    2: § a lead to hunger, and dizziness.
    3:2
    4:2
    5:40
    
## Instruction is introduced

    /ill check out the drug list
    /rlset help for help
    /rlset reload configuration file
    /rlset true [type] opens a function
    /rlset false [type] closes a function
    /rlset type to view type
