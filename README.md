# A Joint Global–Local Network for Human PoseEstimation With Millimeter Wave Radar （IEEE Internet of Things Journal 2022）
![image](https://github.com/Carbord/mmWave-based-Pose-Estimation/blob/main/images/method%20workflow.png?raw=true)
# *Abstract*
This paper proposes a two-branch learning model, namely, the joint global-local network, for human pose estimation using millimeter wave radar. The aim of this work is to remediate the ill-posed problems in human pose estimation arising from using the destructive observations with superimposed reflection signals. In the developed two-branch learning model, the global branch takes use of the superimposed signals from the whole human body to reconstruct the coarse pose estimation from a global perspective, and the local branch is responsible for fining the pose estimations with the decomposed signals from individual body parts in a complementary way. In doing this, two branch learning processes will be coordinated with the followed attention-based fusion module in terms of the local and global consistency. It is remarkable that, the learning driven by the decomposed signals is motivated by exploiting the spatial-temporal evolution patterns of individual body parts for inferring the corresponding movements, which plays a crucial yet complementary role in the collaboration with the learning driven by the superimposed signals. With the two-branch learning architecture, the proposed method is advantageous in incorporating the local motion constraints from individual body parts into the coarse global estimation from the whole human body, which contributes to reconstructing plausible yet accurate pose estimations with the local and global kinematic consistency. Extensive experiments are presented to demonstrate the effectiveness of the proposed method.


# **BibTex**
```
@ARTICLE{9865148,<br>
  author={Cao, Zhongping and Ding, Wen and Chen, Rihui and Zhang, Jianxiong and Guo, Xuemei and Wang, Guoli},<br>
  journal={IEEE Internet of Things Journal}, <br>
  title={A Joint Global-Local Network for Human Pose Estimation with Millimeter Wave Radar}, <br>
  year={2022},<br>
  volume={},<br>
  number={},<br>
  pages={1-1},<br>
  doi={10.1109/JIOT.2022.3201005}}
```
# **Experiment setting**<br>
We collect the radar data, i.e., range-Doppler map(RDM) sequence, from three scernarios and four subjects. 

The pictures and layouts are shown as follows:
![image](https://github.com/Carbord/mmWave-based-Pose-Estimation/blob/main/images/room_layout.png?raw=true)


#  **Data**
In each environment, the subjects, one-at-a-time, performed five different activities, i.e., (i) both arms swing, (ii) lifting legs, (iii) stepping, (iv) raising hands, and (v) boxing. Each activity is collected for 20 s for 10 times.

1. The data are stored in three file folders, in which the hierachy is Scenario/Action/Subject/*.mat (*.npy).

2. The RDM data is stored as the mat file with the shape of 400  * 128 * 128, where 400 means the frame number, 128 * 128 represents the size of one RDM frame. For example, "boxing_1_p1.mat" stands for the 1-th session of the boxing action of subject 1.


3. The skeleton data is stored as the npy file with the shape of 400  * 17 * 3, where a 17-joint human skeleton tree is adopted for human pose esitmation.
![image](https://github.com/Carbord/mmWave-based-Pose-Estimation/blob/main/images/skeleton_tree.png?raw=true)
