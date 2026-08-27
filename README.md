# GH360
All documentation around the GH360 robot.

# Joint Configuration Application
A MATLAB application was created to reliably set up a joint on the GH360 robot. The process consists of three steps: defining a joint in the app using the CAD model, manufacturing the tendons, and mounting the tendons on the joint with the correct pulley configuration.

## Defining a Joint in the App
Defining a joint in the app requires a CAD model of the robot. The main page of the app, allows the user to select and edit a joint. Because each joint has two active pulleys, both the right and left joint sides must be defined. A drop-down menu allows the user to swap between the two. In the edit menu, the user can define important parameters such as the radius of the active and passive pulleys and tendon diameter. Additionally the center of the active and passive pulley as well as the tendon attachment positions have to be defined. These can be simply obtained from the CAD model. The location of the frame of reference is not important as long as all positions are in the same reference frame. While the locations are in 3D, one axis should approximately be aligned. To transform it into a 2D problem, the used can select which axis of the reference frame is mapped into x and y in the 2D coordinate system. By pressing **Save**, the defined parameters are stored. After the parameters are saved, the user returns to the main page. Here, the user can calculate the tendon lengths using the **Show Tendon Lengths** button. After which the **Show Pulley Config** button becomes available, which when pressed calculates the pulley configuration. Finally, a **Create Sim Config File** button gives the user the possibility to generate the configuration file used by the simulated equilibrium controller.

## Manufacturing Tendons
Both filament and sleeve lengths are required to manufacture the tendon. The tendon lengths are calculated by pressing **Show Tendon Lengths** on the main page. Subsequently, the **Show Pulley Config** becomes available, which can be used to obtain an overview page that shows the user which tendon is connected to the inner and which is connected to the outer pulley. To obtain the measurements required for manufacturing the two tendons, the user can press the **Manufacturing Help** button. The **Manufacturing Help** page, shows the lengths at which both the inner filament and sleeve are supposed to be cut. To assemble the tendon, the sleeve is simply slid over the filament and clamped at both ends.

## Mounting and Configuring Tendons on the Joints
After the tendons have been manufactured and connected to the corresponding active and passive pulleys, the inner and outer active pulleys can be mounted on the motor. First, the motor should be moved to 0 rad position. Then, the inner active pulley is taken and screwed onto the motor plate in the configuration shown on the **Pulley Config** page. The blue and red lines visualize the tendons and show the user how many rotations the tendon must be wrapped around the pulley.


