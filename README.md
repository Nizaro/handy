# handy
This repo is intended to help prepare the experiments based on robotic touch. 

## First Experiment:
We want to complement a monocular view for 3D reconstruction (Depth Anything V2) with touch coming from a robot.
Our goal is to use the embedding coming from Depth Anything V2 combined in a model with different touches that can help to obtain 3D position/ orientation (i.e. 3D position plus normal)
We can also see the hand contact not only as a position and normal estimation, but as a curvature estimation.

We want a model that can output the shape of the object

First we can develop a turn table that is holding a camera.
We also need to start with object of different shape : simple cup can be a good begining based on different elipsoids.
For this purpose we will 3D print different cups.

## Evaluation & Data Generation
To support the 3D printing and evaluation process, we developed a dedicated **Cup Generator & Evaluation Pipeline**. This tool allows us to:
- Generate parametric cup variants with controlled geometric deformations (shear, flare).
- Simulate FDM 3D printing artifacts.
- Benchmark **Depth-Anything-V2** on these synthetic variants before real-world robotic testing.

Repo: [cup-generator-depth-eval](https://github.com/635jack/cup-generator-depth-eval)
