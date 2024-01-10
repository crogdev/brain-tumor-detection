
# Project Title

This repository contains 2 projects.


### brain-tumor-detection-1

Dataset: https://www.kaggle.com/datasets/navoneel/brain-mri-images-for-brain-tumor-detection (8.27 MB)

Code: https://github.com/MohamedAliHabib/Brain-Tumor-Detection

[Info: It will take about 1-2 hours to train model in this]


### brain-tumor-detection-2
Dataset: https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri (44.3 MB)

Code: https://github.com/akd6203/brain-tumor-detection

[Info: It will take about 2-5 min to train model in this]

## Run:
Both projects can be run using same conda environment

[Info: Use cmd, not powershell if on windows]

Step 1: Download Anaconda/Miniconda. https://docs.conda.io/projects/miniconda/en/latest/

Step 2: conda env create -n braint -f environment.yml

Step 3: jupyter-notebook

Done



---
---
---
---
---

### Misc snippets to save/load model locally:

#### Save
from tensorflow.keras.models import save_model

model.compile(optimizer='adam', loss='binary_crossentropy', metrics=['accuracy'])

model.fit(x=X_train, y=y_train, batch_size=32, epochs=50, validation_data=(X_val, y_val))

model.save('your_model.h5')

#### Load
from tensorflow.keras.models import load_model

model = load_model('your_model.h5')




