
# Lane Detection for Structured Curved Roads

This project focuses on the lane detection aspect of an autonomous vehicle using camera as a sensor.Data collected is processed using python,implemented using transformer based process.




## Table Of Contents

1. Introduction
2. Algorithm
3. Data Collection
4. Installation
5. Results
6. Contributing
7. License
8. Acknowledgements
## Introduction

Lane Detection is essential for autonomous vehicles.This project aims to provide the direction to the driver so that the vehicle stays within a designating line,thereby reducing the risk of accidents.This study explores a transformer based lane detection technique to address the challenges particularly in the context of structured curved roads.
## Algoithm

The Transformer based detection technique is used for lane detection in curved roads.The following steps outline the process implemented in this project:

1. The input image is passed through CNN backbone where feature map is extracted.

2. It is then passed to the encoder which takes feature sequence as input and extracts the most relevant features and passes to the decoder.

3. In decoder,lane query sequence(S) and encoder output feature sequence as input and undergoes cross attention to output lane features.

4. These are then passed through the MLP to produce vertical ranges and object scores.

5. Display the results .
## Dataset

CurveLanes dataset is taken for our project.

The Dataset is about 76GB after compression. We split the whole rar file into 6 parts each has about 13GB. We provide download link from Google Drive and Baidu Pan to facilate users from all over the world.

CurveLanes.part1.rar

https://drive.google.com/open?id=1nTB2Cdyd0cY3nVB1rZ6Z00YjhKLvzIqr

Link: https://pan.baidu.com/s/1-nmUOCrU0twBZtOe_neuLw Extraction code: m67c

CurveLanes.part2.rar

https://drive.google.com/open?id=1iv-2Z9B6cfncogRhFPHKqNlt-u7hQnZd

Link: https://pan.baidu.com/s/1YrLK9tm7jRpgwaIDOzUplA Extraction code: 8adg

CurveLanes.part3.rar

https://drive.google.com/open?id=1n2sFDdy2KAaw-7siO7HWuwxUeVb6SXfN

Link: https://pan.baidu.com/s/10UTTRkgk5dDPXJZBQT4jAg Extraction code: ur4e

CurveLanes.part4.rar

https://drive.google.com/open?id=1xiz2oD4A0rlt3TGFdz5uzU1s-a0SbsX8

Link: https://pan.baidu.com/s/1b-dShapx3Q0SyYqdhzujxQ Extraction code: ognl

CurveLanes.part5.rar

https://drive.google.com/open?id=1vpFSytqlsJA-rzfuY2lyXmZvEKpaovjX

Link: https://pan.baidu.com/s/18wvCPNaQHiJmQ0YeNJOYsA Extraction code: i6r8

CurveLanes.part6.rar

https://drive.google.com/open?id=1NZLvaBWj0Mnuo07bxKT7shxqi9upSegJ

Link: https://pan.baidu.com/s/1nqQ-uPnsDzQs3T35yhQqDw Extraction code: 9q0y
## Installation

1. Install Vs code and ensure necessary tools are installed.
2. Ensure that the python environment is created.

## Usuages

1. Load the Dataset in the python environment
2. Check the following installations are available in the python environment or not
   Create python environment:
conda create -n hdmapnet python=3.10
conda activate hdmapnet
Install pytorch (>=2.0.0):
pip install torch torchvision torchaudio torchdata
Install mmcv (>=2.0.0):
pip install -U openmim
mim install mmcv
Install requirements:
pip install -r requirements.txt
Install cuda11.7 (add to your ~/.bashrc and then source ~/.bashrc)
export CUDA_HOME=/usr/local/cuda-11
export PATH=$PATH:$CUDA_HOME/bin
export LD_LIBRARY_PATH=/usr/local/cuda/lib64${LD_LIBRARY_PATH:+:${LD_LIBRARY_PATH}}

    
## Results

The result demonstrates the effectiveness in detecting the lane lines . Below are the example images showing the performance of the algorithm.

![Screenshot (1286)](https://github.com/user-attachments/assets/cea3c3b5-5746-4407-a4d9-b1d7aac7ccef)

## Contributing

Contributions are always welcome! Please open an issur or submit a pull request.


## License

This project is licensed under the MIT License-see the license file or details


## Acknowledgements

Special thanks to [Prof.Giressha.H.M,Shreyas Mutnal,Harshita Gokavi,Harshit Koliwad,KLE Technological University] for their support and contributions to this project.


