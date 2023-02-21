# What is WebGL and why use Three.js

## Introduction

Three.js is a 3D JavaScript library that enables developers to create 3D experiences for the web.

It works with WebGL, but you can make it work with SVG and CSS but those two are quite limited.

## WebGL

- JavaScript API
- Render triangles at a remarkable speed
- Result can be drawn in a canvas
- Compatible with most modern browsers
- Uses the GPU

The instructions to place the points and draw the pixels are written in shaders (pixel/fragment, vertex, geometry shaders).

We provide a bunch of information to those shaders like the points positions, model transformations, the camera coordinates and things get positioned and colorized the way we want.

This is why WebGL is so hard. Drawing a single triangle on the canvas would take at least 100 lines of code.

Native WebGL benefits from existing at a low level which enables optimizations and more control.

## Three.js

- JavaScript library
- MIT license
- Right above WebGL
- Created by Ricardo Cabello a.k.a. mrdoob
