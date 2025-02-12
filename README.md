# Robotics Projects Showcase
The aim of this repository is to highlight my proficiency and expertise in robotics by compiling some of my most notable projects in the field. \
The following projects represent my own work and, in some cases, involve collaborative efforts. For detailed insights into individual contributions, please refer to the specific repository. \
These projects have allowed me to delve into various aspects of robotics, encompassing pure control theory [1, 2] and the application of probabilistic algorithms [3, 7]. Among these endeavors, the ones I found most enjoyable were [4, 5], where I had the pleasure of collaborating with close friends in France and individuals from diverse backgrounds whom I met during my time in beautiful Japan.

## 1) Model-free Control Barrier Functions for obstacle avoidance

- **Repository:** [GitHub Link](https://github.com/DennisRotondi/AMR22_FP8_Model_free_CBF)
- **Year:** 2023
- **Programming Language:** MATLAB
- **Additional Resources:** [Report](https://github.com/DennisRotondi/AMR22_FP8_Model_free_CBF/blob/master/report.pdf), [Slides](https://docs.google.com/presentation/d/1cNUM1Hq5WOP4jOX6p8fWa-TL-2o4LwJ9hxVOweNTL3Q/edit?usp=sharing), [Video](https://drive.google.com/drive/folders/1BrxUTx0JuhWMO_hbAV8zvJXK9wSYaCpP?usp=sharing)

### Description

This project is the result of the final work for the exam [Autonomous Mobile and Robotics (AMR)](https://www.diag.uniroma1.it/oriolo/amr/) WS 2022/23, taught by Professor [Giuseppe Oriolo](https://www.diag.uniroma1.it/oriolo/) at Sapienza University of Rome. 
It revolves around Control Barrier Functions (CBFs). A CBF is a mathematical function that represents a safety constraint. It is designed to ensure that the system stays within safe operating bounds or avoids unsafe states while achieving its control objectives (e.g. regulation). Our goal has been to implement the CBFs by exploiting the full knowledge of the robot dynamic model, and using only the kinematic one (also called the Model-Free approach due to the much simpler equations). The simulations (cf. additional resources) have been carried out using a point robot and a unicycle, highlighting the pros and cons of each approach.

## 2) Gravity learning for elastic joint robots

- **Repository:** [GitHub Link](https://github.com/DennisRotondi/robotics2_project)
- **Year:** 2022
- **Programming Language:** MATLAB
- **Additional Resources:** [Report](https://github.com/DennisRotondi/robotics2_project/blob/master/Report_Rotondi_Scaparro.pdf), [Slides](https://docs.google.com/presentation/d/165GUNOE-dIQUmgw-vLpszNcTZbrL-P3V7CobsmjXhgE/edit?usp=sharing), [Video](https://drive.google.com/drive/folders/1DCEF3msvgXbq4hISgg4q9fJZa7GfT--3?usp=sharing)

### Description

This project is the result of the final work for the exam [Robotics 2](https://www.diag.uniroma1.it/deluca/rob2_en.php) SS 2021/2022, taught by Professor [Alessandro De Luca](https://www.diag.uniroma1.it/deluca/) at Sapienza University of Rome. 
Here, we delve into the modeling of elastic joint robots, a specific category that is gaining increasing popularity, with its most extreme manifestation being soft robots. Designing a PD controller for such robots is non-trivial, and in this project, we explore and demonstrate how it is feasible to regulate the position of the end effector using an iterative gravity learning compensation term. The simulations (cf. additional resources) are conducted using a 3R elastic joint robot.

## 3) 2D Range Only SLAM

- **Repository:** [GitHub Link](https://github.com/DennisRotondi/probabilistic_robotics_project)
- **Year:** 2022
- **Programming Language:** Octave

### Description

This project is the result of the final work for the exam [Probabilistic Robotics](https://sites.google.com/diag.uniroma1.it/probabilistic-robotics-2021-22/home) SS 2021/2022, taught by Professor [Giorgio Grisetti](https://sites.google.com/dis.uniroma1.it/grisetti/home) at Sapienza University of Rome. Here, I have implemented backend optimization for the Simultaneous Localization and Mapping (SLAM) problem using only odometry and range measurements (distance from landmarks). Additionally, the difference between performing SLAM with this sensor fusion and working independently with only range measurements is explored.

## 4) RoboCup Autonomous Robot Manipulation Challenge 2023

- **Repository:** [GitHub Link](https://github.com/DennisRotondi/arm_2023), [HRI Extension](https://github.com/DennisRotondi/eai_hri_project)
- **Year:** 2023
- **Programming Language:** MATLAB
- **Additional Resources:** [Report](https://github.com/DennisRotondi/eai_hri_project/blob/master/report.pdf), [Video](https://drive.google.com/file/d/1aAxM02qK1T6J0tL3uSaWgUbBY04pCLik/view)

### Description

This project is the solution proposed by the Italian team to compete against all the other countries in the RoboCup Autonomous Robot Manipulation Challenge 2023 world finals in Bordeaux, France. Participants were tasked with completing a recycling task with a robot manipulator in a dynamic environment. Our approach involves perception neural networks (YOLO) to identify the objects in the environment. The bounding boxes are then reprojected into the 3D world, and through 3D point matching techniques (iterative Closest Point algorithm), we estimated the positions of the objects to compute the optimal grasping direction. The robot has been moved by an impedance controller to guarantee safety. The challenge code has been extended and adapted with an interactive unconstrained language module to be considered as the final project for the exam [Human-Robot Interaction](https://sites.google.com/a/dis.uniroma1.it/human-robot-interaction/) SS 2022/2023, taught by Professor [Luca Iocchi](https://sites.google.com/a/dis.uniroma1.it/iocchi/home) at Sapienza University of Rome.

## 5) The Lego Lunar Rover

- **Repository:** [GitHub Link](https://github.com/DennisRotondi/TESP-2023-SRL)
- **Year:** 2023
- **Programming Language:** Python, JavaScript
- **Additional Resources:** [Slides](https://docs.google.com/presentation/d/1brLksOLnWhpN5oyCPqFwvuAbko7c9YVF80kQ7MEr1qA/edit?usp=sharing), [Video](https://drive.google.com/file/d/1Q4VsljjR6gzpzra17ERn7jukDuctEdYL/view?usp=sharing)

### Description

This project is the outcome of the [Tohoku University Engineering Summer Program (TESP)](http://www.astro.mech.tohoku.ac.jp/TESP/) Robotics 2023 under the supervision of Professor [Kazuya Yoshida](https://www.eng.tohoku.ac.jp/driving_force/english/vol1-1.html). The primary objective was to develop a rover-like robot from scratch with mobility in sandy environments, capable of teleoperation with an obstacle avoidance module. 
A Raspberry Pi 4 served as the main computer, running ROS on Ubuntu 20.04 and connecting to the LEGO Mindstorms EV3 to drive the servo motors installed in the LEGO structure
As a depth sensor, an Intel RealSense Depth Camera D435 was employed. The robot incorporates a YOLO v7-tiny architecture for identifying obstacles and implementing avoidance strategies.

## 6) Web-Based Client for Pick and Delivery Robotics Tasks

- **Repository:** [GitHub Link](https://github.com/DennisRotondi/progetto_labiagi)
- **Year:** 2021
- **Programming Language:** C++, JavaScript
- **Additional Resources:** [Video](https://www.youtube.com/watch?v=a57-CVdI46s)

### Description

This project is the result of the final work for the exam [Laboratorio di Intelligenza Artificiale e Grafica Interattiva (LABIAGI)](https://sites.google.com/diag.uniroma1.it/labiagi-2020-21/home) SS 2020/21, taught by Professor [Giorgio Grisetti](https://sites.google.com/dis.uniroma1.it/grisetti/home) at Sapienza University of Rome.
It allows to configure a client interface to notify the robot of new objectives, causing it to move in a pre-set navigation environment. From the web interface, anyone can "log in" (specifically, an ID sender is created, which will then be used on the ROS node server to determine who can actually maneuver the robot and who can only confirm deliveries). The server communicates with the client through the exchange of ROS messages, using roslibjs + rosbridge. The robot distinguishes commands from "authorized" users and "guests"; the latter can only confirm arrival, and once they do, the robot will be available again to receive direction commands from authorized users. If a user of this type confirms arrival, the next position command can only be given by that user, allowing them enough time to pick up the package and potentially put another one on top. The software has been tested with the [SRRG2 robotics navigation suite](https://gitlab.com/grisetti/labiagi_2020_21/-/tree/master/workspaces/srrg2_labiagi/src?ref_type=heads).

## 7) Laser Matcher

- **Repository:** [GitHub Link](https://github.com/DennisRotondi/rp_project)
- **Year:** 2021
- **Programming Language:** C++

### Description

This project is the result of the final work for the exam [Robot Programming](https://sites.google.com/diag.uniroma1.it/robot-programming-2023-24/home) WS 2021/22, taught by Professor [Giorgio Grisetti](https://sites.google.com/dis.uniroma1.it/grisetti/home) at Sapienza University of Rome.
It consists of a ROS node that subscribes to "/base_scan". From there, starting with the known position of the robot, it will use LaserScan messages obtained through this subscription to correct the position of odom->base_link given by the node that deals with low-level encoders. The result is an updated map->odom tf and the estimated pose2D advertised in the ROS environment. This is efficiently achieved by matching scans through the Iterative Closest Point (ICP) algorithm.
