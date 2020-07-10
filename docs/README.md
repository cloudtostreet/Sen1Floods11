# **Sen1Floods11 Documentation**

## **Bucket Structure**
Please refer below for a description of each file and folder inside the `cnn_chips` bucket that hosts Sen1Floods11.

### _**Folders**_
___
_**Labeled Data**_

`QC_v2/`: 446 labeled chips of Water/NoWater/NoData.

`S2/`: 446 Sentinel-2 L1C Chips overlapping labeled data.

`S1/`: 446 Sentinel-1 GRD Chips overlapping labeled data.

_"Other" data matching labels_

`Perm/:`: 446 chips of permenent water derived from JRC overlapping labeled data.

`S1Flood/`: 446 chips of water/nowater derived from standard OTSU thresholding of Sentinel-1 VH band overlapping labeled data.

`S2Flood/`: 446 chips of water/nowater derived from standard classification of Sentinel-2 data overlapping labeled data.
___
_**Weak Data**_

`NoQC/`: 4,385 weakly-labeled chips derived from traditional Sentinel-2 Classification.

`S2_NoQC/:`: 4,385 Sentinel-2 L1C chips overlapping weakly-labled data.

`S1_NoQC/:`: 4,385 Sentinel-1 GRD chips overlapping weakly-labeled data.

_"Other" data matching weak labels_

`S1Flood_NoQC/`: 4,385 chips of water/nowater derived from standard OTSU thresholding of Sentinel-1 VH band overlapping weakly-labeled data.
___

### _**Files**_

`Sen1Floods11_labeled.tgz`: _.tgz_ file containing labeled data in QC_v2, S2, & S1

`CNN_Chips_FTC.geojson`: _.geojson_ file containing bounding-box and meta-data for each chip in labeled data (does not contain weakly-labeled data).