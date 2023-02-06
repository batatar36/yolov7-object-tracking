# yolov7-object-tracking


### Steps to run Code
- Clone the repository.
```
git clone https://github.com/batatar36/yolov7-object-tracking.git
```
- Go to the cloned folder.
```
cd yolov7-object-tracking
```
- Upgrade pip with mentioned command below.
```
pip install --upgrade pip
```
- Install requirements with mentioned command below.
```
pip install -r requirements.txt
```
- Run the code with mentioned command below (by default, pretrained [yolov7](https://github.com/WongKinYiu/yolov7/releases/download/v0.1/yolov7.pt) weights will be automatically downloaded into the working directory if they don't already exist).
```
# for detection only
python detect.py --weights yolov7.pt --source "your video.mp4"

#if you want to change source file
python detect_and_track.py --weights yolov7.pt --source "your video.mp4"

#for WebCam
python detect_and_track.py --weights yolov7.pt --source 0

#for External Camera
python detect_and_track.py --weights yolov7.pt --source 1
```

- Output file will be created in the ```working-dir/runs/detect/obj-tracking``` with original filename
