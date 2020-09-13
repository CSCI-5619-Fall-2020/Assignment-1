# Assignment 1: Babylon.js and TypeScript

**Due: Monday, September 20, 10:00pm CDT**

This is a skeleton of a small project that will let you build, debug, and run Babylon applications locally.

The objective of this assignment is twofold:
1. Get your computer set up to work with the toolset we are using.
2. Do a little bit of work with Babylon.

## Submission Information

You should fill out this information before submitting your assignment.  Make sure to document the name and source (e.g. website URL) for any third party assets such as 3D models, textures, or any other content used that was not solely written by you.

Name: 
UMN Email:
Build URL:
Third Party Assets:

## Rubric

Graded out of 10 points. Each of the parts to be added are presented in lecture or covered in one of the lessons in the [Babylon 101](https://doc.babylonjs.com/babylon101/) tutorials.

1. Ensure your program builds with no Typescript warnings. (1)
2. Add the debug layer to your scene. (1)
3. Add a ground plane with some interesting ground texture.  Should be centered under the initial position of the camera. (1)
4. Add a SpotLight to the scene that is a color other than white, located a reasonable distance above the viewer's initial position. (1)
5. Use the MeshBuilder to add at least 2 objects with interesting materials and/or textures, sitting on the ground. (2)
6. Use keyframe animation to add at least 2 moving objects above the ground, but below the lights. (2)
7. Add shadows for both the directional and spot lights. (1)
8. Build the program by executing `npm run build` and then upload the contents of the `dist` folder to your public `.www` directory.  Make sure to set the permissions so that it loads correctly in a web browser.  You should include this URL in submission information section of your `README.md` file. (1)

**Bonus Challenge:** When you click on one of your objects with the mouse, play a sound and have a particle system shoot particles out from the center of the object. (1)

**Notes:** This assignments assumes that you will find your own texture images on the internet.  Make sure to document all of these third party assets. You won't be judged on aesthetics, but I do want you to do more than just copy from the tutorials.

## Submission

You will need to check out and submit the project through GitHub classroom.  The project folder should contain just the additions to the sample project that are needed to implement the project.  Do not add extra files, and do not remove the `.gitignore` file (we do not want the "node_modules" directory in your repository.)

**Do not change the names** of the existing files.  The TA needs to be able to test your program as follows:

1. cd into the directory and run ```npm install```
2. start a local web server and compile by running ```npm run start``` and pointing the browser at your ```index.html```

Please test that your submission meets these requirements.  For example, after you check in your final version of the assignment to GitHub, check it out again to a new directory and make sure everything builds and runs correctly.

## Development Environment

The sample has already been set up with a complete project for Typescript development.

To work with this sample and prepare your submission, you should have Node.js installed, which you can retrieve from [nodejs.org](http://nodejs.org) or by downloading `npm` using a package manager.

In addition to Node, you should make sure a recent (e.g., version 3.9 or later) version of Typescript is installed.  The easiest way to do this is by executing `npm install --global typescript`.

Under the hood, we are using the Node `npx` command to both build the project (with webpack) and run a local http webserver on your machine.  The included ```package.json``` file is set up to do this automatically.

## Running 

After checking out the project, you need to initialize by pulling the dependencies from npm with:
```
npm install
```

After that, you can compile and run a server with:
```
npm run start
```

You do not have to run ```tsc``` to build the .js files from the .ts files;  ```npx``` builds them on the fly as part of running webpack.

You can run the sample by pointing your web browser at ```https://localhost:8080```.

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br /><span xmlns:dct="http://purl.org/dc/terms/" property="dct:title">Material for <a xmlns:cc="http://creativecommons.org/ns#" href="https://canvas.umn.edu/courses/194179" property="cc:attributionName" rel="cc:attributionURL">CSCI 5619 Fall 2020</a></span> by <a xmlns:cc="http://creativecommons.org/ns#" href="https://illusioneering.umn.edu/" property="cc:attributionName" rel="cc:attributionURL">Evan Suma Rosenberg</a> is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>. 

The intent of choosing (CC BY-NC-SA 4.0) is to allow individuals and instructors at non-profit entities to use this content.  This includes not-for-profit schools (K-12 and post-secondary). For-profit entities (or people creating courses for those sites) may not use this content without permission (this includes, but is not limited to, for-profit schools and universities and commercial education sites such as Coursera, Udacity, LinkedIn Learning, and other similar sites).   

## Credits

This assignment was based upon content from the 3D User Interfaces Fall 2020 course by <a xmlns:cc="http://creativecommons.org/ns#" href="https://github.blairmacintyre.me/3dui-class-f20" property="cc:attributionName" rel="cc:attributionURL">Blair MacIntyre</a> at Georgia Tech.