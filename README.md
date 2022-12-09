
# Transformer Fault Detector

This ML/AI solution is used in the process of discovering the
presence of a fault in a transformer before it manifests itself in the form of a breakdown. The
fault detection is achieved by training a ML model to first identify if the image given to it is a transformer, followed by taking its thermal images and enabling
the ML to identify any hotspots that can be picked from the thermal images and then reading the metadata to determine if the region of intrest(ROI) is actually beyond
the set threshold which would classify the ROI as a potential fault that would need attention of the transformer to continue working without any glitches.


## Run Locally

- Install dependencies.

```bash
  pip install flirimageextractor
  pip install loguru
  pip install numpy
  pip install pandas
  pip install matplotlib
  pip install tk #ensure 'conda install tk' is run on anaconda command prompt
  pip install pyqt5
  pip install scikit-image
```
- Install pytorch and create pyenv.

```bash
  conda create -n pytorch_env -c pytorch pytorch torchvision
  source activate pytorch_env
  conda install -c pytorch pytorch torchvision
```
- Open cmd prompt.
- Clone the project in cmd prompt.

```bash
  git clone <<your http link in github code button>>
```

- Go to the project directory.

```bash
  cd Transformers-FaultDetector
```
- Open code in any IDE.
- Open CapstoneTrial.ipynb file.
- Run all blocks of code.

## Input Folder
 These folders are used to hav Transformers images that are ed into the ML model for fault detection.
    
    - datasetsVisibleImages : Visible Images of the Transformers.
    - datasetsThermalImages : Thermal Images of th Transformers used to detect hotspots.
    - datasetsGoogleImages  : Google Images for training the model. 

## Output Folder
 These folders hold the image of the Transformers after the spots that are faulty are identified. 
 Clear this folder, before running the model.

    - runs/detect/exp : Contains the Thermal images with the fault hotspots detected.
 


