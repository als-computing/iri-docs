# ALS IRI Demonstration Project
Th Advanced LightSource (ALS) is embarking on a project to demonstrate capabilities in line with with the DOE's [Integrated Research Infrastructure](https://science.osti.gov/-/media/ascr/ascac/pdf/meetings/202306/Brown_IRI_ASCAC_2023206.pdf) (IRI) initiative. The IRI is currently creating test beds at compute facilities for demonstrating close collaboration with DOE scientific facilities.

The ALS has chosen a use case that shows significant integrations between beamlines and compute facilities. This project will demonstrate feasibility of using the ASCR Compute Facilities for workloads that add significant value to the beamline user experience. We endeaver to run the same use case using NERSC, ALCF, OLCF and the ESNet Test Bed.

See also:
* Project [Requirements](docs/requirements.md)
* Project [Design](docs/design.md)

## Use Case: Tomography Reconstruction and Segmentation

A user at the ALS microCT beamline 8.3.2 will launch a scan, perform a tomographic reconstruction and segment the resulting reconstruction, all from a web browser at their beamline.
* When the scan is complete, the data is copied to the ASCR facility.
* The raw scan data is registered in the ALS SciCat instance.
* The user opens a web browser and launch a jupyter notebook, hosted at the ASCR facility. The user will use this noetbook to perform a tomography reconstruction.
* The reconstructed data set is registered in the ALS SciCat instance, associated with the raw data set.
* The user will open the MLExchange Segmentation application and train a network to segement frames.
* [TBD] what happens to the segmentation result?

