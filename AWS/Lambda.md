#### Lambda Server-less architecture 
Lambda Function runs on ```EC2```, now using ```Firecracker```.

```Firecracker``` is a lightweight, customizable VM that builds on ```Kernel-based Virtual Machine```.

Before ```Firecracker```, Lambda requests an EC2 instance every time a job runs. 2 Problems:
1. Waste of resources. e.g. launched instances have fixed amount of CPU/ RAM like ```3GB```, but the lambda function only has ```128MB```
2. Dependent on EC2

###VM vs. Container
In this case, VM has better security boundary. Instances of VM cannot communicate. 
