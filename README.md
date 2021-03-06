# AliNet
Source code for AAAI-2020 paper "[Knowledge Graph Alignment Network with Gated Multi-hop Neighborhood Aggregation](https://arxiv.org/pdf/1911.08936.pdf)". 

<p align="center">
  <img width="90%" src="https://github.com/nju-websoft/AliNet/blob/master/architecture.png" />
</p>

## Dataset
We use two entity alignment datasets DBP15K and DWY100K in our experiments. DBP15K can be downloaded from [JAPE](https://github.com/nju-websoft/JAPE) and DWY100K is from [BootEA](https://github.com/nju-websoft/BootEA).


## Code
> The code of AliNet (w/o relation loss) is now available. Other code is under refactoring and coming soon.

* "alinet.py" is the implementation of AliNet (w/o rel. loss).

### Dependencies
* Python 3
* Tensorflow 2.0 (**Important!!!**) 
* Scipy
* Numpy
* Pandas
* Scikit-learn

For example, to run AliNet (w/o rel. loss) on DBP15K ZH-EN, use the following script (supposed that the DBK15K dataset has been downloaded into the folder '../data/'):
```
python3 main.py --input ../data/DBP15K/zh_en/mtranse/0_3/
```

To run AliNet (w/o rel. loss) on DBP15K, use the following script:
```
bash run_dbp15k.sh
```

> If you have any difficulty or question in running code and reproducing experimental results, please email to zqsun.nju@gmail.com or cmwang.nju@gmail.com.

## Citation
If you use our model or code, please kindly cite it as follows:      
```
@inproceedings{AliNet,
  author    = {Zequn Sun,
               Chengming Wang, 
               Wei Hu, 
               Muhao Chen, 
               Jian Dai, 
               Wei Zhang, 
               Yuzhong Qu},
  title     = {Knowledge Graph Alignment Network with Gated Multi-hop Neighborhood Aggregation},
  booktitle = {AAAI},
  year      = {2020}
}
```