<!--
 * @Author: wayne
 * @LastEditors: wayne
 * @Date: 2022-09-24 21:40:27
 * @LastEditTime: 2022-10-09 15:22:43
 * @Description: 
-->
# Official YOLOv7

## add Decoupled Head Test


```shell
python -m torch.distributed.launch --nproc_per_node 2 --master_port 9527 train.py --workers 8 --device 0,1 --sync-bn --batch-size 24 --data ./data/coco.yaml --img 640 640 --cfg cfg/training/yolov7.yaml --weights ./yolov7_training.pt --name yolov7 --hyp data/hyp.scratch.p5.yaml 
```