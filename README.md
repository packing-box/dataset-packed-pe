# Dataset of packed PE files

This is a fork of the dataset at [https://github.com/chesvectain/PackingData](https://github.com/chesvectain/PackingData) with some samples sanitized (e.g. UPX-packed samples in the ´not-packed´ folder or samples with a same hash from the packer and `not-packed` folders).

It also includes a folder named `outliers` containing samples we could identify as potentially disturbing our models, i.e. when they were sorted among the not packed samples while demonstrating characteristics of packed data. This dataset can be used for training machine learning models tailored to PE executable packing.

Folder `labels` contains a [Python script](labels/generate-category-labels.py) for generating labels based on the packer categories mentioned in the table of [`packed` folder's `README.md`](packed/README.md) with the resulting JSON dictionaries.


## :star: Related Projects

You may also like these:

- [Awesome Executable Packing](https://github.com/packing-box/awesome-executable-packing): A curated list of awesome resources related to executable packing.
- [Bintropy](https://github.com/packing-box/bintropy): Analysis tool for estimating the likelihood that a binary contains compressed or encrypted bytes (inspired from [this paper](https://ieeexplore.ieee.org/document/4140989)).
- [Dataset of packed ELF files](https://github.com/packing-box/dataset-packed-elf): Dataset of ELF samples packed with many different packers.
- [Docker Packing Box](https://github.com/packing-box/docker-packing-box): Docker image gathering packers and tools for making datasets of packed executables.
- [DSFF](https://github.com/packing-box/python-dsff): Library implementing the DataSet File Format (DSFF).
- [PEiD](https://github.com/packing-box/peid): Python implementation of the well-known Packed Executable iDentifier ([PEiD](https://www.aldeid.com/wiki/PEiD)).
- [PyPackerDetect](https://github.com/packing-box/pypackerdetect): Packing detection tool for PE files (fork of [this repository](https://github.com/cylance/PyPackerDetect)).
- [REMINDer](https://github.com/packing-box/reminder): Packing detector using a simple heuristic (inspired from [this paper](https://ieeexplore.ieee.org/document/5404211)).

Example of visualization created with [Bintropy](https://github.com/packing-box/bintropy):

<p align="center"><img src="https://raw.githubusercontent.com/packing-box/docker-packing-box/main/docs/pages/imgs/calc.png"></p>

