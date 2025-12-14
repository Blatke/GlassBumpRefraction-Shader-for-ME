# GlassBumpRefraction Shader for ME
It's a shader mod for HS2 / AI-Shoujo Studio, letting an object be rendered as a refractive glass. This mod is based on [GlassBumpRefraction.shader](https://github.com/Blatke/GlassBumpRefraction.shader).

![AI_2025-12-13-22-37-11-291](https://github.com/user-attachments/assets/e26dd36f-a304-4626-a051-88cf45b1ea07)

## How to Use
Download the **.zipmod** file for the latest version on the [Release](https://github.com/Blatke/GlassBumpRefraction-Shader-for-ME/releases) Page, then drag and drop it into your **/mods/** folder to finish installation, or use KKManager to install this mod.

In Studio, select the object you want to change the shader, and open MaterialEditor tab. Assign _Shader_ option to **Blake/GlassBumpRefraction**. In the following figure, I changed the shader of the plane item to this Shader.

![AI_2025-12-13-22-37-45-547](https://github.com/user-attachments/assets/16ba7905-92dc-493f-84e9-b56492e39ad4)

If you don't need the shadow casted by the plane as a glass, can switch off the option of _Shader Casting Mode_ of its material on MaterialEditor tab.

## List of Properties
### Maps
1. **BumpMap** - indicating how the surface does bump and refraction. It has a hexagon texture by default. The following figure shows the effect by importing another bump map.

![AI_2025-12-13-22-40-43-363](https://github.com/user-attachments/assets/92320389-d1b3-401e-ad90-9a0e12b144a7)

2. **ColorMask** - indicating what parts to have refraction and what parts not to. This should be imported an RGB(A) texture, in which the highest value in RGB channels is recognized as full refraction and 0 value means no such refraction. This value is also multiplied by alpha channel. It has a pure white texture by default.
3. **MainTex** - Main map or Albedo.
### Colors
1. **Color** - base color being multiplied by value of MainTex. Alpha channel indicates the transparency.
### Parameters
1. **BumpMapScale** - scaling multiplier for BumpMap.
2. **BumpMapScale_XY_Ratio** - X/Y ratio in BumpMapScale.
3. **BumpMapStrength** - intensity of BumpMap.
4. **BumpMapRotate** - rotation of BumpMap.
5. **Distortion** - affecting offset of refraction.
6. **RefractionIndex** - affecting direction of refraction.
7. **RefractionDepth** - affecting offset of refraction.
8. **ColorMaskStrength** - multiplier of ColorMask.
9. **ColorMaskInvert** - when 1.0, ColorMask is flipped.

## About Me
Bl@ke

Front Page: https://www.blatke.cc

Discord Server: https://discord.gg/nc5pmnf8X3

QQ Chatgroup for Modders: 904857543
