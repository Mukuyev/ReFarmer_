---

kanban-plugin: board

---

## AI Management

- [ ] Change P_AISpawnPoints from Actor Class to Object Class (I think I can not change this due to Object class does not have got All the capabilities for existing in level)
- [ ] Extreme: Change The all AI system to the Instance Static Mesh System where as we know that every AI has got a same static mesh but they are instanced
- [ ] Fixing AI Controller Problem where we are spawn tons of AI, their controller also works with them, if we can decrease the background usage of it, we may increase out performance.
	Look For: Disabling enabling AI controller, Posses or Unposses the AI controller
- [ ] May affect the optimization, Maybe AI Move to works in the background, check it if it works in the background or not, if works disable it after their health is 0
- [ ] NavMesh needs to be fixed; Problem is AIs are stopping weirdly
- [ ] Need to send data of spawned and dead from spawner to main place to our spawner, Basically finishing our object polling system
- [x] When are we using the change location of a mesh when set visibility to false, meshes are overlapping and goes to the different places of map which means it is a bug
- [ ] Maybe?
	AIs Spawns at the same location
- [x] Implementing different collision for AI and Towers
- [x] Problem; Reference one and not reference one called twice for each AI, fix it


## AI Abilities

- [ ] Creating new Shield System where some of the AIs' are going to implement this system for regenerating their health when they are moving to the goal destination
- [ ] Some AIs' is going to have got overall shield where they are going to implement dividing damage into several pieces and decrease the upcoming damage amount
- [ ] Easily adjustable speed from time to time




%% kanban:settings
```
{"kanban-plugin":"board","list-collapse":[false,false]}
```
%%