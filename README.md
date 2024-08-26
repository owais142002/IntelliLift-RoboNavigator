## IntelliLift RoboNavigator (Work in Progress)
An advanced robotics project that integrates a robotic arm mounted on a mobile platform to autonomously detect, navigate towards, and manipulate objects based on natural language commands. This project leverages state-of-the-art technologies in robotics, computer vision, and natural language processing to create a seamless and intelligent system for object handling and navigation.

## Key Features:
- Autonomous Navigation: The robotic car uses ARUCO markers for precise localization and navigation towards specified objects.
- 6D Pose Estimation: The robotic arm employs Gen6D model for accurate pose estimation of objects, enabling precise manipulation.
- Natural Language Command Interpretation: Utilizes Large Language Models (LLMs) to translate verbal commands into actionable JSON data for object identification and task execution.
- Kinematic Modeling: Advanced kinematic and inverse kinematic algorithms ensure smooth and accurate movement of the robotic arm.
- Simulation to Reality Transition: Developed initially in a simulated environment using ROS and Gazebo, the project successfully transitions to real-world applications.

## Technologies Used:
- Robotic Operating System (ROS): For creating a flexible framework that integrates all robotic components and facilitates communication between them.
- Gazebo: A 3D simulation environment for testing and validating the robotic systems before real-world deployment.
- Gen6D Pose Estimation Model: For estimating the 6D pose of objects, crucial for precise manipulation by the robotic arm.
- ARUCO Markers: Used for object identification and localization, providing a reliable method for the robotic car to navigate towards objects.
- Large Language Models (LLMs): For interpreting natural language commands and converting them into machine-executable instructions.
- Kinematic and Inverse Kinematic Modeling: To calculate the required joint angles and movements for the robotic arm to interact with objects accurately.

## Project Workflow:
- Command Input: User provides a verbal command, e.g., "Go grab the Rubik's cube."
- Command Interpretation: LLM translates the command into JSON format: {"object_name":"Rubik's cube"}.
- Object Identification: The system maps the object name to its corresponding ARUCO marker ID.
- Navigation: The robotic car navigates towards the marker ID using computer vision and ARUCO detection.
- Pose Estimation and Manipulation: The robotic arm estimates the 6D pose of the object and lifts it.
- Return and Placement: The robotic car returns to a default position, guided by another ARUCO marker, and the arm places the object.

## Outcome:
The project demonstrates a sophisticated integration of robotics, computer vision, and natural language processing, showcasing the potential for highly automated and intuitive robotic systems in various applications, from warehouse logistics to assistive technologies. This project not only highlights technical prowess in multiple domains but also demonstrates the practical application of these technologies in creating efficient and user-friendly robotic solutions
