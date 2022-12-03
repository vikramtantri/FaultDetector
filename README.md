
# Transformer Fault Detector

This ML/AI solution is used in the process of discovering the
presence of a fault in a transformer before it manifests itself in the form of a breakdown. The
fault detection is achieved by training a ML model to first identify if the image given to it is a transformer, followed by taking its thermal images and enabling
the ML to identify any hotspots that can be picked from the thermal images and then reading the metadata to determine if the region of intrest(ROI) is actually beyond
the set threshold which would classify the ROI as a potential fault that would need attention of the transformer to continue working without any glitches.
## Run Locally

Install dependencies

```bash
  pip install flirimageextractor
  pip install loguru
  pip install numpy
  pip install pandas
  pip install matplotlib
  pip install PyQt5
  pip install tk #ensure 'conda install tk' is run on anaconda command prompt
```
