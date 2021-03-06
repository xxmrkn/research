># Experiment 1 (Pretrained = False, Data Augmentation = False)
### [ parameter ]
| model architechture | vit_base_patch16_224 | resnet18d | vgg11 |
| ---- | ---- | ---- | ---- |
| image size | 224×224 | 224×224 | 224×224 |
| batch size | 32 | 32 | 32 |
| debug size | 0.2 | 0.2 | 0.2 |
| epoch | 10 | 10 | 10 |
| lr | 1e-4 | 1e-4 | 1e-4 |
| optimizer | Adam | Adam | Adam |
| criterion | CrossEntropyLoss | CrossEntropyLoss | CrossEntropyLoss |
| random state | 1234 | 1234 | 1234 |

### [ result ]
| model architechture | vit_base_patch16_224 | resnet18d | vgg11 |
| -- | -- | -- | -- |
| best valid accuracy | 0.5906 | 0.8209 | 0.8384 |
| best valid f1-score | 0.4453 | 0.6283 | 0.6349 |
| best valid loss | 1.1983 | 0.5554 | 0.5132 |
| leader board (private)[^1] | 0.31705 (0.32631) | 0.65960 (0.66038) | 0.67843 (0.68653) |
| training time | 320m 18s | 355m 1s | 358m 9s |
---
># Experiment 2 (Pretrained = True, Data Augmentation = False)
### [ parameter ]
| model architechture | vit_base_patch16_224 | resnet18d | vgg11 |
| ---- | ---- | ---- | ---- |
| image size | 224×224 | 224×224 | 224×224 |
| batch size | 32 | 32 | 32 |
| debug size | 0.2 | 0.2 | 0.2 |
| epoch | 10 | 10 | 10 |
| lr | 1e-4 | 1e-4 | 1e-4 |
| optimizer | Adam | Adam | Adam |
| criterion | CrossEntropyLoss | CrossEntropyLoss | CrossEntropyLoss |
| random state | 1234 | 1234 | 1234 |

### [ result ]
| model architechture | vit_base_patch16_224 | resnet18d | vgg11 |
| -- | -- | -- | -- |
| best valid accuracy | 0.8312 | 0.8568 | 0.8611 |
| best valid f1-score | 0.6605 | 0.6708 | 0.6798 |
| best valid loss | 0.5562 | 0.4989 | 0.4433 |
| leader board (private)[^1] | 0.66773 (0.65804) | 0.73314 (0.73534) | 0.72685 (0.73933) |
| training time | 325m 14s | 346m 46s | 379m 59s |
[^1]:The private leaderboard is calculated with approximately 81% of the test data.

># Train1Epoch (Optimizer : SGD momentum)
### [ parameter ]
| model architechture | f1(lr = 1e-4) | f1 (lr = 1e-3) |
| ---- | ---- | ---- |
| vit_base_patch16_224 | 0.6713 | 0.6429 |
| resnet18d | 0.1160 | 0.4590 |
| vgg11 | 0.5555 | 0.6348 |

># Train1Epoch (Optimizer : Adam)
### [ parameter ]
| model architechture | f1(lr = 1e-4) | f1 (lr = 1e-3) |
| ---- | ---- | ---- |
| vit_base_patch16_224 | 0.6501 | 0.1447 |
| resnet18d | 0.6319 | 0.6090 |
| vgg11 | 0.6725 | 0.0874 |

># Experiment 3 (Pretrained = True, Data Augmentation = True, Optimizer : Adam)
### [ parameter ]
| model architechture | vit_base_patch16_224 | resnet18d | vgg11 |
| ---- | ---- | ---- | ---- |
| image size | 224×224 | 224×224 | 224×224 |
| batch size | 32 | 32 | 32 |
| debug size | 0.2 | 0.2 | 0.2 |
| epoch | 10 | 10 | 10 |
| lr | 1e-4 | 1e-4 | 1e-4 |
| optimizer | Adam | Adam | Adam |
| criterion | CrossEntropyLoss | CrossEntropyLoss | CrossEntropyLoss |
| random state | 1234 | 1234 | 1234 |

### [ result ]
| model architechture | vit_base_patch16_224 | resnet18d | vgg11 |
| -- | -- | -- | -- |
| best valid accuracy | 0.8806 | 0.8881 | 0.8856 |
| best valid f1-score | 0.7199 | 0.7141 | 0.7114 |
| best valid loss | 0.3809 | 0.3626 | 0.3635 |
| leader board (private)[^1] | 0.68272 (0.69591) | 0.73448 (0.74777) | 0.72075 (0.73026) |
| training time | 332m 48s | 313m 16s | 438m 55s |

># Best Score (Pretrained = True, Data Augmentation = True)
### [ parameter ]
| model architechture | vit_base_patch16_224 | resnet18d | vgg11 |
| ---- | ---- | ---- | ---- |
| image size | 224×224 | 224×224 | 224×224 |
| batch size | 32 | 32 | 32 |
| debug size | 0.2 | 0.2 | 0.2 |
| epoch | 10 | 10 | 10 |
| lr | 1e-4 | 1e-4 | 1e-4 |
| optimizer | SGD | Adam | Adam |
| criterion | CrossEntropyLoss | CrossEntropyLoss | CrossEntropyLoss |
| random state | 1234 | 1234 | 1234 |

### [ result ]
| model architechture | vit_base_patch16_224 | resnet18d | vgg11 |
| -- | -- | -- | -- |
| best valid accuracy | 0.8987 | 0.8881 | 0.8856 |
| best valid f1-score | 0.7284 | 0.7141 | 0.7114 |
| best valid loss | 0.3301 | 0.3626 | 0.3635 |
| leader board (private)[^1] | 0.73448 (0.74941) | 0.73448 (0.74777) | 0.72075 (0.73026) |
| training time | ???m ??s | 313m 16s | 438m 55s |