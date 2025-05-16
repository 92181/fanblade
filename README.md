# Turbine Fan Generator
A flexible turbine fan generator using multiple curves for control, written in Javascript. The turbine generator itself has no dependecies, for viewing purposes WebGPU is used. 
I created this project because I wanted to use it to generate fan blades for my drone, in any size, with any amount of fanblades, many more settings can be tweaked.

Various things that can be done are...
* You can dynamically change the size of the blades, the cut-off point relative to the propellor shroud & the amount of fan blades. 
* Change the curvature of the fanblades, fanblade shroud. You can also quite easily change the tickness of the blades while manipulating the curves. 
* The final result can be easily exported to an STL file, to do this you need to press the P key.

The curvature of the blade is controlled by multiple bezier curves, wich can be easily tweaked in the code itself, alongside many other settings. Some settings are harder to change than others.

# Usage
You can run the viewer and generator by cloning the Github project and running a simple HTTP file server.
As of 2025 WebGPU only works with Chrome.

```sh
python3 -m http.server
```

Then you can move around within the scene with your keyboard and rotate with a mouse.
- `WASD` To move around the WebGPU scene.
- `P` Press the P key to generate and download an STL file of the turbine.

# Pictures
<p align="center">
  <img src="./images/0.png" width="45%">
  &nbsp; &nbsp; &nbsp; &nbsp;
  <img src="./images/1.png" width="45%">
</p>

# License & References
This project uses the MIT Attribution license. If you like this project consider starring it.

For the WebGPU renderering references were taken from samples by [WebGPU Samples](https://github.com/webgpu/webgpu-samples).
