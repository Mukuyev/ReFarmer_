#AI 

## Enemy: Identity & Role

Enemy Name: Bear
Sounds: Bear Sounds
Role in Game: Attacking the tower which we will create, If there is another tower in the way of us, it will just destroy it, or Try to Destroy it. 
Unique Traits: None
## Enemy: Core AI Behaviors

Default State Patrol & Patrol Rout: Will come from Dark Forest and from Forest and Directly come to Attack the tower, no idle state (I think)
Movement: Fixed Path
Animation: Running, Attacking
Purpose: Because there is too much Aura around main tower
Detection/Perception: For Basic There is no Detection

If Detection True;

Sight Range/Cone: How far can it see, and is it a narrow or wide view?
Hearing Range: Can it detect sounds? If so, how far?
Reaction Time: How quickly will it react to a detected player?
Line of Sight Requirement: Can it see through objects?
Detection State Changes: (e.g., Transition from "Patrol" to "Alert" or "Chase")

Movement: Attacking (Chasing)
Attack Pattern: Melee Combo
Attack Cooldown/Speed: 2 Sec
Engagement Distance: For Main Tower, very close 1 m (Melee Type)
Use of Cover/Obstacles: Not
Special Ability Usage: Have not got special ability
Combat State Changes: From "Chase" to "Attack"
Reaction to Damage: Not
Hit Animation/Feedback: How does the enemy react when hit? - Just play some sound and play animation 
Stagger/Knockback: Not
Death Animation/Feedback: Maybe play Niagara effect when dying.
Pathfinding: Only Fixed Route
Use of NavMesh: For now we will use it
Pathfinding Behavior: There will be no obstacles

## Enemy: AI State Machine

States: Chase, Attack, Death           ( Example States e.g., Idle, Patrol, Alert, Chase, Attack, Retreat, Stunned, Death)

Chase: AI will chase (Directly go to the main building)
Attack: AI will directly attack if comes to exact location of main tower or distance is met
Death: AI will die if it's health is 0, but we will not actually kill it, we will make it's health back to Max Health and sent it to the place where they are coming 

Transition Rules:
Chase ==> Attack ------ IF distance is met for main building
Chase & Attack ==> Death ------ If health is 0 or below

DO NOT NEEDED BELOWS 
==(e.g. "When the player enters the sight range of 'Patrol' state, transition to 'Alert'" or "When the health is 0 in 'Attack' state, transition to 'Death'")
==Example:
==Initial State: Patrol
==Transition:
==Player Enters Sight Range -> Alert
==Player within Melee Range (or Ranged Range) -> Attack
==Player Escapes Range -> Chase
==Health reaches 0 -> Death
==Enemy gets hit -> Stunned/Flustered

## Enemy: Difficulty Scaling (Optional)

NOT NEEDED For this AI

Stat Adjustments: (e.g., Increased health, damage, speed on higher difficulty)
Behavior Changes: (e.g., More aggressive, Better cover usage on higher difficulty)
New Abilities: (e.g., Unlocking a new ability on higher difficulty)









