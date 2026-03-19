# NEURON-D-25-01766
Code in **'A reciprocal glial circuit calibrates injury information and governs the tissue response balance'**

which includes two parts: 

**1 Analysis code for image data**; 

**2 Analysis code for sequencing data**.

If you have any feedback or issues, you are welcome to either post an issue in the Issues section or send an email to jingmiao@cibr.ac.cn.

## ATP1.0 *in vivo* and *ex vivo* imaging data analysis

### Exemplar data

You can download the Exemplar data [here](https://www.dropbox.com/scl/fi/xkwx2v67kkw809dwqkfqs/ExampleData.tif?rlkey=enpvuiic0je6a5kd24l8pg0ri&st=rl3vuxql&dl=0) 

You can download the project files post signal extraction via [AQuA](https://github.com/yu-lab-vt/AQuA) (*Yizhi Wang et.al nat. neurosci 2019*)  from [here](https://www.dropbox.com/scl/fi/0cm8lg0rokjd7xk63m5kg/ExampleData_AQuA.mat?rlkey=t6c5v52zg4y7dorj7p85yxwfi&st=jm7t0ygl&dl=0).

Options for signal extraction can be downloaded [here](/OptsOfAqua.csv).

### Code 

1. [**Res2DensityMap**](/Res2DensityMap.m): This function accepts an AQUA project file 'res' and outputs a normalized Inflares density map.
2. [**Res2DensityCurve**](/Res2DensityCurve.m): This function accepts an AQUA project file 'res' and outputs a Inflares density curve.
3. [**Res2RoiRegion**](/Res2RoiRegion.m): This function takes an AQUA project file 'res' as input and outputs a two-dimensional ROI of Inflares,  with the ROI color mapping corresponding to the maximum response for the signal.
4. [**Res2FreqPlt**](/Res2FreqPlt.m): This function accepts an AQUA project file 'res' and plots frequency figure.
