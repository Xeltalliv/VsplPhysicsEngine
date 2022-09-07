## What is this
3D rigidbody physics engine based of:  
1. Ian Millington's book called "Game Physics Engine Development"  
2. https://danielchappuis.ch/download/ConstraintsDerivationRigidBody3D.pdf  
3. http://www.mft-spirit.nl/files/MTamis_Constraints.pdf  

## Features
Each rigidbody can have multiple colliders.  
Colliders:  
1. Planes  
2. Spheres  
3. Boxes  
4. Capsules  

Joints:  
1. Slider joint  
2. Hinge joints  
3. Unvisersal joints  
4. Three axis limited joints  
5. Ball and socket joints (3 axis unlimited)  
6. Shared motion joint (allows to linearly connect movement/rotation of one rigidbody to movement/rotation or another rigidbody)  
7. Center distance  
8. Point distance  

Joints 1-4 support limits and motors  

Force generators:  
1. Global acceleration  
1. Local acceleration  
3. Springs  
4. Buoyancy  

Collision returns multiple contact points.  
Cone friction.  

## Missing features
Doesn't automatically compute center of mass.  
Doesn't use generalized collision detection. There is code for each possible combination of colliders.  
Doesn't preserve contact data from the last frame.  
Doesn't have warm starting.  
Doesn't have sleep optimization.  
Doesn't have coarse collision phase or any data structures to early out collision of far objects.  

## How to compile
1. Press Code -> Download ZIP.
2. Open vspl compiler [on github pages](https://xeltalliv.github.io/ScratchTools/ProgLang/), or download it's [source code](https://github.com/Xeltalliv/ScratchTools/tree/main/ProgLang) and run it locally.  
3. If your browser supports it, unzip this source code and press "Pick directory" and pick the directory that contains everything from this repo (not just src) and allow file reading. If browser doesn't support it, use "Import zip" instead.  
4. Press "Compile"  
5. In case of using "Pick directory", you will be prompted again for file write access. Accept it and compiled project will overwrite "Compiled.sb3" in "output" directory. In case file "Compiled.sb3" doesn't exist, you reject write access or using "Import zip", the compiled project will be downloaded as usually downloading any other files in the browser.  

The demo of this physics engine can be seen [here](https://turbowarp.org/727515422).