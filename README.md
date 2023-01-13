# Toy Data Test
toy data test for evaluation of EDMD online

## detail
1. EDMD part
2. EDMD online part

### EDMD part
+ standard EDMD
+ preparation for EDMD online part

### EDMD online part
+ update time evoluetion mapping on feature space
+ the initial mapping on feature space is determined in standard EDMD

### data definition
![data_definition](./images/edmd_online.jpeg)

## File Structure
```
.
├── create_toy_data.m
├── data
│  ├── result
│  │  └── linear_time_variant.mat
│  └── toy_data
│     └── linear_time_variant.mat
├── DICTOL                                            //csc library
├── edmd_online
│  ├── dmd.m
│  ├── mat_to_mat_tilde.m
│  ├── mat_to_vec_check.m
│  ├── next_mat_K.m
│  └── projection_onto_range_mat.m
├── images
│  ├── algorithm.jpeg
│  ├── edmd_online.jpeg
│  ├── linear_time_variant_trajectory.jpg
│  └── linear_time_variant_transition.jpg
├── main.m
├── plot.m
├── README.md
├── SymConfig.m
├── test.m
├── time_evolution
│  └── linear_time_variant.m
└── util_plot
   ├── error_transition.m
   └── rsme.m
```

<!-- + main.m: main file for toy data test
+ util: utility function defined on this directory
    + dmd.m: dynamic mode decomposition
    + time_evolutions2d.m: define time evolution function on state space
    + mat_to_mat_tilde.m: convert matrix to matrix tilde (big matrix)
    + mat_to_vec_check.m: convert matrix to vector
+ images: images directory
+ archive: archive directory using nonlinear mapping(state space <-> feature space)
    + utility functions for _main.m
        + nonlinear_mapping.m: define nonlinear mappnig from state space to feature space
        + nonlinear_mapping_inv.m: define nonlinear mapping from feature space to state space
        + time_evolution.m: define time evolution function on state space
+ plot: functions defined for plot
    + error_transition.m: return rsme corresponding to iteration
    + rsme.m: define rsme(root square mean eror) between 2 matrices
+ DCTORL: csc library -->

+ detail later...

## csc
+ convolutional sparse coded(dictionary learning)
+ D(Dictionary): mapping from feature space to state space

## DICTOL
* [githb link](https://github.com/tiepvupsu/DICTOL)