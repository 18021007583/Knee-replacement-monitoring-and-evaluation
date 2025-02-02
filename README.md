# Knee-replacement-monitoring-and-evaluation

# Wearable inertial measurement unit（IMU）
The activity data is acquired by two wearable IMUs mounted on the thigh and shank, as shown in Fig. 1. The IMU consists of an STM32F407 microcontroller, an MPU9250 accelerometer and gyroscope module, an Arduino Bluetooth module and a lithium battery (300 mAh). The size of the sensor node is 56.5×37.5×15.5 mm3, weighs 30 g, and the sampling frequency is 100 Hz. The range of accelerometer and gyroscope are ±156.5 m/s2 (16g) and ±34.9 rad/s (2000°/s), respectively. During data collection, the two sensor nodes are kept on the sagittal plane of the thigh and the shank.

# Rehabilitation assessment equipment
Baltimore Therapeutic Equipment (BTE) Primus RS is an advanced equipment integrating assessment, rehabilitation and training. In this experiment, BTE Primus RS is used as the standard for evaluating the knee ROM of patients. During the swing of the robotic arm, the angular velocity of the equipment can be manually adjusted to meet the needs of different subjects. The patient's shank is tied to the arm of BTE Primus RS, and the thigh is fixed on the chair so that accurate ROM could be recorded (Fig. 1). Generally speaking, the smaller the difference between the estimated ROM and BTE Primus RS, the higher the accuracy of the proposed sensor system.


# Experimental data collection
In order to achieve accurate monitoring and evaluation during the rehabilitation of TKR patients, we have constructed a systematic experimental scheme to collect substantial clinical data. Experimental items include active and passive knee flexion-extension, gait activities, etc. Before data acquisition, the patients will be instructed and tested accordingly, and the BTE Primus RS equipment will be operated by a professional physical therapist. The detailed experimental procedure is described as follows (Fig. 2).
 
1) Passive Flexion-extension: Participants wear sensor IMUs, and then ask to perform a flexion experiment driven by BTE Primus RS, as shown in Fig. 2 (a). Considering the potential safety hazards for patients, three angular velocities are set at 15°/s, 30°/s and 45°/s, rather than larger speeds. The test is repeated twice for each angular velocity, and the duration of each time is 30s. The initial and final position of the flexion will be set, depending on the patient's tolerance. In order to ensure uniformity, all experiments of healthy adults are consistent with patients.
2) Active Flexion-extension: Participants are required to lie flat on the bed with their arms under the head. Then slide one foot along the plane of the bed, from the far end to the proximal end, until it is unable to bend or painful, as shown in Fig. 2 (b). The flexion-extension activities (twice on left and right side, respectively) are repeated 3 times for each group of experiments.
3) Gait flexion-extension: This test requires participants to walk 10 meters in a straight line, maintaining their own rhythm. During the whole walking, the patients are uniformly asked to use a walking aid to prevent falls, as shown in Fig. 2 (c). The gait activities are repeated twice for each participant.

# Original data description
The format of the original flexion-extension activity data is .bsn, which can be read and processed through the BSN_demo.m code. The original nine-axis sensor data will be obtained, including three-axis acceleration, gyroscope and magnetometer signals.
