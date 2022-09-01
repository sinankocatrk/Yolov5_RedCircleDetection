<div align="center">
<p>
   <a align="left" href="https://medium.com/@sinankocatrk/g%C3%B6r%C3%BCnt%C3%BC-i%C5%9Fleme-raporlar%C4%B1m-1-d360f4548175" target="_blank">
   <img width="550" src="https://user-images.githubusercontent.com/76816180/187943155-70622b45-73d5-4d03-9487-39cbe45e56b3.png"></a>
</p>
<br>

<br>
<p>
YOLOv5 🚀 is a family of object detection architectures and models pretrained on the COCO dataset, and represents <a href="https://ultralytics.com">Ultralytics</a>
 open-source research into future vision AI methods, incorporating lessons learned and best practices evolved over thousands of hours of research and development.
</p>



<!--
<a align="center" href="https://ultralytics.com/yolov5" target="_blank">
<img width="800" src="https://github.com/ultralytics/yolov5/releases/download/v1.0/banner-api.png"></a>
-->

</div>

## <div align="center">Documentation</div>

[Medium Article1](https://medium.com/@sinankocatrk/g%C3%B6r%C3%BCnt%C3%BC-i%C5%9Fleme-raporlar%C4%B1m-1-d360f4548175) <br>
[Medium Article2](https://medium.com/@sinankocatrk/g%C3%B6r%C3%BCnt%C3%BC-i%CC%87%C5%9Fleme-raporlar%C4%B1m-2-112ebd0c9faf) <br>
[Medium Article3](https://medium.com/p/c94694c69527)

## <div align="center">Quick Start Examples</div>

<details open>
<summary>Install</summary>

Clone repo and install [requirements.txt](https://github.com/ultralytics/yolov5/blob/master/requirements.txt) in a
[**Python>=3.7.0**](https://www.python.org/) environment, including
[**PyTorch>=1.7**](https://pytorch.org/get-started/locally/).

```bash
git clone https://github.com/sinankocatrk/Yolov5_RedCircleDetection  # clone
cd yolov5
pip install -r requirements.txt  # install
```

</details>

<details open>
<summary>Inference</summary>

Inference with YOLOv5 and [PyTorch Hub](https://github.com/ultralytics/yolov5/issues/36)
. [Models](https://github.com/ultralytics/yolov5/tree/master/models) download automatically from the latest
YOLOv5 [release](https://github.com/ultralytics/yolov5/releases).

```python
import torch

# Model
model = torch.hub.load('ultralytics/yolov5', 'yolov5s')  # or yolov5m, yolov5l, yolov5x, custom

# Images
img = 'https://ultralytics.com/images/zidane.jpg'  # or file, Path, PIL, OpenCV, numpy, list

# Inference
results = model(img)

# Results
results.print()  # or .show(), .save(), .crop(), .pandas(), etc.
```

</details>



<details>
<summary>Inference with detect.py</summary>

`detect.py` runs inference on a variety of sources, downloading [models](https://github.com/ultralytics/yolov5/tree/master/models) automatically from
the latest YOLOv5 [release](https://github.com/ultralytics/yolov5/releases) and saving results to `runs/detect`.

```bash
python detect.py --source 0  # webcam
                          img.jpg  # image
                          vid.mp4  # video
                          path/  # directory
                          path/*.jpg  # glob
                          'https://youtu.be/Zgi9g1ksQHc'  # YouTube
                          'rtsp://example.com/media.mp4'  # RTSP, RTMP, HTTP stream
```

</details>

<details>



