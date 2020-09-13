# Assignment 1: Babylon.js and TypeScript

**Due: Monday, September 20, 10:00pm CDT**

This is a skeleton of a small project that will let you build, debug, and run Babylon applications locally.

The objective of this assignment is twofold:
1. Get your computer set up to work with the toolset we are using.
2. Do a little bit of work with Babylon.

## Required Information

You should fill out this information before submitting your assignment.  Make sure to document the name and source (e.g. website URL) for any third party assets such as 3D models, textures, or any other content used that was not solely written by you.

Name: 
UMN Email:
Build URL:
Third Party Assets:

## Rubric

Graded out of 10.

Each of the parts to be added are discussed in one of the lessons in the [Babylon 101](https://doc.babylonjs.com/babylon101/) tutorial.

1. Ensure your program builds with no Typescript warnings. (1)
2. Add a ground plane with some interesting ground texture.  Should be centered under the initial position of the camera. (1)
3. Change the PointLight that is in the sample code to a directional light that is not very bright and not white, and also add one SpotLight to the scene, a reasonable distance above the viewer's initial position. (1)
4. Add at least 5 objects, with interesting materials and/or textures, sitting on the ground. (2)
5. Use keyframe animation to add at least 2 moving objects above the initial viewer position, but below the lights. (2)
6. When you click on one of your objects with the mouse, play a sound and have a particle system shoot particles out from the center of the object. (1)
7. Add shadows, for both the directional and spot lights. (1)

Up to 2 additional bonus points will be given for using interesting textures, lights and materials.  (You won't be judged on aesthetics;  I want you to do more than just cut and paste code and textures from the tutorial.)

## Submission

You will need to check out and submit the project through GitHub classroom.  The project folder should contain just the additions to the sample project that are needed to implement the project.  Do not add extra files, and do not remove the .gitignore file (we do not want the "node_modules" directory in your repository.)

**Do not change the names** of the existing files (e.g., index.html, index.ts, etc).  The TA needs to be able to test your program as follows:

1. cd into the directory and run ```npm install```
2. start a local web server and compile by running ```npm run start``` and pointing the browser at your ```index.html```

Please test that your submission meets these requirements.  For example, after you check in your final version of the assignment to GitHub, check it out again to a new directory and make sure everything builds and runs correctly.

## Development Environment

The sample has already been set up with a complete project for Typescript development.

To work with this sample and prepare your submission, you should have Node (and in particular, npm and npx) installed, which you can retrieve from [nodejs.org](http://nodejs.org).   

In addition to node, you should make sure a recent (e.g., version 3.9 or later) version of Typescript is installed, as described at [www.typescriptlang.org](http://www.typescriptlang.org).

Finally, we will use the node `npx` command to both build the project (with webpack) and run a local http webserver on your machine.  The ```package.json``` is set up to run this server 

## Running 

You set up the initial project by pulling the dependencies from npm with 
```
npm install
```

After that, you can compile and run a server with:
```
npm run start
```

You do not have to run ```tsc``` to build the .js files from the .ts files;  ```npx``` builds them on the fly as part of running webpack.

You can run the sample by pointing your web browser at ```https://localhost:8080/index.html```

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Material for <a xmlns:cc="http://creativecommons.org/ns#" href="https://canvas.umn.edu/courses/194179" property="cc:attributionName" rel="cc:attributionURL">CSCI 5619 Fall 2020</a></span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://illusioneering.umn.edu/" property="cc:attributionName" rel="cc:attributionURL">Evan Suma Rosenberg</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>. 

The intent of choosing (CC BY-NC-SA 4.0) is to allow individuals and instructors at non-profit entities to use this content.  This includes not-for-profit schools (K-12 and post-secondary). For-profit entities (or people creating courses for those sites) may not use this content without permission (this includes, but is not limited to, for-profit schools and universities and commercial education sites such as Coursera, Udacity, LinkedIn Learning, and other similar sites).   

## Credits

This assignment was based upon content from the 3D User Interfaces Fall 2020 course by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.blairmacintyre.me/3dui-class-f20" property="cc:attributionName" rel="cc:attributionURL">Blair MacIntyre</a> at Georgia Tech.