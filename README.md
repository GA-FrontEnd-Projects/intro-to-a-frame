# Intro to A-Frame

[A-Frame](https://aframe.io/) is a powerful tool for creating virtual reality experiences to be displayed on the web (WebVR). It uses [THREE.js](https://threejs.org/) under the hood, which is a library that lets us create experiences with [WebGL](https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API), a tool for displaying graphics in browsers.

There is a lot to A-Frame, so we're going to be focusing on the basics in this project, and you can continue to experiment with the library on your own to get a feel for what else it can do.

## What is it?
A-Frame is a JavaScript/HTML framework built on top of THREE.js that makes it easy to create 3D and VR experiences that run in regular web browsers. Just like regular HTML, you can change a given tag's (in A-Frame, tags are called `entities`) behaviors and appearance by passing information into attributes. You can also write custom JavaScript to create specific behaviors for entities.

## Why is it cool?
There has been a big push on VR over the past few years, mostly with headset-based experiences. If you've tried any of the popular experiences, you'll know that they're incredible, but they still face a number of problems. The headsets and computers that are needed to run these experiences are expensive, the experiences don't always work on every headset, content is expensive to create, and the audience who can see a given experience is limited to people who can afford the expensive headsets and computers. WebVR (which A-Frame creates) solves a lot of these problems.

Most personal computers these days have the power to run decent VR experiences. If you have an up-to-date, major browser, you shouldn't run into too much trouble. It's also much easier to create an experience for WebVR -- the skills required to create experiences are just about the same as what's required to build a webpage. Since content is accessible via the web, the potential audience is huge. WebVR also works on (and is sometimes better on) mobile devices, either through a standard browser view or by using a Cardboard.


## Important terms to know
Before we get started experimenting with A-Frame, here are some terms you should know:

*Scene*: The experience you create in an A-Frame project. In the code, it starts with the `<a-scene>` element.

*Entity*: Any of the items in your scene, represented by HTML tags, regardless of whether the items are visible in the scene. In the code, these are represented by primitive shapes (`<a-plane>`, `<a-circle>`, `<a-box>`, etc.) and by `<a-entity>` tags, which you can think of as A-Frame's version of `<div>`s.

*Component*: A set of functionality, written in JavaScript, that can be added to entities by adding HTML attributes with semicolon-delimited key-value pairs in their values (`<a-entity geometry="primitive: plane; height: 100; width: 100;"></a-entity>`, for example). A-Frame offers many useful components for us in the core library, but we can also create our own or use components made by other developers.

## Time to code
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

11) Add music to the scene. Experiment with adding music to different entities in the scene to see how distance can affect music volume.

12) Create an entity that acts as the "player" with a camera component and add music inside the camera element so it moves with the player.

13) Create a mixin for the box and spawn a new box when a user clicks on a box (use components for the click handler and random placement of the new boxes).

When you're ready to see the product of your work in VR, set up a new project on [Glitch.me]()