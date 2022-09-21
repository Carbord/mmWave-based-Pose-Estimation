# The dataset for mmWave-based human pose estimation will be released soon !

# **Experiment setting**<br>
We collect the radar data, i.e., range-Doppler map(RDM) sequence, from three scernarios. The pictures and layouts are shown as follows:

![image](https://github.com/Carbord/mmWave-based-Pose-Estimation/blob/main/images/room_layout.png)


#  **Data**
1. The data are stored in three file folders, in whihc the hierachy is Scenario/Action/Subject/*.mat (*.npy).

2. The RDM data is stored as the mat file with the shape of 400  * 128 * 128, where 400 means the frame number, 128 * 128 represents the size of one RDM frame. For example, "boxing_1_p1.mat" stands for the 1-th collection of the boxing action of subject 1.


3.The skeleton data is stored as the npy file.
