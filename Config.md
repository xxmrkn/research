># Configuration -not pretrained-
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
[^1]:The private leaderboard is calculated with approximately 81% of the test data.
---
># Configuration -pretrained-
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
| leader board | 0.25752 | 0.42800 | 0.43018 |
| training time | 320m 18s | 355m 1s | 358m 9s |