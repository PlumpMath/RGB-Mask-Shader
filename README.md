# RGB-Mask-Shader
RGB-Masking Shader for Blender as material overwrite

## Description
There a different approaches to render RGB-Mask passes for external compositing in Photoshop or any other compositing software. This is a approach with built in Blender tools by using a shader and the pass index in Blender.
Future there will be a little script with shows the assigned channel of all objects in scene.

THE SCRIPT IS WORK IN PROGRESS AND DOES NOTHING RIGHT AT THE MOMENT. ONLY THE SHADER WORKS.

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
Blender 2.76

## Future plans
1. Adding a overview to the Blender interface to see which channel is assigned objects in scene
2. Adding the shader to a scene by using a button in Blender
