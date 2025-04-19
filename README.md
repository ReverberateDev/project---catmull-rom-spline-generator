# Catmull-Rom Spline Generator

This project is a C++ implementation of a Catmull-Rom spline generator. It visualizes a 2D grid where splines are generated based on control points. Users can interactively modify control points using keyboard inputs.

## Features
- Smooth Catmull-Rom spline generation.
- 2D grid visualization of splines and control points.
- Real-time control point manipulation via keyboard.
- Supports looped and non-looped splines.

## How It Works
1. Control points are predefined or input by the user.
2. The `CreateSpline` function calculates intermediate points using the Catmull-Rom spline algorithm.
3. Control points and spline points are mapped to a 2D grid.
4. Users can modify control points interactively.

## Keyboard Controls
- **Arrow Keys**:
    - **UP**: Move the current control point up.
    - **DOWN**: Move the current control point down.
    - **LEFT**: Move the current control point left.
    - **RIGHT**: Move the current control point right.
- **BACKSPACE**: Switch to the previous control point.
- **ESCAPE**: Exit the program.

## How to Run
1. Compile the program:
     ```bash
     g++ -o catmull_romspline catmull_romspline.cpp
     ```
2. Run the program:
     ```bash
     ./catmull_romspline
     ```

## Example Output
The program outputs a grid where:
- `C` marks control points.
- `0` marks spline points.
- `?` marks the currently selected control point.

Example:
```
. . . . . . . . . . . . . C . . . . . . . .
. . . . . . . . . . . . . 0 0 ? . . . . . .
. . . . . . . . . . . . . . . . . . . . . .
```
Pressing **[Backspace]** will shift `?` to `C`.

## Future Improvements
- Add mouse-based control point manipulation.
- Improve visualization with colors or a graphical interface.
- Optimize for larger grids or more control points.

## License
This project is open-source under the MIT License.
This project is a C++ implementation of a Catmull-Rom spline generator. It visualizes a 2D grid where splines are generated based on control points. Users can interactively modify control points using keyboard inputs.

Features
Smooth Catmull-Rom spline generation.
2D grid visualization of splines and control points.
Real-time control point manipulation via keyboard.
Supports looped and non-looped splines.
How It Works
Control points are predefined or input by the user.
The CreateSpline function calculates intermediate points using the Catmull-Rom spline algorithm.
Control points and spline points are mapped to a 2D grid.
Users can modify control points interactively.
Keyboard Controls
Arrow Keys:
UP: Move the current control point up.
DOWN: Move the current control point down.
LEFT: Move the current control point left.
RIGHT: Move the current control point right.
BACKSPACE: Switch to the previous control point.
ESCAPE: Exit the program.
How to Run
Compile the program: g++ -o catmull_romspline catmull_romspline.cpp
Run the program: ./catmull_romspline
Example Output
The program outputs a grid where:

C marks control points.
0 marks spline points.
? marks the currently selected control point.
Example: . . . . . . . . . . . . . C . . . . . . . . 0 0 ? . . . . . . . . . . . . .
Pressing [Backspace] will shift ? to c

Future Improvements
Add mouse-based control point manipulation.
Improve visualization with colors or a graphical interface.
Optimize for larger grids or more control points.
License
This project is open-source under the MIT License.