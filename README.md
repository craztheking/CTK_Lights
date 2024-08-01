# CTK_Lights
Breakable/Switchable Lights with Fuse Box (Insurgency Sandstorm)

Extract CTK_LightSystem into X:\SandstormEditor\Insurgency\Content
Once Inside editor Move CTK_LightSystem into your Maps Content Folder


BP__CTK_Fuse_box
Fuse box is breakable, parallel to original fuse boxes in game.
Inside Defaults, link all lights that will shut off when this fuse is broken.


BP_CTK_Switch
Inside Defaults, link all lights that are toggable by this switch.


BP_CTK_Light
Refrence this for new lights otherwise Fuse box and Switch will be unusable with this BP.
Inside Defaults,
On Material; Lit material (Uses Emissive)
Off Material; Broken material (No Emissive)
Break Particle; Particle effect used once broken.
Break Sound; Sound Effect used once broken.
Use Spot Light; This is a toggle to swap between Spot and Point Lights.
Use Hitbox; This is used to pinpoint a damage area, instead of the light being broken when damaging any part of your lights mesh.
View Hitbox; Shows the hitbox, used to scale or move hitbox position, make sure to toggle this off when completed or it will be shown in game.

Unused, do not change these, they are refrenced by blueprint only.
Fuse On
Is Broken
Is On

Also; Light Properties are not used, the BP was origianlly derrived from Base Light Blueprints.

Positions that may need to be adjusted when creating your own child;

Light and LightBroken, This is often need to be rotated 180 on X or Y Axis.

AK; This may need to be adjusted to change the location sound is projected from when breaking the light.

PointLight, SpotLight, LightBeam; When moving PointLight, the others are attached and will move with. Light Beam Template may need to be changed to match your light, alongside the position of Light Beam may need to be adjusted.

Hit Box; When used this will need to be adjusted to accomodate the damageable area to break the light.
