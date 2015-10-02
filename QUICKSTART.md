### ECHAM Quick-Start

#### Download source code

* Sign up for a user account on the MPI Users Forum at https://code.zmaw.de/projects/mpi-esm-users
* Sign in and download the latest MPI-ESM__.tar.gz from https://code.zmaw.de/projects/mpi-esm-users/files.
* Copy .tar.gz file to your home directory on fram
* Extract files with `tar -xvf`

#### Compile model
On fram, go to the `src/echam` subdirectory of the extracted `mpiesm-n.n.__` directory and run the
configuration script:
```
module load intel/intel-15
module load netcdf/4.3.2/intel-15
./configure --prefix=/home/jwalker/echambuild CC=icc FC=ifort F77=ifort CXX=icpc
```

Compile the source code:
```
make
```

