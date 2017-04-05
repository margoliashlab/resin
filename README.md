# Resin
Resin is a spectral analysis toolbox for Python inspired by [SAP](http://soundanalysispro.com/).

## Requirements
+ Python 2.7+
+ Numpy

Optional Requirements
+ Scipy
+ Matplotlib

## Installation

```bash
git clone https://github.com/kylerbrown/resin
cd resin
pip install .
```
## Usage example

```python
from resin import Spectra
spec = Spectra(rate=30000, 
		NFFT=512,
		data_window=500,
		noverlap=412,
		n_tapers=4,
		freq_range=(300, 90000))
spec.signal(data)
spec.spectrogram()
```

![Example spectrogram](spectrogram_example.png)

## Authors

Mike Lusignan wrote `segmentation` as part of his PhD thesis. Details of the algorithms can be found in: 
Lusignan, M. E. University of Chicago. (2012). [_Growing up singing: Behavioral and physiological perspectives on song acquisition_]( http://pi.lib.uchicago.edu/1001/cat/bib/9370223).

Resin is a fork of `segmentation`, writen by Kyler Brown, 2017.

