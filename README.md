# Wrist-Rolling-Motion-Dataset
This repository contains the WRM (Wrist-Rolling Motion) dataset, which includes wrist-rolling motion data collected from users attempting to unlock their mobile phones. The dataset captures the dynamics of wrist movements through three types of sensors: the orientation sensor, the linear acceleration sensor, and the gyroscope sensor. 



## Overview
The WRMR dataset comprises wrist-rolling motion data collected from 20 randomly selected users as they simulate the action of unlocking their mobile phones. Each sample in this dataset includes 8 variables recorded over 50 time steps, providing valuable insights into wrist movement dynamics.

## Dataset Details
### Sensors Used:
Orientation Sensor: Measures the rotation angles across three dimensions.
Linear Acceleration Sensor: Measures acceleration in the absence of gravitational effects.
Gyroscope Sensor: Records the angular velocity of the device.
Variable Exclusion: The X-axis rotation angle is excluded from the dataset since it does not effectively reflect wrist-rolling characteristics during the unlocking action.

### Sampling Rate: 
The sensors collect data at a frequency of 50 Hz, which is then downsampled to 10 Hz for processing.

### Data Processing:
Users are instructed to repeat the wrist-rolling motion multiple times, resulting in samples of varying lengths.
For samples exceeding 50 time steps, data is truncated to maintain consistency.
For samples with fewer than 50 time steps, zeros are padded to meet the required length.
Data segments where the motion has not yet begun are removed to ensure accuracy in motion analysis.
