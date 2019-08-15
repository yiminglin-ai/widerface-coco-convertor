# Convert WIDERFace annotations to COCO format.

Download [widerface](http://shuoyang1213.me/WIDERFACE/) and put it in `data/`, the directory tree should look like the following: 
```shell
data
└── widerface
    ├── wider_face_split
    ├── WIDER_train
    │   └── images
    │       ├── 0--Parade
    │       └── ...
    └── WIDER_val
        └── images
            ├── 0--Parade
            ├── ...
```

convert the annotations:
```shell
python scripts/convert_widerface_to_coco.py --datadir data/widerface  --subset all --outdir ./
```
