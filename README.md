## Introduction

The **Facial Action Coding System (FACS)** is a system for describing facial micro-expressions. A set of anotations called *Action Units (AU)* are manually defined by expert to categorize and labelize these AUs, that are generated by the movement of one or more facial muscles. At this day, 46 main AUs are defined in FACS, which their combinations can refer to a specific emotion.

> More informations : https://imotions.com/blog/learning/research-fundamentals/facial-action-coding-system/


```
@article{ekman1978facial,
  title={Facial action coding system},
  author={Ekman, Paul and Friesen, Wallace V},
  journal={Environmental Psychology \& Nonverbal Behavior},
  year={1978}
}
```

## Detection and Intensity Estimation

Detecting AUs is the task of predicting the presence (or not) of an AU for an image. AUs are also devided on 5 intensity levels, where *A* refers to a minimal activation level and *E* to a maximal level. Intensity estimation predicts the intensity of the AU.

## Data

The ***Denver Intensity of Spontaneous Facial Action (DISFA)*** database consists of over 130,000 examples from 27 participants, 12 women and 15 men, where each persons was recorder for 4 minutes reacting to stimuli video that were supposed to enable a particular expression on the subjects. For each video in the dataset, 12 Action Units were manually annotated  for each frame by a certified FACS expert.


>Dataset Info : 
>```
>@article{mavadati2013disfa,
  >title={Disfa: A spontaneous facial action intensity database},
  >author={Mavadati, S Mohammad and Mahoor, Mohammad H and Bartlett, Kevin and Trinh, Philip and Cohn, Jeffrey F},
  >journal={IEEE Transactions on Affective Computing},
  >volume={4},
  >number={2},
  >pages={151--160},
  >year={2013},
  >publisher={IEEE}
>} 
>```

## Face mesh

Here we rely on the facemesh extraction tool from [mediapipe](https://github.com/google/mediapipe/blob/master/docs/solutions/face_mesh.md) solutions.

![participant SN030 from DISFA](media/facemesh.gif)
