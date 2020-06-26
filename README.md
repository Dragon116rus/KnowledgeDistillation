Thesis experiments with the Knowledge Distillation 
========================

This repository contain experiments for the following datasets in corresponding directories:

- CIFAR-10
- CIFAR-100
- CINIC-10

Experiments
-----------------
Before run the Knowledge Distillation you need to have already trained teacher models. For this purpose you can run `*_train_classic.ipynb` or you can download it by the following links:

CIFAR-10

- [ResNet 20](https://drive.google.com/open?id=1B8ucmEU8veZD1iLkvOIUdSUAOiFGRbmZ)  
- [ResNet 32](https://drive.google.com/open?id=1--j4BPPbVcYkV_Ivsl_KIRGv44BtyYOh)
- [ResNet 44](https://drive.google.com/open?id=1-1vVBhh2qmsPqD4KUcAdk0xl-7yjSojT)  
- [ResNet 56](https://drive.google.com/open?id=1-AdSye8yDTB4HaFxSgiS3Q6fFv-dS1WZ)

CIFAR-100

- [ResNet 20](https://drive.google.com/open?id=1-7svennxwIE_xFkIxXwcPPQujiZUa3If)  
- [ResNet 32](https://drive.google.com/open?id=1-L7WJtrmrOYCrZJcJhw-2MsUzxt0odwv)

CINIC-10

- [ResNet 20](https://drive.google.com/open?id=1zL4TMAWkEK_dzOTZ347v3gqBKTGZQqA2)  
- [ResNet 32](https://drive.google.com/open?id=1-eIcGuuRP8XuMCe3p6lOClE4B5DAHiaX)


There are 3 types of the Knowledge Distillation:

- `*_distillation_train.ipynb` - classical Knowledge Distillation approach
- `cached_*_distillation.ipynb` - classical Knowledge Distillation approach, but without using augmentations
- `aug_cached_*_distillation.ipynb` - proposed Knowledge Distillation approach

Logs
-----------------
To see the logs you can use `tensorboard`. 
You can use the following comand to run it:

```tensorboard --logdir {directory path} ```

where `directory path` - path to directory which contain logs (it may have in subdirs).

For example if you want to see all logs you can use:

 ```tensorboard --logdir . ```

 Or if you want to see logs of CIFAR-10 experiments you can use:

 ```tensorboard --logdir cifar10```
