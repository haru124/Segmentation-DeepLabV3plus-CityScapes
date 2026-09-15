Reference repo : https://github.com/Tramac/awesome-semantic-segmentation-pytorch


│
├── data/ 
|    |__images
|    |   |_train -- subset of city folders
|    |   |_test
|    |   |_val
|    |
|    |__gtFine
|        |_train
|        |_test
|        |_val
|                 
|___ weights    # pretrained model weights -- initial loading
|
├── src/ods/
│   ├── constants/
│   │   └── __init__.py
│   │
│   ├── entity/
│   │   └── config_entity.py
│   │
│   ├── config/
│   │   └── configuration.py
│   │
│   ├── datasets/
│   │   ├── cityscapes_dataset.py
│   │   └── transforms.py
│   │   └── dataloader.py
│   │
│   ├── models/
│   │   ├── backbones
|   |   |        |-----resnet.py     (-- same as in repo)
|   |   |        |-----resnetv1b.py    (-- same as in repo)
|   |   |        |-----mobilenetv2.py       (-- same as in repo)
|   |   |-----nn 
|   |   |     |-----basic.py     (-- same as in repo)
|   |   |     |-----jpu.py        (-- same as in repo)
│   │   └── deeplabv3_plus.py    ---- (-- same as in repo -- ) 
│   │
│   ├── losses/
│   │   └── losses.py   #empty
│   │
│   ├── evaluation/
│   │   └── metrics.py
│   │
│   ├── training/
│   │   └── trainer.py
│   │_____ inference  
|   |          |___ inference.py 
|   |
|   | 
│   |____ onnx  
|   |      |___ inference.py 
|   |       |___ export.py
|   |
|   | 
│   ├── tracking/                   # ✅ NEW (simple, clean)
│   │   ├── mlflow_logger.py
│   │   └── tensorboard_logger.py
│   │
|   |___ profiler
|   |     |__profiler_utils.py
|   |	   
|   |
│   └── utils/
│       ├── common.py
│       ├── checkpoint.py           # ✅ save/load models
│       └── visualization.py        # ✅ debug + predictions
│
│
├── config/
│   ├── config.yaml
│   └── experiments/
│       ├── exp_01.yaml
│       ├── exp_02.yaml
│       └── exp_03.yaml
│
├── outputs/                        # ✅ ALL GENERATED STUFF
|   |-----inference/ exp folders/ plots and visualization folders-- stored plots and         |     |                   inference images
│   ├── checkpoints/   -- must be stored with exp name, loss, primary val metric | |       |     |                   value, epoch number
│   ├── logs/
│   ├── tensorboard/
│   ├── mlruns/
│   └── profiler/
│ 
│
├── main.py
├── template.py                     # ✅ folder generator
├── requirements.txt
└── Dockerfile
