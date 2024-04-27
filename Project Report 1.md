# 1. Main steps of SLAM
To achieve visual SLAM, we first need to collect pictures of relevant scenes through the camera, then initialize the map. Then we match the features of the current frame with the features of the last key frame to obtain the estimated pose of the camera. During this process, we need continuously insert new keyframes to prevent tracking loss. Next we need to perform local mapping on each keyframe to continuously update the attributes of the map points observed in each keyframe and then connect all map points observed in these keyframes. Finally, after completing the step of checking loop closure, we compare the optimized camera trajectory with the ground truth to obtain a more accurate camera estimated trajectory.
# 2. Run Step1 Code and its results
After running the code in Step 1, we can get the following results:
![step1.1](https://github.com/haizicao/462-individual-project/blob/417bd3bfb92aefe33e67a025a5e61efbadb63fb1/step1.1.png)
![step1.2](https://github.com/haizicao/462-individual-project/blob/f4bf72b43a92d607ce7b3ae31e1f6806c60af562/step1.2.png)
![step1.3](https://github.com/haizicao/462-individual-project/blob/f4bf72b43a92d607ce7b3ae31e1f6806c60af562/step1.3.png)
![step1.4](https://github.com/haizicao/462-individual-project/blob/f4bf72b43a92d607ce7b3ae31e1f6806c60af562/step1.4.png)
# 3. Self Reflection
By running the above example, I think that to implement visual SLAM, I first need to collect scene data in advance. Then I can use the above code for map initialization and camera trajectory estimation and optimization. In addition, when collecting data, I think using sharp-edged objects may make visual SLAM more successful.
