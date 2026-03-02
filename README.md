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
▼SFD_ObjectPickup
▼Main
▼Parrent_M1
▌▌▌▼Grab
▌▌▌▌▼Space
▌▌▌▌▌Your Object
▼Rotation
▌RotationConstraint
▌▼Rotation Phys
▌▌▼Rotation Phys Y
▌▌▌Parrent_RY
▌▌▌▼Rotation Phys X
▌▌▌▌Parrent_RX2

### How it Works
