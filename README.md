# Gesture Recognition Case study IIITB Assignment ![](https://img.shields.io/badge/Vaidehi-SureshKrishna-brightgreen.svg?colorB=ff0000)
>Identify gesture in smart tv can make hassel free operation which increases the value of product .It is also a marketing strategy to stand against competitor.
>This project is about identifying 5 such common gesture that can be used on videos.
## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
- Data available https://drive.google.com/uc?id=1ehyrYBQ5rbQQe6yL4XbLWe3FMvuVUGiL
- The data set is given to identify 5 gestures 
- Videos are 30 frames per sec (30fps)
- The gestures are continuously monitored by the webcam mounted on the TV. Each gesture corresponds to a specific command:
 
| Gesture | Action |
| --- | --- | 
| Thumbs Up | Increase the volume. |
| Thumbs Down | Decrease the volume. |
| Left Swipe | 'Jump' backwards 10 seconds. |
| Right Swipe | 'Jump' forward 10 seconds. |
| Stop | Pause the movie. |

## Conclusions
![Metrics](https://github.com/vaidehiu/Gesture-recognition/blob/main/BestModel.png)
<br>
The best model chosen is Time distributed +GRU+CONV2D
<br>
The process of evaluation: Among the best listed Convlstm2d +timedistributed and Time distributed +GRU+CONV2D GRU gives best accuracy with considerable trainable params(ie; not too much )almost at same epoch as well. Infact LSTM model has very less params as less as 13k which makes it very simple model and takes less training time. But yet the best validation score was seen in GRU model.
**Reason**
- GRU model has 7 times less params than Conv3d (ie approx 1lakh params)
- Validation accuracy is maximum for simple model 81%
- Training accuracy is 85% which is good.
- Difference between train and validation is 4.4% less than 5% which is tolerable. This confirms there is tolerable overfitting of model or in other words model is not overfitted.
- Size of model approx – 1mb (1259kb)

**BEST MODEL:**  Time distributed +GRU+CONV2D




## Technologies Used
Pillow==9.0.1
matplotlib==3.5.0
imageio==2.19.0
keras==2.7.0
numpy==1.19.4
scikit-image==0.19.2
scipy == 1.4.1



## Contact
Reach out the creators on,
- Linkedin:
    - [Suresh Krishna](https://www.linkedin.com/in/sureshkrishh/)
    - [Vaidehiu](https://www.linkedin.com/in/vaidehiu/)
- Github:
    - [Suresh Krishna](https://github.com/Sureshkrishh)
    - [Vaidehiu](https://github.com/vaidehiu)    
