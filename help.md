# Generate fake data
````bash
 python "./src/main.py" --load_best -sf -sf_num 50000 -metrics none -cfg "./src/configs/CIFAR10/DCGAN.yaml" -data "C:\datasets\cifar10" -ckpt "./ckpt" -save "./output/DCGAN"
````

# Compute FID for two folders
```bash
python "./src/evaluate.py" -metrics fid --dset1 "C:\datasets\light\cifar10-image-folder\train" --dset2 "./output/DCGAN/samples/CIFAR10-DCGAN-train-2022_01_11_20_32_07/fake"
```
