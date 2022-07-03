# CUDA exercises

This repository includes code that can be used as starting point to solve exercises of the CINECA Summer School 2022.

Refer to the slides for the description of the exercise.

To prepare your environment on M100 cluster, the `hpc-sdk` module should be loaded. 

To compile and run the source code use the following command line:
```
nvcc -arch=sm_70 -o cuda_code cuda_code.cu -run
```

To run NVIDIA profiler and generate a summary of statistics.  
```
nsys profile --stats=true ./cuda_code 
```

The folder `solutions` contains the modified source code to match exercises' requests. 