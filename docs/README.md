# **Sen1Floods11 Documentation**

## **Bucket Structure**
Please refer below for a description of each file and folder inside the `sen1floods11` bucket that hosts Sen1Floods11.
Note that the most recent data is available within the `v1.1` folder.

### _**Folders**_

_**data/flood_events/HandLabeled**_

`LabelHand/`: 446 labeled chips of Water/NoWater/NoData.

`S1Hand/`: 446 Sentinel-1 GRD Chips overlapping labeled data.

`S2Hand/`: 446 Sentinel-2 L1C Chips overlapping labeled data.

`JRCWaterHand/`: 446 chips of permenent water derived from JRC overlapping labeled data.

`S1OtsuLabelHand/`: 446 chips of water/nowater derived from standard OTSU thresholding of Sentinel-1 VH band overlapping labeled data.

_**data/flood_events/WeaklyLabeled**_

`S1OtsuLabelWeak/`: 4,385 chips of water/nowater derived from standard OTSU thresholding of Sentinel-1 VH band overlapping weakly-labeled data.

`S2IndexLabelWeak/`: 4,385 weakly-labeled chips derived from traditional Sentinel-2 Classification.

`S1Weak/`: 4,385 Sentinel-1 GRD chips overlapping weakly-labeled data.

_**data/perm_water**_

`S1Perm/`:

`JRCPerm/`: 

_**splits**_

`flood_handlabeled/`: contains train, test, and validation splits for handlabeled images of floods (see: `data/flood_events/HandLabeled`).

`perm_water/`: contains train, test, and validation splits for permanent water (see: `data/perm_water/`)

### _**Files**_

`CNN_Chips_FTC.geojson`: _.geojson_ file containing bounding-box and meta-data for each chip in labeled data (does not contain weakly-labeled data).