# The UroCell Dataset
The repository contains the UroCell dataset - an **annotated volumetric dataset of intracellular compartments** obtained with focus ion beam and scaning electron microscopy (FIB-SEM). 

### Procedure
We obtained tissue samples from urinary bladders of 6-8 weeks old healthy male C57BL/6J mice in accordance with European guidelines and Slovenian legislation. The experiments were approved by the Veterinary Administration of the Slovenian Ministry of Agriculture and Forestry (permit no. U34401-6/2015/4) in compliance with the Animal Health Protection Act and the Instructions for Granting Permits for Animal Experimentation for Scientific Purposes. 
The volumetric data were obtained from the tissue with a FIB-SEM dual beam electron microscope. Briefly, urinary bladders were isolated and immediately cryo-fixed with a CPC device (Leica), freeze-substituted in AFS (Leica) with 2% OsO4 in acetone, and embedded in Epon. To locate the region of interest, which were terminally differentiated cells of the bladder epithelium (umbrella cells), Epon ultrathin sections were inspected with the Philips CM100 transmission electron microscope and the location of cells was correlated with their location in the epon block. The epon block was then taken into a dual beam Helios NanoLab 650 microscope (FEI) and the umbrella cell was sectioned with the FIB. 

The dimensions of of each pixel were x=5.49 nm, y=5.49 nm, z=15.0 nm. We binned x and y pixels by 3 to obtain an almost isotropic resolution in all three directions which resulted in 1056 serial sections of 1366x1180 pixels. The voxel dimensions in the dataset are thus approximately x=16 nm, y=16 nm, z=15 nm. 

### Annotations

The dataset contains 5 annotated sub-volumes of 256x256x256 voxels. Currently, two intracellular compartment types are annotated: mitochondria and endolysosomes. All annotations were revised by biomedical experts. We will add other compartment types in the future.

### Dataset structure

The dataset is structured into three folders, each containing five 256x256x256 sub-volumes. The files are stored in the gzipped Neuroimaging Informatics Technology Initiative (NIfTI) volumetric file format.

* *data*: contains the original FIB-SEM scanned data
* *mito*: contains manual annotations of mitochondria
* *lyso*: contains manual annotations of endolysosomes

### Cite us
Please cite our [paper](https://doi.org/10.1016/j.compbiomed.2020.103693) if you use this dataset. 

### Acknowledgements
The dataset is published under the [CC-BY-NC-SA 4.0 licence](https://creativecommons.org/licenses/by-nc-sa/4.0/legalcode). Feel free to use it for your research with necessary attributions. 
