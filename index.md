<div><h1 align="center">  RevIN </h1></div>
<div><h3 align="center">Reversible Instance Normalization for Accurate Time-Series Forecasting against Distribution Shift</h3></div>
<div><h3 align="center">ICLR 2022</h3></div>


<div align="center">
<a href="https://github.com/ts-kim/">Taesung Kim*</a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
<a href="https://sites.google.com/view/jinhee-kim">Jinhee Kim*</a> &nbsp;&nbsp;&nbsp;  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://openreview.net/profile?id=~Yunwon_Tae1">Yunwon Tae</a> &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
<a href="https://cbokpark.github.io/">Cheonbok Park</a> &nbsp;&nbsp;&nbsp;  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
<a href="https://github.com/jangho87">Jang-Ho Choi</a> &nbsp;&nbsp;&nbsp;  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; 
<a href="https://sites.google.com/site/jaegulchoo/">Jaegul Choo</a>
</div>

<div align="center">
KAIST AI &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
KAIST AI &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
VUNO &nbsp;&nbsp;&nbsp;  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
NAVER Corp. &nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
ETRI &nbsp;&nbsp;&nbsp;  &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
KAIST AI
</div>

<div align="center">
*Denotes Equal Contribution
</div>


<div style="display: flex; flex-direction: row;">
 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://openreview.net/forum?id=cGDAkQo1C0p"><img src="icons/paper.png" width="50px"></a> &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="https://github.com/ts-kim/revin/"><img src="icons/github.png" width="50px"></a> 
</div>

<img src="./figs/fig1.gif" width="1000px" height="500px">


# Poster
<img src="./figs/RevIN_Poster_ICLR_2O22.jpg" width="1000px" height="562px">


# Abstract

Statistical properties such as mean and variance often change over time in time series, i.e., time-series data suffer from a distribution shift problem. This change in temporal distribution is one of the main challenges that prevent accurate time-series forecasting. To address this issue, we propose a simple yet effective normalization method called reversible instance normalization (RevIN), a generally applicable normalization-and-denormalization method with learnable affine transformation. The proposed method is symmetrically structured to remove and restore the statistical information of a time-series instance, leading to significant performance improvements in time-series forecasting, as shown in Fig. 1. We demonstrate the effectiveness of RevIN via extensive quantitative and qualitative analyses on various real-world datasets, addressing the distribution shift problem.


# Experimental Results

RevIN can alleviate the distribution discrepancy problem by removing
non-stationary information in the input layer and then restoring it in the output layer. The
analysis is conducted on the ETT and ECL datasets using SCINet (Liu et al., 2021) as the baseline.

<img src="./figs/fig3.PNG" width="1000px" height="500px">


These are prediction results on three variables in the Nasdaq data,
Close, DTB6, and DE1, to verify the effectiveness
of RevIN on obvious non-stationary time series.

<img src="./figs/fig6.PNG" width="1000px" height="800px">

<!-- 
RevIN
consistently outperforms all three baselines, Informer, N-BEATS, and SCINet, by a large margin, achieving state-of-the-art performance. RevIN shows robust performance against the prediction length.

<img src="./figs/table1.PNG" width="1000px" height="500px">



RevIN significantly improves the forecasting performance of the baselines on
on additional real-world datasets.

<img src="./figs/table4.PNG" width="1000px" height="500px">



RevIN shows outstanding performance compared to classical and state-of-the-art normalization methods normalization methods,

<img src="./figs/table3.PNG" width="1000px" height="500px">



In time series, a domain can be a location of a sensor where
the data is collected. Here, RevIN successfully solves the distribution shift problem by alleviating data distribution discrepancy between different domains, leading to better generalization performance in the cross-domain time-series forecasting task.

<img src="./figs/table5.PNG" width="1000px" height="500px">
 -->


Additional multivariate time-series forecasting results.
 

<img src="./figs/fig9.jpg" width="1000px">



# Citation

```
@inproceedings{
    kim2022reversible,
    title={Reversible Instance Normalization for Accurate Time-Series Forecasting against Distribution Shift},
    author={Taesung Kim and Jinhee Kim and Yunwon Tae and Cheonbok Park and Jang-Ho Choi and Jaegul Choo},
    booktitle={International Conference on Learning Representations},
    year={2022},
    url={https://openreview.net/forum?id=cGDAkQo1C0p}
}
```
