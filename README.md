# GPU-Powered Fluid Simulation

https://github.com/user-attachments/assets/1b470a56-66d0-4162-a043-c180e653d6a7



https://github.com/user-attachments/assets/5878a233-2988-4307-9254-4490120d3989



A real-time 2D fluid simulation built **entirely from scratch in C++**.

No physics engine. No fluid simulation library. No linear algebra library.

**Click and drag your mouse through the fluid to interact with it in real time.**

## Under the hood

The complete simulation pipeline was implemented from scratch, including:

* Navier–Stokes discretisation
* Diffusion
* Advection
* Pressure projection
* Iterative solving until convergence
* All required linear algebra

After getting the CPU implementation working, I parallelized the computationally expensive grid operations using **OpenGL shaders**.

The result runs at around **40–60 FPS on a 256×256 grid**, while keeping GPU usage relatively low.

### Stack

**C++ · OpenGL · GLSL**

The main goal was simple: **understand how a fluid simulator actually works by building one from the ground up.**
