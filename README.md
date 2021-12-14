# animatedLamp
Build a 3D model of a lamp and animate its movement

In this project, first we configured our laptop based on the dedicated card inside the system for rendering purposes. My device had AMD Radeon Graphics card R5 M330 which uses OpenCL to compute the cycles rendering on the model.

Modelling phase:
At first, we made a plane on which the lamp will stand. Then we used Bezier curve and Bezier circles to create the mesh which includes the lamp base and the whole structure of the lamp. In this we use the curve to change the geometry of the mesh. As we were making the model of the lamp, alongside we were joining armatures to the arms of the lamp (armatures act as a bone structure to the model of the lamp which gives a base structure to the lamp). After assigning bones (armatures) to the respective arms of the lamp. Then with the help of constraints, we restricted the motion of these armatures according to the degrees of freedom of the joint. With the help of node editor, material was applied to the different parts of the lamp. The material was either glossy, or diffusive. The lamp also has a light, for this an emissive material was added to the head of the lamp. This was added along with a spotlight lamp. 

Animation Phase:
Through the options panel we applied Auto Inverse Kinematics(IK). This helps in moving the bones together in a motion. The movement depends on the bones present beneath the rigid strucure. For Animation, first, using the timeline, we assigned the poses to the timeframe (called as the ‘key frames’) and using this the animation was progressed. Then using this timeline, movement of camera was also added to make the animation better. Then the animation was rendered and the images after the animation render were saved in a folder and a video is made using the video editor of Blender.

Link to .avi file of rendered motion:
https://drive.google.com/file/d/1Sl5hpwvwmmu1Mge8bXgOr8NoW59IqBsD/view?usp=drive_web

