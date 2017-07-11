# Intro to A-Frame

[A-Frame](https://aframe.io/) is a powerful tool for creating virtual reality experiences to be displayed on the web (WebVR). It uses [THREE.js](https://threejs.org/) under the hood, which is a library that lets us create experiences with [WebGL](https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API), a tool for displaying graphics in browsers.

There is a lot to A-Frame, so we're going to be focusing on the basics in this project, and you can continue to experiment with the library on your own to get a feel for what else it can do.

A-Frame uses a declarative superset of HTML tags to construct scenes and experiences. Just like regular HTML, you can change a given tag's (in A-Frame, these are called `entities`) behaviors and appearance by passing information into attributes. You can also write custom JavaScript to create specific behaviors for entities.

Before we get started, here are some terms you should know:

*Scene*: Broadly, the experience you create in an A-Frame project. In the code, it starts with the `<a-scene>` element.

*Entity*: Any of the items in your scene, represented by HTML tags, regardless of whether the items are visible in the scene. In the code, these are represented by primitive shapes (`<a-plane>`, `<a-circle>`, `<a-box>`, etc.) and by `<a-entity>` tags, which you can think of as A-Frame's version of `<div>`s.

*Component*: A set of functionality, written in JavaScript, that can be added to entities by adding the component name and configuration as attributes with semicolon-delimited key-value pairs in their values (`<a-entity geometry="primitive: plane; height: 100; width: 100;"></a-entity>`, for example). A-Frame offers many useful components for us in the core library, but we can also create our own or use components made by other developers.

Open the index.html file in this folder to start with a default scene, which you can modify to your liking. You can see other example scenes on A-Frame's homepage, and you should keep the A-Frame documentation open while you're developing.

Some ideas for quick projects:

1) Change the box color from blue to red.

2) Change the box height, width, and depth to 10.

3) Make sure the box bottom rests on the floor (and not in the floor).

4) Turn the box so that an edge connecting the bottom and top faces is directly in front of you, rather than one of its faces being directly in front of you.

5) Move the box so that it sits at your 3 o'clock when the page loads.

5) Move the box so that it sits at your 9 o'clock when the page loads.

6) Add a purple sphere with a radius of 5 five meters ahead of you at your 12 o'clock. Make sure its bottom rests on the floor.

7) Make the box change color when a cursor hovers over it (and change the color back to the original when the cursor leaves it. (Hint: look up the `a-cursor` element and some mouse events).

8) Create an animation to move the box in a repeating pattern. Look for elements in the documentation that might help you with this.

9) Include the additional [physics package](https://github.com/donmccurdy/aframe-physics-system) and experiment with gravity.

10) Also in the physics package, experiment with collision detection. Either move the box when the player hits it, or prevent the player from moving through the box.

11) Add music to the scene. Experiment with music file placement to see how distance affects the music volume.

12) Create an entity that acts as the "player" with a camera component and add music inside the camera element so it moves with the player.

13) Create a mixin for the box and spawn a new box when a user clicks on a box (use components for the click handler and random placement of the new boxes).

When you're ready to see the product of your work in VR, set up a new project on [Glitch.me]()