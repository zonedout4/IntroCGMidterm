# IntroCGMidterm

## Ring Shader (Reflection)
I created a Shader Graph using reflection for the rings. It differs from the one done in class because it is a lit shader instead of calculating diffuse and ambient light manually. It uses the same Shader Graph logic used in Lecture 4 to simulate specular lighting and simply adds it to the base colour. I added floats so that I could edit the metallic and smoothness values of the material. This suits the scene because the rings are supposed to be shiny metal.

## Waterfall Shader (Texture Tiling)
I created a Shader Graph using texture tiling and offset for the waterfall. It works by adding time to a direction vector, which controls the speed and direction that the texture moves. For the waterfall, since I want it to go straight down, the direction vector is set to 0, -1. Then, I plug that result into a Tiling and Offset node to properly output a UV. That UV output goes into sample texture, which is multiplied by base colour for the final result. This suits the scene because a texture moving downwards is a simple yet effective way to create the illusion of falling water.
