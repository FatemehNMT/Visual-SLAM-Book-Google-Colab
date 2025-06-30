# Visual-SLAM-Book-in-Google-Colab
**slambook2 and running its codes in Google Colab**

This is not a novel, unique, state-of-the-art project. It is in fact, a notebook for me, to gather my knowledge on Visual-SLAM in a pack, or a basic tutorial for a beginner in this field, according to [slambook2](https://github.com/gaoxiang12/slambook2), with more explaination of codes and more related examples.

There are many GitHub accounts providing these codes in similar or different ways and versions. In fact, there is no significant difference here in presenting them, except for trying to:  
+	Introduce the subject as a basic tutorial, considering the book itself.
+	Install, run and present everything in Colab-Notebooks (although, there are some problems attached to its applying there (more specifically, when the main source is in C++)).
+	Provide more related information, algorithms and introduce some useful links and examples.
+	Focusing on C++ language and applying CMake, while running some of the examples may be challenging.

The information will be gathered in my notebook in chapters mainly following the reference book's order; moreover, there are other sections on applied tools and their main applications, introduced algorithms and their usage's goals, and extra related topics.  

**In summary, chapters of the book contain:**  
* **Chapter 1**	<ins>Introduction to SLAM</ins>  
* **Chapter 2**	<ins>3D Rigid Body Motion</ins>
  Study the rigid body geometry in three-dimensional space: rotation matrix, transformation matrix, quaternion, and Euler angle.
  Applying the Eigen library’s matrix and geometry module.  
* **Chapter 3**	<ins>Lie Group and Lie Algebra</ins>  
  The concept of Lie group, Lie algebra, and their applications of SO(3), SE(3) and the corresponding Lie algebras.  
The meaning and usage of the BCH (Baker-Campbell-Hausdorff) formula.  
Applying Sophus to perform operations on Lie algebras.  
* **Chapter 4**	<ins>Cameras and Images</ins>  
  projecting a spatial point into image planes.  
* **Chapter 5**	<ins>Nonlinear Optimization</ins>  
  Forming the batch state estimation problem into a least-square and solving the least-square problem.  
Applying the Google Ceres and g2o library to solve a least-square problem.  
* **Chapter 6 & 7**	<ins>Visual Odometry</ins>  
  Study how to extract feature points from images and match feature points in multiple images.  
Learn the principle of epipolar geometry and use epipolar constraints to recover the camera’s 3D motion between two images.  
Study how to solve the PNP problem and use the known correspondence between the 3D structure and the 2D image to solve the camera’s 3D motion.  
Study the ICP algorithm and use the point clouds matching to estimate 3D motion.  
Study how to obtain the 3D structure of corresponding points on the 2D image through triangulation. Study the principle of optical flow.  
Learn how to use the direct method to estimate the camera pose.  
Use g2o to implement the direct method.   
* **Chapter 8 & 9**	<ins>Filters and Optimization</ins>  
  Formulate the backend problem into a filter or least-square optimization problem.  
Using the sparse structure in the bundle adjustment problem.  
Solve a BA problem with g2o and Ceres.  
Learning principles of sliding window optimization and basic knowledge about pose graph optimization. 
Pose graph optimization with g2o.  
* **Chapter 10**	<ins>Loop Closure</ins>  
  The role of loop closure in SLAM and applying tools to manage it.  
* **Chapter 11**	<ins>Dense Reconstruction</ins>  
  Estimating and implementing the dense depth in monocular SLAM, and some of the commonly used map forms in RGB-D reconstruction. Obstacle avoidance, navigation and reconstruction are the main applications of dense map.  
Introducing the algorithm of the mapping, as one of the two goals of SLAM. We hope that the map can be used for localization, navigation, obstacle avoidance, and interaction.   
* **Chapter 12**	<ins>Practice: Stereo Visual Odometry</ins>  
Focusing on problems due to VO (such as continuously tracking the image or controlling the scale of BA) and methods of handling them.  
A simplified version of VO is implemented and its running effects is estimated in the Kitti dataset. 
