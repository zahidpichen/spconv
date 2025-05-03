# ⚠️ This is for Google colab users only ⚠️

This is a branch from the [traveler59](https://github.com/traveller59) the original maintainer of [spconv repository](https://github.com/traveller59/spconv.git)

this branch was created to solve the version compatability between spconv and cumm as stated in this [issue](https://github.com/traveller59/spconv/issues/726)

I created this branch due to it's simplicity when using [OpenPCDet](https://github.com/open-mmlab/OpenPCDet.git)


# Useage
---

**NOTE** - run this first in order to build spconv and cumm. 
```
import os
os.environ["CUMM_CUDA_ARCH_LIST"] = "7.5"
```
You can get the ARCH list for orin nano, Xavier, etc from the issue mentioned above

1. Clone the required reopsitories
```
!git clone https://github.com/FindDefinition/cumm.git
!git clone https://github.com/zahidpichen/spconv.git
```
2. Go to the folder and do start installation
```
cd cumm
!pip install -e .
```
3. Go back
`cd ..`
4. Now go to spconv folder, start the installation and start the build
```
cd spconv
!pip install -e .
import spconv
```


