# ICCAD-2019_Paper-341
## Machine Learning-Based Hotspot Detection: Fallacies, Pitfalls and Marching Orders 

The Datasets and the source code mentioned in the paper are shared in this repository.

### Technical details of the proposed ICCAD-2019 benchmarks
 - Layer Numbers
	  - 0: Extent
	  - 10: Metal polygons
	  - 21: Hotspot core marker
	  - 23: Non-Hotspot core marker
 - Hotspots and Non-Hotspots can be identified in one of the following ways:
	  - Through their corresponding marker layers.
	  - Cellnames: Every pattern in the file has a unique name in the form of a cellname. Hotspot patterns contain the keyword `_hotspot` in their cell names, whereas, Non-Hotspot patterns contain `_nonhotspot`.
	  - Labels: Every pattern contains a text label at its center (in layer 0). The label is same as the cell name.
 - Identifying Truly-Never-Seen-Before (TNSB) hotspots within the Testing Dataset - 1:
	 - A CSV file containing the cell names of TNSB hotspots is included in the same folder as the Testing Dataset - 1. 
### Simple ML-based hotspot detection flow (discussed in section 3 of the paper)
- The source code (Jupyter notebook (Python 2.7)), training and testing datasets, and the pre-trained models are made available.
- Users can either use the pre-trained models or re-train them locally. Instructions to switch between the two modes, to change dataset paths etc., are provided in the main code.
### Source code of State-Of-The-Art (SOTA) methods
- Source code of `DAC'17 [24]` and `TCAD'18 [23]` can be found in [link](https://github.com/phdyang007/dlhsd)
- Source code of `SMACD'18 [1]` can be found in [link](https://github.com/unnir/lithography_hotspot_detection)
- Authors of `VTS'18 [15]` have not publicly released their code yet. It was shared with us privately. Therefore, to obtain the source code of `VTS'18 [15]`, please contact the corresponding authors directly.