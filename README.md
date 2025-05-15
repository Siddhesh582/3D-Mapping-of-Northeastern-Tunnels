# 🌐 3D Mapping of Northeastern University Tunnels

## 🌟 Project Vision
This project aims to transform indoor spatial mapping by automating 3D measurement processes, significantly reducing human error and enabling a scalable approach for disaster management and emergency response.

## 📝 Problem Statement
During natural or man-made disasters, accurate spatial data is crucial for efficient rescue and recovery operations. Traditional manual mapping methods are often time-consuming and prone to errors, while existing technologies may fail in complex, obstructed,  featureless, and repetitive environments. This project addresses these challenges by developing a robotic system capable of generating accurate 3D maps in real-time, aiding rescue teams in navigating damaged or unsafe structures.

![Image](https://github.com/user-attachments/assets/b21579e8-95c9-4556-a323-53333fe224e8)

## 🔧 Hardware Configuration
Ubuntu 20.04 on Lenovo LOQ Laptop: ROS 2 Humble with CUDA Toolkit for GPU acceleration

Stereo Labs ZED Mini: RGB-D camera with integrated IMU for motion tracking

Mounting Setup: Stabilized using a rolling chair/desk to ensure accuracy in smooth and semi-structured environments

## 💻 Software and Methodology
SLAM Framework: RTAB-Map for graph-based SLAM with loop closure detection using Bayesian bag-of-words

Robotic Middleware: ROS 2 for data fusion, odometry calculation, and real-time visualization through RViz 2, Cloud Compare View

ZED SDK: Calibration and depth data streaming

Algorithms Used:

Front-End Processing: Odometry estimation and graph node/edge construction

Back-End Processing: Graph optimization utilizing G2O and TORO for map refinement

Performance Testing: Evaluated handheld vs. stabilized setups in environments with smooth floors (tunnels) and rougher terrains (debris or uneven surfaces)

## Data Files
https://northeastern-my.sharepoint.com/:f:/r/personal/shingate_s_northeastern_edu/Documents/RSN%20Final%20Project%20Data?csf=1&web=1&e=bWzNCz

## 🏆 Key Accomplishments
Enhanced Situational Awareness: Automated 3D mapping provides accurate spatial data in disaster-affected areas

Improved Localization: Loop closure techniques effectively reduced odometric drift in complex environments

Stabilized Mapping: Chair-mounted camera setup improved mapping precision by 60% compared to handheld use

Dynamic Visualization: Real-time map updates allowed rescue teams to monitor progress effectively 📡

## 📈 Performance Metrics
Accuracy:

Stabilized Configuration: Achieved sub-meter alignment with ground truth in tunnel-like structures

Handheld Configuration: Showed drift up to 1.5m in non-linear and obstructed pathways

Optimal Speed: Maintaining a motion speed of less than 0.5 m/s to avoid tracking errors

Stability: Enhanced setup with chair mounting significantly improved accuracy

## 💡 Applications and Use Cases
Disaster Response: Generating 3D maps for navigating collapsed or partially obstructed structures

Search and Rescue: Identifying safe pathways and hazardous zones for rescue operations

Infrastructure Assessment: Creating detailed maps of damaged tunnels or confined spaces

AR/VR Training: Simulating disaster scenarios for emergency response training

## 🚀 Challenges and Future Directions
Challenges Faced:

Repetitive, Featureless Walls: Difficult to distinguish locations, leading to odometric drift.

Terrain Complexity: Glass walls due to reflective and transaprent nature posed a challenge in estimating depth perception and feature extraction, often leading to mapping inconsistencies or sensor errors affecting map quality.

Data Management: Handling large data sets from extended mapping sessions.

## Next Steps:

Enhanced Sensing: Incorporating LiDAR for environments with minimal texture

Real-Time Processing: Integrating with NVIDIA Jetson for on-site mapping

Dynamic Mapping: Improving robustness to environmental changes, such as shifting debris

Mobile Access: Building an app for rescue teams to access real-time maps 📱

## 📌 Conclusion
This project demonstrates the potential of RTAB-Map to generate accurate 3D maps during disaster scenarios, offering a cost-effective and efficient alternative to traditional methods. Its ability to adapt to complex environments and provide real-time visualization makes it a valuable tool for rescue operations, infrastructure assessment, and disaster preparedness.
