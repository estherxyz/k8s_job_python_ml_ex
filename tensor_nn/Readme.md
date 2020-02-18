# Tensorflow NN training Sample

## Description
NN training sample for verifing AFS function.

Verify item:
+ tensorflow image
+ cpu using
+ gpu using
+ K8S coreDNS (get file from github)


### GPU Tensorflow NN sample
File: `/nn_gpu_ex.py`

Using tensorflow NN with GPU.
```
# get source code from github. Then execute.
$ curl https://raw.githubusercontent.com/estherxyz/k8s_job_python_ml_ex/nn_ex/tensor_nn/nn_gpu_ex.py > nn_ex.py && python nn_ex.py
```


### CPU Tensorflow NN sample
File: `/nn_cpu_ex.py`

Using tensorflow NN without GPU.
```
# get source code from github. Then execute.
$ curl https://raw.githubusercontent.com/estherxyz/k8s_job_python_ml_ex/nn_ex/tensor_nn/nn_cpu_ex.py > nn_ex.py && python nn_ex.py
```

Add this(L27) to switch into CPU mode.
```python
# use CPU
os.environ['CUDA_VISIBLE_DEVICES'] = '-1'
```

