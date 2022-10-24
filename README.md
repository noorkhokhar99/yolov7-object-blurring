# yolov7-object-blurring

### Steps to run Code
- Clone the repository.
```
git clone https://github.com/noorkhokhar99/yolov7-object-blurring.git
```
- Goto the cloned folder.
```
cd yolov7-object-blurring

```
- Upgrade pip with mentioned command below.
```
pip install --upgrade pip
```
- Install requirements with mentioned command below.
```
pip install -r requirements.txt
```
- Download [yolov7](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt) object detection weights from link and move them to the working directory {yolov7-object-blurring}
- Run the code with mentioned command below.
```
#if you want to change source file
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" --blurratio 20

#for specific class (person)
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" -classes 0 --blurratio 50

#hide-detected-bounding-boxes
python detect_and_blur.py --weights yolov7.pt --source "your video.mp4" -classes 0 --blurratio 50 --hidedetarea
```
- Output file will be created in the <b>working-dir/runs/detect/exp</b> with original filename.

### Results





