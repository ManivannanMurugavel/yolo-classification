# yolo-classification


## Prediction Command
`
./darknet classifier predict classify/classify.data classify/darknet19.cfg darknet19_46000.weights dog.jpg
`
** OUTPUT **
`
GPU isn't used 
 OpenCV version: 3.2.0
mini_batch = 1, batch = 1, time_steps = 1, train = 0 
   layer   filters  size/strd(dil)      input                output
   0 conv     32       3 x 3/ 1    224 x 224 x   3 ->  224 x 224 x  32 0.087 BF
   1 max                2x 2/ 2    224 x 224 x  32 ->  112 x 112 x  32 0.002 BF
   2 conv     64       3 x 3/ 1    112 x 112 x  32 ->  112 x 112 x  64 0.462 BF
   3 max                2x 2/ 2    112 x 112 x  64 ->   56 x  56 x  64 0.001 BF
   4 conv    128       3 x 3/ 1     56 x  56 x  64 ->   56 x  56 x 128 0.462 BF
   5 conv     64       1 x 1/ 1     56 x  56 x 128 ->   56 x  56 x  64 0.051 BF
   6 conv    128       3 x 3/ 1     56 x  56 x  64 ->   56 x  56 x 128 0.462 BF
   7 max                2x 2/ 2     56 x  56 x 128 ->   28 x  28 x 128 0.000 BF
   8 conv    256       3 x 3/ 1     28 x  28 x 128 ->   28 x  28 x 256 0.462 BF
   9 conv    128       1 x 1/ 1     28 x  28 x 256 ->   28 x  28 x 128 0.051 BF
  10 conv    256       3 x 3/ 1     28 x  28 x 128 ->   28 x  28 x 256 0.462 BF
  11 max                2x 2/ 2     28 x  28 x 256 ->   14 x  14 x 256 0.000 BF
  12 conv    512       3 x 3/ 1     14 x  14 x 256 ->   14 x  14 x 512 0.462 BF
  13 conv    256       1 x 1/ 1     14 x  14 x 512 ->   14 x  14 x 256 0.051 BF
  14 conv    512       3 x 3/ 1     14 x  14 x 256 ->   14 x  14 x 512 0.462 BF
  15 conv    256       1 x 1/ 1     14 x  14 x 512 ->   14 x  14 x 256 0.051 BF
  16 conv    512       3 x 3/ 1     14 x  14 x 256 ->   14 x  14 x 512 0.462 BF
  17 max                2x 2/ 2     14 x  14 x 512 ->    7 x   7 x 512 0.000 BF
  18 conv   1024       3 x 3/ 1      7 x   7 x 512 ->    7 x   7 x1024 0.462 BF
  19 conv    512       1 x 1/ 1      7 x   7 x1024 ->    7 x   7 x 512 0.051 BF
  20 conv   1024       3 x 3/ 1      7 x   7 x 512 ->    7 x   7 x1024 0.462 BF
  21 conv    512       1 x 1/ 1      7 x   7 x1024 ->    7 x   7 x 512 0.051 BF
  22 conv   1024       3 x 3/ 1      7 x   7 x 512 ->    7 x   7 x1024 0.462 BF
  23 conv      2       1 x 1/ 1      7 x   7 x1024 ->    7 x   7 x   2 0.000 BF
  24 avg                             7 x   7 x   2 ->      2
  25 softmax                                           2
Unused field: 'classes = 2'
  26 cost                                              2
Total BFLOPS 5.485 
avg_outputs = 211746 
Loading weights from darknet19_46000.weights...
 seen 64, trained: 1472 K-images (23 Kilo-batches_64) 
Done! Loaded 27 layers from weights-file 
 classes = 2, output in cfg = 0 
top: Using default '1'
224 224
dog1.jpg: Predicted in 889.085000 milli-seconds.
dog: 0.999985
`