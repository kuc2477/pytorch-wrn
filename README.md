# Wide Residual Networks PyTorch Implementation

PyTorch Implementation of [Wide Residual Networks, BMVC 2016](http://www.bmva.org/bmvc/2016/papers/paper087/abstract087.pdf)

![residual-block](./arts/block.png)


## Installation
```
$ git clone https://github.com/kuc2477/pytorch-wrn && cd pytorch-wrn
$ pip install -r requirements.txt
```


## CLI
Implementation CLI is provided by `main.py`.

#### Usage 
```
$ ./main.py --help
$ usage: WRN torch implementation [-h] [--dataset {cifar100,mnist,cifar10}]
                                [--total-block-number TOTAL_BLOCK_NUMBER]
                                [--widen-factor WIDEN_FACTOR] [--lr LR]
                                [--epochs EPOCHS] [--batch-size BATCH_SIZE]
                                [--test-size TEST_SIZE]
                                [--checkpoint-interval CHECKPOINT_INTERVAL]
                                [--model-dir MODEL_DIR] [--resume] [--no-gpus]
                                (--test | --train)

optional arguments:
  -h, --help            show this help message and exit
  --dataset {cifar100,mnist,cifar10}
  --total-block-number TOTAL_BLOCK_NUMBER
  --widen-factor WIDEN_FACTOR
  --lr LR
  --epochs EPOCHS
  --batch-size BATCH_SIZE
  --test-size TEST_SIZE
  --checkpoint-interval CHECKPOINT_INTERVAL
  --model-dir MODEL_DIR
  --resume
  --no-gpus
  --test
  --train

```

#### Train
```
$ python -m visdom.server &
$ ./main.py --train [--resume-latest | --resume-best]
```

#### Test
```
$ ./main.py --test
```


## Reference
- [Wide Residual Networks, BMVC 2016](http://www.bmva.org/bmvc/2016/papers/paper087/abstract087.pdf)
- [dalgu90/wrn-tensorflow](https://github.com/dalgu90/wrn-tensorflow)


## Author
Ha Junsoo / [@kuc2477](https://github.com/kuc2477) / MIT License
