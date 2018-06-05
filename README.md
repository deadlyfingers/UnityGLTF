# UnityGLTF

[![Join the chat at https://gitter.im/KhronosGroup/UnityGLTF](https://badges.gitter.im/KhronosGroup/UnityGLTF.svg)](https://gitter.im/KhronosGroup/UnityGLTF?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)

Unity3D library for importing and exporting [GLTF 2.0](https://github.com/KhronosGroup/glTF/) assets.

The goal of this library is to support the full glTF 2.0 specification and enable the following scenarios:
- Run-time import of glTF 2.0 files
- Run-time export of glTF 2.0 files
- Design-time import of glTF 2.0 files
- Design-time export of glTF 2.0 files

The library will be modularized such that it can be extended to support additional capabilities in Unity or support additional extensions to the glTF specification.  The library is designed to work with Unity 2017 and above.

## Current Status

Work Items and Issues targeting a 1.0 release of the library can be found in
[Road to 1.0](https://github.com/KhronosGroup/UnityGLTF/projects/1)

## Building
1. Open the Unity project located in `UnityGLTF\`
2. Check `UnityGLTF\Assets\UnityGLTF\Plugins` settings:
  - `JsonNet.../Newtownsoft.Json.dll` binary should be configured for everything but UWP.
  - `JsonNet.../Portable/Newtownsoft.Json.dll` binary should be configured for **UWP** only.

## Localhost server
To get assets do a **recursive** git clone.

`git clone https://github.com/deadlyfingers/UnityGLTF --recursive`

Or if you've already done a git clone then use:

`git submodule update --init --recursive`

Change directory to `UnityGLTF/www` dir and start a localhost server on port **8080**. If you have Python 3 installed you can run a localhost server using:

`python -m http.server 8080`

## Examples

1. Clone or download the repository.
2. Open up the Unity project and run any of the example scenes in `Assets/GLTF/Examples`

You should see something like this:

![GLTF Lantern](/Screenshots/Lantern.png)

