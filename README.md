Pairwise
========

Pairwise distance covariance is calculated as the distance between the C-alpha atoms of protein residues for indexes i and j with respect to the average calculated over a trajectory.

Installation
------------

The python dependencies required are:
```bash
pip install Cython matplotlib mdtraj
```
Usage
-----

Compile the `distance.pyx` file as: 
```bash
python setup.py build_ext --inplace
```

The following generates a heatmap plot using data from two separate trajectories:
```bash
python plot_distance_2d.py $WT_DIR/distance_matrix.dat $MUTANT_DIR/distance_matrix.dat
``` 

