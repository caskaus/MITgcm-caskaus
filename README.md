[![Build Status](https://github.com/MITgcm/MITgcm/workflows/build/badge.svg)](https://github.com/MITgcm/MITgcm/actions)
[![Documentation Status](http://readthedocs.org/projects/mitgcm/badge/?version=latest)](http://mitgcm.readthedocs.io/en/latest/?badge=latest)
[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.1409237.svg)](https://doi.org/10.5281/zenodo.1409237)

# MITgcm

MIT General Circulation Model master code and documentation. The main MITgcm webpage can be found [here](http://mitgcm.org).

## Documentation

Access the latest documentation [here](http://mitgcm.readthedocs.io/en/latest/)

## Running the trial case tutorial_global_oce_latlon

```
cd /scratch/ds2/km7623/MITgcm/verification/tutorial_global_oce_latlon
cp -r /scratch/ds2/km7623/MITgcm/modules.sh .
source modules.sh
```

```
../../../tools/genmake2 -mods ../code -optfile /scratch/ds2/km7623/MITgcm/tools/build_options/linux_amd64_ifort_gadi
```

```
make depend
```

```
make
```
After make is done successfully, you will end up with an executable ```mitgcmuv``` in the ```/build``` directory
