# FFN object detection experiment on darknet

About Darknet framework: http://pjreddie.com/darknet/

The use of the framework on Windows and Linux:：https://github.com/AlexeyAB/darknet

The cfg file of this work is in the cfg folder.
* yolov4-train-sgd.cfg: stochastic gradient descent method with momentum to train YOLOv4, using a step-by-step learning strategy, a total of 30,000 iterations are trained, and the learning rate drops to one-tenth of the original at 15,000 and 25,000 iterations, respectively.
* yolov4-train-adam.cfg: use Adam optimizer to train YOLOv4, using a step-by-step learning strategy, a total of 30,000 iterations are trained, and the learning rate drops to one-tenth of the original at 15,000 and 25,000 iterations, respectively.
* yolov4-pretrain-sgd.cfg: stochastic gradient descent method with momentum to train YOLOv4, using a step-by-step learning strategy, a total of 20,000 iterations are trained, and the learning rate drops to one-tenth of the original at 14,000 and 18,000 iterations, respectively.
* yolov4-pretrain-adam.cfg: use Adam optimizer to train YOLOv4, using a step-by-step learning strategy, a total of 20,000 iterations are trained, and the learning rate drops to one-tenth of the original at 14,000 and 18,000 iterations, respectively.

* cspdaknet53+ffn-train-sgd.cfg: stochastic gradient descent method with momentum to train the combination of FFN and CSPDaknet53, using a step-by-step learning strategy, a total of 30,000 iterations are trained, and the learning rate drops to one-tenth of the original at 15,000 and 25,000 iterations, respectively.
* cspdaknet53+ffn-train-adam.cfg: use Adam optimizer to train the combination of FFN and CSPDaknet53, using a step-by-step learning strategy, a total of 30,000 iterations are trained, and the learning rate drops to one-tenth of the original at 15,000 and 25,000 iterations, respectively.
* cspdaknet53+ffn-pretrain-sgd.cfg: stochastic gradient descent method with momentum to train the combination of FFN and CSPDaknet53, using a step-by-step learning strategy, a total of 20,000 iterations are trained, and the learning rate drops to one-tenth of the original at 14,000 and 18,000 iterations, respectively.
* cspdaknet53+ffn-pretrain-adam.cfg: use Adam optimizer to train the combination of FFN and CSPDaknet53, using a step-by-step learning strategy, a total of 20,000 iterations are trained, and the learning rate drops to one-tenth of the original at 14,000 and 18,000 iterations, respectively.

* yolov4-tiny-train-sgd.cfg: stochastic gradient descent method with momentum to train YOLOv4-Tiny, using a step-by-step learning strategy, a total of 30,000 iterations are trained, and the learning rate drops to one-tenth of the original at 15,000 and 25,000 iterations, respectively.
* yolov4-tiny-train-adam.cfg: use Adam optimizer to train YOLOv4-Tiny, using a step-by-step learning strategy, a total of 30,000 iterations are trained, and the learning rate drops to one-tenth of the original at 15,000 and 25,000 iterations, respectively.
* yolov4-tiny-pretrain-sgd.cfg: stochastic gradient descent method with momentum to train YOLOv4-Tiny, using a step-by-step learning strategy, a total of 20,000 iterations are trained, and the learning rate drops to one-tenth of the original at 16,000 and 18,000 iterations, respectively.
* yolov4-tiny-pretrain-adam.cfg: use Adam optimizer to train YOLOv4-Tiny, using a step-by-step learning strategy, a total of 20,000 iterations are trained, and the learning rate drops to one-tenth of the original at 16,000 and 18,000 iterations, respectively.

* cspdaknet53-tiny+ffn-train-sgd.cfg: stochastic gradient descent method with momentum to train the combination of FFN and CSPDaknet53-tiny, using a step-by-step learning strategy, a total of 30,000 iterations are trained, and the learning rate drops to one-tenth of the original at 15,000 and 25,000 iterations, respectively.
* cspdaknet53-tiny+ffn-train-adam.cfg: use Adam optimizer to train the combination of FFN and CSPDaknet53-tiny, using a step-by-step learning strategy, a total of 30,000 iterations are trained, and the learning rate drops to one-tenth of the original at 15,000 and 25,000 iterations, respectively.
* cspdaknet53-tiny+ffn-pretrain-sgd.cfg: stochastic gradient descent method with momentum to train the combination of FFN and CSPDaknet53-tiny, using a step-by-step learning strategy, a total of 20,000 iterations are trained, and the learning rate drops to one-tenth of the original at 16,000 and 18,000 iterations, respectively.
* cspdaknet53-tiny+ffn-pretrain-adam.cfg: use Adam optimizer to train the combination of FFN and CSPDaknet53-tiny, using a step-by-step learning strategy, a total of 20,000 iterations are trained, and the learning rate drops to one-tenth of the original at 16,000 and 18,000 iterations, respectively.

The pre-training weights of YOLOv4 and CSPDaknet53+FFN extract 105 layers from https://github.com/AlexeyAB/darknet/releases/download/darknet_yolo_v3_optimal/yolov4.weights.

The pre-training weights of YOLOv4-Tiny and CSPDaknet53-Tiny+FFN extract 27 layers from https://github.com/AlexeyAB/darknet/releases/download/darknet_yolo_v4_pre/yolov4-tiny.weights.

The log files during the experiment are stored in the log folder, and all the data in our work comes from this, the file naming rules are consistent with the cfg file.

The visualization results during training are stored in the results folder, the file naming rules are consistent with the cfg file.

The training dataset comes from https://pjreddie.com/media/files/VOCtrainval_11-May-2012.tar and https://pjreddie.com/media/files/VOCtrainval_06-Nov-2007.tar.

The testing dataset comes from https://pjreddie.com/media/files/VOCtest_06-Nov-2007.tar.
