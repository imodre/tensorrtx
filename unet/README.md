# U-Net

For the Pytorch implementation, you can refer to [milesial/Pytorch-UNet](https://github.com/milesial/Pytorch-UNet)

```
// 1. generate mnasnet.wts from [pytorchx/mnasnet](https://github.com/wang-xinyu/pytorchx/tree/master/mnasnet)

// 2. put mnasnet.wts into tensorrtx/mnasnet

// 3. build and run

cd tensorrtx/mnasnet

mkdir build

cd build

cmake ..

make

sudo ./mnasnet -s   // serialize model to plan file i.e. 'mnasnet.engine'

sudo ./mnasnet -d   // deserialize plan file and run inference

// 4. see if the output is same as pytorchx/mnasnet
```

