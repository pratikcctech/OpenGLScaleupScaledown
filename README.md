# OpenGLScaleupScaledown
# Visualizer Project

The Visualizer project is a graphical application that utilizes OpenGL to visualize various geometric shapes and algorithms.

## Features

- **Collision Detection:**
  - Detects collisions between two objects.
  - User inputs coordinates and velocities for both objects.
  - Displays collision points using OpenGL.

- **Bezier Curve:**
  - Generates Bezier curves based on user-provided control points.
  - User inputs control points (x, y) for the Bezier curve.
  - Displays the Bezier curve using OpenGL.

- **Hermite Curve:**
  - Computes Hermite curves using user-provided control points.
  - User inputs control points (x, y) for the Hermite curve.
  - Displays the Hermite curve using OpenGL.

- **B-Spline Curve:**
  - Calculates B-Spline curves based on given control points.
  - User inputs control points (x, y) for the B-Spline curve.
  - Displays the B-Spline curve using OpenGL.

- **Color Palette:**
  - Allows users to select colors for visualization.

- **Scaling:**
  - Supports scaling up and down of visual elements.
  - this is Based on the the runtime Click of button
 
    ```
        connect(pushButton_6, &QPushButton::clicked, this, &Visualizer::scaleUpClicked);
        connect(pushButton_7, &QPushButton::clicked, this, &Visualizer::scaleDownClicked);
  - and the Function code as follows
    ```
      void Visualizer::scaleUpClicked()
      {
          // Access OpenGLWindow and perform scaling up
          if (mRenderer)
          {
              mRenderer->setScaleFactor(0.1); // You can adjust the scaling factor
          }
      }
      void Visualizer::scaleDownClicked()
      {
          // Access OpenGLWindow and perform scaling down
          if (mRenderer)
          {
              mRenderer->setScaleFactor(-0.1); // You can adjust the scaling factor
          }
      }

## Usage

1. Build and run the application using your preferred IDE or build system.

## Dependencies

- Qt: Ensure you have the Qt framework installed.

##Output



https://github.com/pratikcctech/OpenGLScaleupScaledown/assets/149318512/c9c6805a-be98-4ac5-b5da-bc50453aa973



