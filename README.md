# Particle Collision Simulator

This is a 3D particle collision simulator created using Python's `vpython` library. The simulation models particle motion and interactions in a particle accelerator-like environment, where protons collide, creating secondary particles like neutrons and pions. The simulation also features a visual interface with dynamic effects such as glowing trails, shockwaves, and sparks.

## Features

- **Particle Movement**: Simulates the motion of particles (protons, neutrons, and pions) inside a cylindrical beam pipe.
- **Collision Handling**: Particles interact with each other, and when they collide, they generate sparks, shockwaves, and produce new particles.
- **Visual Effects**: Includes glowing trails for particles, shockwaves from collisions, and realistic particle behavior.
- **Heads-Up Display (HUD)**: Tracks the number of particles, collisions, and energy in the system.
- **Custom Lighting & Textures**: Beautiful ambient lighting with metallic textures for components and glowing particle effects.
  
## Installation

1. **Install Python**: Ensure that Python 3.x is installed on your system.
   
2. **Install Dependencies**: Use `pip` to install the necessary libraries. You can install them by running:

    ```bash
    pip install vpython numpy
    ```

## How to Run

1. Clone or download the repository:
   
   ```bash
   git clone https://github.com/your-username/Particle-Collision-Simulator.git
   
2. Navigate to the project directory and run the script:

    ```bash
    python particle_simulator.py
    ```

The simulation will start in a new window, displaying the 3D simulation of particles and their interactions.

## How It Works
### Key Components:
- Particles: Each particle is an instance of the Particle class, which includes properties like position, velocity, radius, mass, and charge. Particles leave glowing trails as they move through the scene.

- Collision Detection: The are_colliding function checks if two particles are within their radii of each other. Upon collision, particles are removed and new ones (proton, neutron, pion) are created.

- Visual Effects: Upon collision, an explosion effect is triggered, including sparks and shockwaves expanding outward. The color and size of the sparks change over time.

### The Simulation Loop:
The main simulation loop continuously updates particle positions, checks for collisions, and manages the dynamic visual effects. When particles collide, they are replaced by a set of new particles. The simulation runs until a maximum number of collisions is reached.

## Example
Simulation Output
The simulation shows the particles moving inside a beam pipe, and when they collide, they produce sparks and shockwaves. The heads-up display (HUD) on the top-left shows information about the current number of particles, collisions, and energy in the system.
<br>
<br>

![3D Simulation](3D%20simulation%20pic.jpg)
<br>
<br>

## Future Improvements
- Particle Types: Add more particle types with different properties (e.g., electrons, neutrinos).
- Performance: Optimize for handling large numbers of particles and real-time interactions.
- User Interface: Add controls to adjust particle velocities, add/remove particles, or modify the environment in real-time.
  
## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgements
`VPython` for 3D rendering.
<br>
`Numpy` for numerical calculations.
