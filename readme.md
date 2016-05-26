# gmsv_luapack_internal

A Garry's Mod module that complements the LuaPack project.

## Info

The only supported compilation platform for this project on Windows is Visual Studio 2010.
The only supported compilation platforms (tested) for this project on Linux are GCC/G\+\+ 4.8 or 4.9. However, any version between 4.4 and 4.9 *MIGHT* work.
The only supported compilation platform (tested) for this project on Mac OSX is Xcode 4.1. However, any Xcode version *MIGHT* work as long as the Mac OSX 10.5 SDK is used.
These restrictions are not random; they exist because of ABI reasons.

Mac was not tested at all (sorry but I'm poor).

If stuff starts erroring or fails to work, be sure to check the correct line endings (\n and such) are present in the files for each OS.

This project requires [garrysmod_common][1], a framework to facilitate the creation of compilations files (Visual Studio, make, XCode, etc). Simply set the environment variable 'GARRYSMOD_COMMON' or the premake option 'gmcommon' to the path of your local copy of [garrysmod_common][1]. We also use [SourceSDK2013][5], so set the environment variable 'SOURCE_SDK' or the premake option 'sourcesdk' to the path of your local copy of [SourceSDK2013][5]. The previous links to [SourceSDK2013][5] point to my own fork of VALVe's repo and for good reason: Garry's Mod has lots of backwards incompatible changes to interfaces and it's much smaller, being perfect for automated build systems like Travis-CI (which is used for this project).


  [1]: https://github.com/danielga/garrysmod_common
  [2]: https://github.com/danielga/sourcesdk-minimal
