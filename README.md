# EasyYOLOv7

[![Open In Colab] (https://colab.research.google.com/drive/1ZeDkhcCN-xsbmu8zea7enK3Kqa1xfOhk?usp=sharing)](https://colab.research.google.com/drive/1ZeDkhcCN-xsbmu8zea7enK3Kqa1xfOhk?usp=sharing)



This repo contains a simple notebook **Train_YOLOv7.ipynb** to train multiple instance of YoloV7  with pytorch. 

The directory structure:
    
 
    ├────── yolov5
    ├────── Train_YOLOv7.ipynb
    ├────── README.md
    

# Instructions
## Setup on Google Drive
Link notebook with your google drive for saving checkpoint,




    
## convert model to tflite 
```
!python3 export.py --weights ../{instance_name}/best.pt --include tflite --optimize --nms #--int8
```

## convert model to tfjs 
```
!python3 export.py --weights ../{instance_name}/best.pt --include tfjs --optimize --nms #--int8
```

## convert model to torchscript 
```
!python3 export.py --weights ../{instance_name}/best.pt --include torchscript --optimize --nms #--int8
```
