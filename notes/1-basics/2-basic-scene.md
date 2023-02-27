# Elements

- A scene that will contain objects
- Some objects
- A camera
- A renderer

## Scene

- Like a container
- We put objects, models, lights, etc. in it
- At some point we ask Three.js to render the scene

```js
const scene = new THREE.Scene();
```

## Objects

Can be many things

- Primitive geometries
- Imported models
- Particles
- Lights
- etc.

### Mesh

A mesh is the combination of a geometry (shape) and a material (looks)

```js
const geometry = new THREE.BoxGeometry(1, 1, 1);
const material = new THREE.MeshBasicMaterial({ color: 0xff0000 });
const mesh = new THREE.Mesh(geometry, material);
```

## Camera

- Not visible
- Serves as a point of view when doing a render
- Can have multiple and switch between them
- Different types

```js
const camera = new THREE.PerspectiveCamera(fov, aspectRatio, ...);
```

### Field of view

- Vertical vision angle
- In degrees
- Also called `fov`

### Aspect ratio

The width of the render divided by the height of the render.

## Renderer

- Renders the scene from the camera fov.
- Result drawn into a canvas
- A canvas is a HTML element in which you can draw stuff
- Three.js will use WebGL to draw the render inside the canvas
- You can create it or you can let Three.js do it

```js
const renderer = new THREE.WebGLRenderer({
  canvas: document.querySelector('.webgl'),
});
```
