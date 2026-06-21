# Rubik's Cube Solver

An interactive Rubik's Cube simulator and solver built with Three.js and browser-side JavaScript. The project renders a fully interactive cube in the browser, supports solving workflows, and includes touch-friendly controls for mobile devices.

## Features

- 3D Rubik's Cube rendered with Three.js.
- Interactive mouse and touch controls for rotating the cube.
- Edit mode for setting face colors before solving.
- Solve workflow with step navigation, play/pause, and reset controls.
- Adjustable cube size and scramble settings through URL query parameters.
- Mobile-aware UI adjustments for smaller screens.

## Controls

- `SOLVE` starts the solving flow.
- `Prev` and `Next` step through the solution.
- `Play/Pause` animates the solution sequence.
- `Reset` reloads the page and restores the current cube state.
- The color palette is used to paint faces in edit mode.

## Project Structure

- `index.html` is the browser entry point.
- `src/environment.js` sets up the scene, camera, renderer, and interactions.
- `src/game.js` contains the cube model and cube-state logic.
- `lib/` contains the runtime libraries used by the app.
- `build/` contains generated browser-ready assets.

## Run Locally

Install dependencies:

```bash
npm install
```

Start a local server:

```bash
npm start
```

The app opens in your browser and should be run from a web server, not directly through Node on `src/*.js` files.

## Notes

- The original project also supports URL parameters such as `order` and `shuffle` to change the cube size and scrambling behavior.
- If you prefer a different static server, open the project folder with any local web server and load `index.html`.
