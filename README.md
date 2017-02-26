# RGB-Mask-Shader
RGB-Masking Shader for Blender as material overwrite

## Description
There a different approaches to render RGB-Mask passes for external compositing in Photoshop or any other compositing software. This is a approach with built in blender tools.

## Screenshot
![Alt text](screenshot.png?raw=true "Screenshot of Blender")

## Howto
1. Download "RGB-Mask-Shader.blend" from the repository
2. Append the Material "RGB-Mask-Shader" to your scene file
3. Apply this shader to a hidden geometry
4. Create a second render layer in "Render layers" panel called "Mask-Layer"
5. Apply the "RGB-Mask-Shader" to the material overwrite
6. Select the geometry you want to be red/green/blue/black in the "Mask-Layer"
7. Go to the "Object panel".
8. Under "Relations" you will find a "Pass Index" -> set it to 1 (R), 2 (G), 3(B) or 0 (black)

### Notes
Every geometry without Pass Index (default is 0) will be black

## Requirement
Blender 2.78
