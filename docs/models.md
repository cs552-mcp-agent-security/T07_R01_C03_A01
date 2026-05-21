# Models overview

This page lists every model implementation under `models/`, roughly in the order
they appear in the README accuracy table.

| File | Architecture | Paper |
|------|--------------|-------|
| `models/vgg.py`         | VGG16            | Simonyan & Zisserman, 2014 |
| `models/resnet.py`      | ResNet18/50/101  | He et al., 2015 |
| `models/regnet.py`      | RegNetX/Y        | Radosavovic et al., 2020 |
| `models/mobilenetv2.py` | MobileNetV2      | Sandler et al., 2018 |
| `models/resnext.py`     | ResNeXt29        | Xie et al., 2017 |
| `models/dla_simple.py`  | SimpleDLA        | Yu et al., 2018 |
| `models/densenet.py`    | DenseNet121      | Huang et al., 2017 |
| `models/preact_resnet.py` | PreActResNet18 | He et al., 2016 |
| `models/dpn.py`         | DPN92            | Chen et al., 2017 |
| `models/dla.py`         | DLA              | Yu et al., 2018 |

All models share the same input shape (3 × 32 × 32) and the same number of output
classes (10). Switching architectures is a one-line change at the top of
`main.py` — replace `net = ResNet18()` with the model of your choice.

For the original CIFAR-10 accuracy results, see the table in `README.md`.
