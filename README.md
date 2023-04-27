
# Eye Movement 👁️

This project utilizes JavaScript and CSS to create an interactive animation that tracks the user's mouse cursor movement on the screen by simulating the movement of a pair of eyes. The animation demonstrates the manipulation of the Document Object Model to alter the position of HTML elements.


## Table of Contents
1. [Concepts](#concepts)
2. [How It Works](#how-it-works)
3. [Run Locally](#run-locally)
4. [Roadmap](#roadmap)
5. [License](#license)
## Concepts

- **DOM manipulation:** The document.getElementsByClassName() method is used to select all elements with the class name 'ball'.
- **Handling user interactions:** The document.onmousemove event is used to track the user's mouse movements and update the position of the eyeballs accordingly.
- **Element positioning:** The style.left, style.top, and style.transform properties are used to position the eyeballs relative to the mouse cursor.


## How It Works
- The HTML file has two elements with the class 'ball', representing the eyeballs. These elements are selected using document.getElementsByClassName() and stored in the balls variable.

- The document.onmousemove event listener is set up to update the position of the eyeballs when the user moves their mouse. The event object contains the clientX and clientY properties, representing the mouse cursor's X and Y coordinates, respectively.

- The x and y variables are calculated by dividing the cursor's X and Y coordinates by the window's width and height, respectively. This normalizes the position of the cursor and scales it between 0 and 100.

- In the loop, which iterates twice for the two eyeballs, the position of each eyeball is updated using the style.left, style.top, and style.transform properties. The style.left and style.top properties set the horizontal and vertical positions of the eyeballs, while the style.transform property applies a translation based on the cursor's position.

- The result is a pair of eyeballs that smoothly follow the user's mouse movements, creating an engaging and interactive animation. This project showcases how to use vanilla JavaScript and CSS to manipulate elements on a webpage and create simple animations.


- balls is a collection of DOM elements with the class name 'ball', representing the eyes.

- document.onmousemove is an event listener that listens for the mousemove event to track the cursor's position.

- document.onmousemove = (event) => { ... }: This event listener is triggered whenever the mouse is moved. It calculates the relative position of the cursor on the screen and updates the position of the eye elements accordingly.

The application starts by getting the DOM elements representing the eyes. When the mousemove event is triggered, the event listener calculates the relative position of the cursor on the screen (in percentage) and updates the positions of the eyes. The for loop iterates through the eye elements, updating their positions based on the calculated cursor position. The eyes follow the cursor as it moves around the screen, creating a dynamic animation.

## Run Locally

Click the green Code button and download the zip file. Click on the index.html file and view the interactive application in your browser. 

## Roadmap

- Change the blue background to a flesh tone and make the eyes bloodshot.


## License

[MIT](https://choosealicense.com/licenses/mit/)

