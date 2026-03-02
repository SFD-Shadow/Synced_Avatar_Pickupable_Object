# Synced Avatar Pickupable Object
A system for adding a synced pickupable object to your VRChat avatar.  
Object can be picked up and rotated by all players, local and remote.  

This system includes a modular prefab, FX controller, and parameters list.  
The prefab spawns at (0, 0, 0) but can be parrented/constrainted to fit individual needs.  

### Uses
- 1 Total Memory/Parameters
- 3 Physbones
- 1 Contact Reciever
- 3 VRC Constraints

### Hierarchy  
```
▼ SFD_ObjectPickup  
ㅤ▼ Main  
ㅤㅤ▼ Parrent_M1  
ㅤㅤㅤ▼ Grab  
ㅤㅤㅤㅤ▼ Space  
ㅤㅤㅤㅤㅤㅤYour Object  
▼ Rotation  
ㅤㅤRotationConstraint  
ㅤ▼ Rotation Phys  
ㅤㅤ▼ Rotation Phys Y  
ㅤㅤㅤㅤParrent_RY  
ㅤㅤㅤ▼ Rotation Phys X  
ㅤㅤㅤㅤㅤParrent_RX2
```

### How it Works
This system uses a pickupable and poseable Physbone for the position of the object.  
For the rotation, it uses 2 physbones that rely on collision with the avatar's hand & finger colliders.  
> [!IMPORTANT]
> Differences between avatar's hand/finger collider, as well as size difference can cause issues or desync
