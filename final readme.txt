python create_coco_100_rawfiles.py

with 100 val files
in val.py script coco.yaml is set like below
parser.add_argument('--data', type=str, default=ROOT / 'data/coco.yaml', help='dataset.yaml path') 
in coco.yaml , val2017_100.txt  is with sorted asc images set
val: val2017_100.txt 
python val_100_images.py --weights "/home/ava/sarala/yolov3/yolov3/selva_simplified_onnx/yolov3_simplified_new.onnx"

python val_100_images.py --weights /home/ava/sarala/yolov3/yolov3/weights/yolov3.pt

python onnx_validation_raw_files.py --weights "/home/ava/sarala/yolov3/yolov3/selva_simplified_onnx/yolov3_simplified_new.onnx"


with 5000 val files
in val_5000.py script coco_5000_val.yaml is set like below
parser.add_argument('--data', type=str, default=ROOT / 'data/coco_5000_val.yaml', help='dataset.yaml path') 
in coco_5000_val.yaml , val2017.txt  is with 5000 images set
val: val2017.txt 
python val_5000.py --weights "/home/ava/sarala/yolov3/yolov3/selva_simplified_onnx/yolov3_simplified_new.onnx"
python val_5000.py --weights /home/ava/sarala/yolov3/yolov3/weights/yolov3.pt


python export.py --weights /home/ava/sarala/yolov3/yolov3/weights/yolov3.pt --include onnx