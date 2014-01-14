Chrome Security Issue
---------------------

Google Chrome will prevent our 3D games from running when the files are stored on our computer instead of on a web server. To get around this issue make sure Chrome is completely closed. Open a command prompt and enter the command:

```
open -a Google\ Chrome --args --disable-web-security
```

Blender Basics
--------------

Blender is a free 3D modeling and animation program. It will make the process of creating 3D models for our game much easier.

[Download Blender](http://www.blender.org/download/)

Blender can be a little confusing to get started with, but is very powerful once you learn the basics. There are many shapes that you can use as a starting point for more complex models. Look under the Add menu on the top main bar to see all your options. Once you add a shape, switch to Edit Mode and set viewport shading to Wireframe. These options can be found towards the bottom of the screen. Now you can use the following keyboard commands to make changes to the shape.

A: Deselect everything
B: Select
S: Scale
G: Move
E: Extrude
Ctrl+R: Duplicate

Export For Three.js
-------------------

After creating a model in Blender we can save it as a specific type of file that we can then use in our game. Make sure your model is selected, then in the top menu bar choose File -> Export -> Collada. Navigate in the file browser to the models folder of our game project and give your model file a name. Remember what you name the file because you will need it later.

Load Model in Three.js
----------------------

Open our game project folder in Sublime Text. Then click on index.html to view the code. Find this line of code and change 'pawn' to the name of your model file.

```
loadColladaObject('pawn', material, 1, scene);
```