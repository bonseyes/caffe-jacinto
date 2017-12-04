# Bonseyes Official Caffe 1.0 Version
###### Caffe-jacinto

Bonseyes Caffe-jacinto is a fork of [tidsp/caffe-jacinto](https://github.com/tidsp/caffe-jacinto) which is a fork of [NVIDIA/caffe](https://github.com/NVIDIA/caffe), which in-turn is derived from [BVLC/Caffe](https://github.com/BVLC/caffe). The modifications in this fork enable training of sparse, quantized CNN models - resulting in low complexity models that can be used in embedded platforms.

The following additional caffe layers have been integrated:
- Single shot detection (SDD) (https://github.com/weiliu89/caffe/tree/ssd) for object detection.
- ImageLabelData and IOUAccuracy layers have been added to train for semantic segmentation.

Modifications relative to original [BVLC/Caffe]
- Pooling layer have been modified from ceil to floor to be compatible to pytorch
- Sparsity training methods (https://github.com/wenwei202/caffe/tree/scnn) have been integrated
- Quantization methods based on Ristretto (https://github.com/pmgysel/caffe) have been integrated

### Future layers to be supported
Additional extensions to be supported.

- Sphereface (https://github.com/wy1iu/sphereface)
- Squeeze and excitation networks (https://github.com/hujie-frank/SENet)
- Additional sparsity methods

## License and Citation

Caffe is released under the [BSD 2-Clause license](https://github.com/BVLC/caffe/blob/master/LICENSE).
The BVLC reference models are released for unrestricted use.

Please cite Caffe in your publications if it helps your research:

    @article{jia2014caffe,
      Author = {Jia, Yangqing and Shelhamer, Evan and Donahue, Jeff and Karayev, Sergey and Long, Jonathan and Girshick, Ross and Guadarrama, Sergio and Darrell, Trevor},
      Journal = {arXiv preprint arXiv:1408.5093},
      Title = {Caffe: Convolutional Architecture for Fast Feature Embedding},
      Year = {2014}
    }
