# Educational Colab-based implementation of SLAM Book 2
**slambook2 and running its codes in Google Colab**


This repository provides an educational and reproducible implementation of selected examples from
**“Visual SLAM: From Theory to Practice ([slambook2](https://github.com/gaoxiang12/slambook2))” by Gao et al.**, adapted to run in Google Colab.


The purpose of this project is not to present a novel or state-of-the-art SLAM system.
Instead, it serves as **a structured learning notebook** to consolidate my understanding of Visual SLAM,
while offering a beginner-friendly tutorial aligned with the reference book.

Several public repositories already provide implementations of SLAM Book examples.
The contribution of this repository lies in the following aspects:

*   Presenting the material as a **step-by-step educational tutorial**, closely following the book.

*   Making the examples **executable in Google Colab**, including environment setup and dependency handling.

*   Providing **additional explanations, notes, and references** to clarify the algorithms and implementation details.

*   Emphasizing **C++ implementations**, CMake-based builds, and practical issues arising when running C++ SLAM code in Colab.

*   Gradually extending the material with **related algorithms, tools, and applied examples**.

⚠️ Due to the Colab environment and the original C++ codebase, some examples require adaptation and may remain partially incomplete. These limitations are documented explicitly in the notebooks.


## **Repository Structure and Content**

The notebooks are organized mainly following the chapter order of the reference book, with additional sections for tools, algorithms, and applied topics.


**Covered Topics**  
* **Chapter 1**	<ins>Introduction to SLAM</ins>
  
* **Chapter 2**	<ins>3D Rigid Body Motion</ins>

  Rigid body geometry in 3D space: rotation matrices, transformation matrices, quaternions, and Euler angles.
  
  Practical use of the Eigen library for matrix and geometry operations.  

* **Chapter 3**	<ins>Lie Group and Lie Algebra</ins>
  
  Concepts of Lie groups and Lie algebras, focusing on SO(3) and SE(3).
  
  Baker–Campbell–Hausdorff (BCH) formula and practical use of Sophus.  

* **Chapter 4**	<ins>Cameras and Images</ins>
  
  Projection of 3D points onto image planes and camera models.
   
* **Chapter 5**	<ins>Nonlinear Optimization</ins>  
  Formulating batch state estimation as a least-squares problem.
  
  Solving nonlinear optimization using Ceres and g2o.  

* **Chapter 6 & 7**	<ins>Visual Odometry</ins>  
  Feature extraction and matching.
  
  Epipolar geometry and motion recovery.
  
  PnP problem.
  
  ICP and point cloud alignment.
  
  Triangulation and optical flow.
  
  Direct methods and g2o-based implementations.   
* **Chapter 8 & 9**	<ins>Filters and Optimization</ins>  
  Backend formulation as filtering or least-squares optimization.
  
  Sparse bundle adjustment.
  
  Sliding window optimization and pose graph optimization 

  using g2o and Ceres.  
* **Chapter 10**	<ins>Loop Closure</ins>  
  Role of loop closure in SLAM and related tools.  
* **Chapter 11**	<ins>Dense Reconstruction</ins>  
  Dense depth estimation in monocular SLAM.
  
  RGB-D reconstruction, obstacle avoidance, navigation, and interaction.

  Mapping as a core SLAM objective.   

* **Chapter 12**	<ins>Practice: Stereo Visual Odometry</ins>  
  A simplified stereo VO pipeline evaluated on the KITTI dataset, focusing on practical challenges such as scale drift and tracking robustness.
