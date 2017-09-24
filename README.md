// Copyright 2010 Intel Corporation
// All Rights Reserved
//
// Permission is granted to use, copy, distribute and prepare derivative works of this
// software for any purpose and without fee, provided, that the above copyright notice
// and this statement appear in all copies.  Intel makes no representations about the
// suitability of this software for any purpose.  THIS SOFTWARE IS PROVIDED "AS IS."
// INTEL SPECIFICALLY DISCLAIMS ALL WARRANTIES, EXPRESS OR IMPLIED, AND ALL LIABILITY,
// INCLUDING CONSEQUENTIAL AND OTHER INDIRECT DAMAGES, FOR THE USE OF THIS SOFTWARE,
// INCLUDING LIABILITY FOR INFRINGEMENT OF ANY PROPRIETARY RIGHTS, AND INCLUDING THE
// WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE.  Intel does not
// assume any responsibility for any errors which may appear in this software nor any
// responsibility to update it.

Date
====
May 2017 - StephanieB5 Updating the code to not rely on the DXSDK.

Date
====
July 2010


Deferred Shading Demo
=====================

This application demonstrates several deferred shading algorithms.


User Interaction
================

- As with other DXSDK samples, use WASD with the mouse (click and drag) to fly
  around the scene.


Requirements for the Windows 10 Visual Studio 2015 update
============

For compilation:

1) Visual C++ 2010 (or later)

For execution:

1) Windows 10
2) DirectX 11 compatible video card
3) Appropriate Visual C++ Redistributable Package (2015)
4) For running outside of the debugger: copy the executable, deferred_shading_W10_VS2015.exe, into the deferred_shading_dx11 folder



Known Issues (dated from 2010)
============
   
1) Output is corrupted on NVIDIA DX11 cards when using the "Quad" deferred
   shading technique. This appears to be a bug in the shader compiler.
   At the time of writing, commenting out the branch on mUI.visualizeLightCount
   (and body) in the GPUQuad function in GPUQuad.hlsl works around the issue.
