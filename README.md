# EmotionsDetector
EmotionsDetector is a little software I wrote to look into non-WIMP user interfaces. The program once run requests access to use the camera
and tries to to read the user's emotions using Affectiva API. It then assigns a link to a webpage, youtube video or playlist based on the emotions that it processed.
It is written in HTML and JS


  Hierarchies: For this project:
   There exist the following hierarchies: Class person inherits from THREE.Object3D.


   HOW THE PROGRAM WORKS: The simulation creates three types of objects:
    A cube: This cube acts as the parent to the person objects surrounding, ergo prompting a translated transformation
    in person objects when cube is affected.

    Person: An object that revolves around its parent node, cube.

    Sphere: Sphere is set above the rest of the simulation to mimic a sun At which the main Light is placed.

    MainLight: This object acts as a source of light for the simulation.

    FillLight: this serves as filler light for the simulation.


    scene, camera, renderer: Which work together to set up a scene for the objects to be displayed.

  DESIGN DECISIONS: The simulations contains a scene graph as follows:
  Cube - parent, whose nodes are the person objects declared in an array.

  A class person made of various objects with declared dependencies on each other from which transformations occur
  (arms,legs and head act as children to the parent body).

  CHALLENGES AND DISCOVERIES:
  The biggest problem I faced with the project was figuring out how to make the person objects rotate about
  the origin. I then discovered that if I made the objects children of the cube, then rotating the cube would give me the
  desired result. 
