# Pentagon Physics Simulator

A realistic 2D physics simulation of colorful balls tumbling inside a slowly rotating pentagon container.

## Features

- **Physics engine**: Powered by [Matter.js](https://brm.io/matter-js/) for accurate rigid-body dynamics
- **Rotating container**: Pentagon walls rotate continuously, shifting gravity's effect relative to the balls
- **Ball collisions**: Balls bounce off walls and each other with restitution, friction, and air drag
- **Interactive controls**: Adjust rotation speed and gravity, add more balls, or reset the scene

## Run locally

Open `index.html` in any modern browser, or serve it with a simple HTTP server:

```bash
python3 -m http.server 8080
```

Then visit [http://localhost:8080](http://localhost:8080).

## Controls

| Control | Description |
|---------|-------------|
| **Rotation** slider | Speed of pentagon rotation |
| **Gravity** slider | Strength of downward gravitational pull |
| **Add Ball** | Drop a new ball at a random position inside |
| **Reset** | Clear and respawn the default ball layout |
