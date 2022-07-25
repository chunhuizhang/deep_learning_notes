
## 0. minst/fashion-mnist

- mnist: 0-9 手写字符（10分类，28*28）
- fashion-mnist：服装类灰度图像识别（10分类，28*28）

```python

from torchvision import datasets
training_data = datasets.FashionMNIST(
    root="data",
    train=True,
    download=True,
    transform=ToTensor()
)

test_data = datasets.FashionMNIST(
    root="data",
    train=False,
    download=True,
    transform=ToTensor()
)
```

## 1. imagenet

- 图像分类问题

## 2. voc

## 3. coco
