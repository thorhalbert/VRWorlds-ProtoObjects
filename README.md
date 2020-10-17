# VRWorlds-ProtoObjects
Protobuf3 3D Object Model for VRWorlds


VRWorld objects are a series of abstracted types, including some initial platonic solids, some industry mesh formats (such as STL, and a packed version of the LDraw Lego format), and eventually complex meshes, textures, and similar objects.

The idea is that each 'entity' will have a complex object, or possibly multiple objects, which comprise it's 3d representation.    The 3d object can be present inside the emissary for the entity, or it can be served up by an object repository cache (by references from the emissary), which can also be local.   Eventually this will also allow dynamic objects to be represented.

These structures are protobuf proto3 structures.   They might be shared via rpc, disk files (or the emissary equivalent), or even shared memory.

Hello world for this is a platonic cube which will represent the deck of the 'Hello **World**', which will be our starting scene in the ultimate Tardis world.   Initial functionality is getting this to be served up by the entity server and permanently fixed in it's location in the world database.
