# YOLO-person-tracking
You only look once
# Dependancies
Python3, tensorflow 1.0, numpy, opencv 3, Cython
# Setup 
python3 setup.py build_ext --inplace
1. Load yolo-tiny.weights
flow --model cfg/yolo-tiny.cfg --load bin/yolo-tiny.weights
Process all images in images/ using tiny yolo and 100% GPU usage
flow --imgdir images/ --model cfg/yolo-tiny.cfg --load bin/yolo-tiny.weights --gpu 1.0
