# MOCHI
Comprehensible Counterfactual Interpretation on Kolmogorov-Smirnov Test

## Setup Experiment Environment

Use the following command to setup the experiment environment.

The command will install the dependencies required by MOCHI.

```
python setup.py install
```

## Interpretation Methods

`grace.py`: The baseline method GRACE [1].

`corner_search.py`: The basline method CornerSearch [2].

`mochi.py`: Our proposed method, MOCHI.

`baselines.py`: Abstract class of interpretation methods.

## Run Experiments

Produce interpretations with the preference list generated by Bitmap [3]



```
sh bin/run_exp_bitmap.sh
```

Produce interpretations with the preference list generated by Spectral Residual [4]


```
sh bin/run_exp_spectral.sh
```

## Dataset

We use the dataset in the NAB repository.


## Links

Bitmap Library: https://github.com/linkedin/luminol

Spectral Residual: https://docs.seldon.io/projects/alibi-detect/en/latest/api/modules.html

NAB Dataset: https://github.com/numenta/NAB/tree/master/data

## Reference

[1] Generating Concise and Informative Contrastive Sample to Explain Neural Network Model’s Prediction

[2] Sparse and Imperceivable Adversarial Attacks

[3] Assumption-free anomaly detection in timeseries

[4] Time-Series Anomaly De-tection Service at Microsoft
