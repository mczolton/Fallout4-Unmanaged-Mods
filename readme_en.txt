//++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
//ENBSeries is a set of graphical modifications for games
//Description on the web page may not be equal to this info.
//created by Boris Vorontsov http://enbdev.com
//++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++

PUBLISHING BINARY FILES OF ENBSERIES ON NEXUS SITES (FALLOUT NEXUS, TES NEXUS, ETC)
IS STRICTLY PROHIBITED. ONLY PRESETS AND SHADERS CAN BE HOSTED THERE.



ENBSeries v0.286 beta for Fallout 4.

Added support of temporary render targets for enbeffectpostpass.fx shader file and
new textures for it, temporary targets have predefined formats and full screen size.
Added enbadaptation.fx external shader for eye adaptation effect. Added adaptation
parameters to enbseries.ini config file. Changed format of main enbeffectpostpass.fx
render targets to 16 bit per channel format to hide color banding completely. Added
dithering to reduce color banding artifacts for game hdr texture. Fixed all reported bugs.


WARNING! For compatibility with some other software (i call it crapware) read "problems"
category of this document, it's very important to not have any other tools hooking in to
game process or graphics. Crashes, graphic artifacts after installing ENB mods/patches
almost always means crapware is running.

//++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
//CHANGES LOG
//++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Version 0.285:
Added support of external enbeffectpostpass.fx shader, which is replacement of
effect.txt shader. Sample file is included, but file format may change after
discussion with modders, so it's just preview. Fixed reported bugs of previous
version. Added parameter to toggle post pass shader.

Version 0.284:
First release of graphic mod as beta test. ENBoost part of it is included and recommended
for performance reasons instead of version 0.283. Added support of external enbeffect.fx
shader and some parameters in enbseries.ini. This version do not have any changes to visuals
by default and require editing of shader (except color correction parameters). I just need
to get statistics if everything works properly and if new file standart is good enough for
custom shaders.

Version 0.283:
Added draw calls statistics to profiler. Added UsePatchSpeedhackWithoutGraphics parameter
to enblocal.ini to disable graphic modification code for maximal performance.

Version 0.282:
Did workaround for Steam GameOverlayRenderer64.dll library which hooks in to game even
when Steam overlay disabled which crashes with the ENBoost.
Added memory control feature to avoid lod issues for users with not enough physical
vram size and for future mods, modify enblocal.ini [MEMORY] category based on information
reported by VRamSizeTest dx11 tool (do not set value bigger than reported by it).
Added ApplyStabilityPatch parameter which toggles off bugfixes, but keep vram adjust feature.
Added fix for the bug with ENBoost startup message or editor visible on character face, it
also should improve game stability (active only when ApplyStabilityPatch=true is set).

Version 0.281:
This build named ENBoost because of similar functionality to Skyrim and Fallout 3 ENBoost.
Added memory control feature to avoid lod issues for users with not enough physical
vram size and for future mods, modify enblocal.ini [MEMORY] category based on information
reported by VRamSizeTest dx11 tool (do not set value bigger than reported by it).
Added ApplyStabilityPatch parameter which toggles off bugfixes, but keep vram adjust feature.

Version 0.280:
First release for Fallout 4, patch may fix some game specific issues. I can't test it
myself, because not suffering from bugs yet, so any reports please post on the forum
of ENBSeries. Added DisableFakeLights to enblocal.ini to remove unrealistic back
lighting for characters.



//++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
//INSTALL
//++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Extract files from folder Patch or WrapperVersion to your game folder, where game
execution file exist.



//++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
//PROBLEMS
//++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
If game crashing or work not as expected, make sure you are not running XFire, Afterburner,
EVGA, Steam overlay, screen and video capturing tools, GeForce Experience, Razer and Logitek
utils, other kind of tools and overlays (crapware). Antiviruses and various fake boosters
also may affect the mod.



//++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
//
//++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
http://enbdev.com
Copyright (c) 2007-2015 Vorontsov Boris (ENB developer)



//++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
//USED THIRD PARTY CODE/MIDDLEWARE AND THEIR LICENSES (THESE ARE NOT MOD LICENSES)
//++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
Using AntTweakBar
Copyright (C) 2005-2015 Philippe Decaudin
AntTweakBar web site: http://www.antisphere.com


Using 3Dmigoto
3Dmigoto authors: Chiri, Bo3b Johnson, Ulf Jalmgrant (AKA Flugan), Ian Munsie (AKA DarkStarSword)

The MIT License (MIT)

Copyright (c) 2014-2015 the 3Dmigoto project authors (see the file AUTHORS.txt
for a complete list)

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
