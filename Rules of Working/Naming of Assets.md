Player Controller name, `PC_Name`
Example ==> PC_Player

Player Character name, `BP_Player` if there is multiple modes that character can play as different pawn or character class, `BP_Player_(Name of Mode)`
Example ==> BP_Player
Example ==> BP_Player_UI (If that mode is minigame, you can give it a minigame's name also)
Example ==> BP_Player_Lobby

Game Mode name, `GM_Name(OrModeName)`
Example ==> GM_Game
Example ==> GM_Lobby

Input Mapping Context name, `IMC_Name`
Example ==> IMC_Movement

Input Action name, `IA_Name`
Example ==> IA_Shoot

Parent actor name, `BP_(SystemThatActorIsGoingToBeUsed)_Parent` 
Example ==> BP_Interactable_Parent

Any actor name, `BP_(IfFromSystem, IncludeName)_Name` 
Example ==> BP_Torch
Example ==> BP_Interactable_Button

Interface name, `BPI_Name`
Example ==> BPI_Interaction

Actor Component name, `BPC_Name`
Example ==> BPC_Inventory

Scene Component name, `BPSC_Name`
Example ==> BPSC_Turret
(?)

AI Controller name, `AIC_Name`
Example ==> AIC_Base

AI Class name, `AI_(Type)_Name`
Example ==> AI_Defense_Jack (:DDDDD)
(?)

Behavior Tree name, `BT_Name(orType)`
Example ==> BT_RangedEnemy
Example ==> BT_BaseEnemy

Blackboard name, `BB_Name(orType)`
Example ==> BB_Base
Example ==> BB_RangedEnemy 

Behavior tree task name, `BTT_TaskName`
Example ==> BTT_CalculateDistance

behavior tree decorators name, `BTD_DecoratorName`
Example ==> BTD_IsInRange

UI naming, `WB_Name`
Example ==> WB_Inventory

HUD naming, `HUB_Name(orMode)`
Example ==> HUD_Lobby
Example ==> HUD_Game


Niagara Emitter, `NE_Name`
Example ==> NE_Burst

Niagara System, `NS_Name`
Example ==> NS_Firework

Niagara modules, `NM_Name`
Example ==> NM_isInRange

Niagara parameter collection, `NP_Name`
Example ==> NP_Wind

Material name, `M_Name`
Example ==> M_Name

Material instance name, `MI_Name`
Example ==> MI_Red

Texture name, `T_Name`
Example ==> T_Table
(?)

Level name, `LI_Name`
Example ==> LI_Jungle

Static Mesh name, `SM_Name`
Example ==> SM_Table

Enumeration name, `E_Name`
Example ==> E_DamageTypes

Data table names, `DT_Name`
Example ==> DT_Inventory

Structure name, `STR_Name`
Example ==> STR_ItemData

Data asset name, `DA_Name`
Example ==> DA_WeaponBase
