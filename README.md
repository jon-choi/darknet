![Darknet Logo](http://pjreddie.com/media/files/darknet-black-small.png)

#Darknet#
Darknet is an open source neural network framework written in C and CUDA. It is fast, easy to install, and supports CPU and GPU computation.

For more information see the [Darknet project website](http://pjreddie.com/darknet).

For questions or issues please use the [Google Group](https://groups.google.com/forum/#!forum/darknet).

#Commands#
Run vanilla detector: ./darknet detect cfg/yolo.cfg yolo.weights [FILE]
Run JChoi counter: ./darknet counter cfg/yolo.cfg yolo.weights [FILE] [CLASS]
Run video: ./darknet detector demo cfg/coco.data cfg/yolo.cfg yolo.weights [video path] -prefix [prefix string] -class [only detect this class]
Stitch output: ffmpeg -f image2 -r 25 -start_number 1 -i [pred__%08d.jpg] -s 720x480 [filename for output]
