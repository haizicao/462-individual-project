# 1. Main steps of SLAM
To achieve visual SLAM, we first need to collect pictures of relevant scenes through the camera, then initialize the map. Then we match the features of the current frame with the features of the last key frame to obtain the estimated pose of the camera. During this process, we need continuously insert new keyframes to prevent tracking loss. Next we need to perform local mapping on each keyframe to continuously update the attributes of the map points observed in each keyframe and then connect all map points observed in these keyframes. Finally, after completing the step of checking loop closure, we compare the optimized camera trajectory with the ground truth to obtain a more accurate camera estimated trajectory.
# 2. Run the code and results of Step1
After running the code in Step 1, we can get the following results:
![]()
