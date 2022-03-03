
yolov3 checkpoints file
"/home/ava/sarala/yolov3/yolov3/weights/yolov3.pt"

yolov3 onnx file
"/home/ava/sarala/yolov3/yolov3/weights/yolov3.onnx"

yolov3 coco val dataset location
/home/ava/DATASET/coco/val2017
"/home/ava/sarala/yolov3/datasets/coco/"

yolov3 onnx export script & command
python export.py --weights /home/ava/sarala/yolov3/yolov3/weights/yolov3.pt --include onnx


yolov3 onnx validation script  & command
python val.py --weights /home/ava/sarala/yolov3/yolov3/weights/yolov3.onnx

project location
/home/ava/sarala/yolov3/

env location
"/home/ava/anaconda3/envs/yolov3_onnx/"

requirements file location
"/home/ava/sarala/yolov3/yolov3/requirements.txt"

pip list file
"/home/ava/sarala/yolov3/yolov3/pip_list.txt"

======
raw file creation

python create_coco_100_rawfiles.py

======
raw file validation
100 raw files
python onnx_validation_raw_files.py --weights /home/ava/sarala/yolov3/yolov3/weights/yolov3.onnx

python val_100_images.py --weights /home/ava/sarala/yolov3/yolov3/weights/yolov3.onnx

python val_100_images.py --weights /home/ava/sarala/yolov3/yolov3/weights/yolov3.pt

