# Hack or Hammer: Can Neural Networks Classify Stellar Types? ☀️🔨

Repository files:
- `final_project.ipynb`: Main Jupyter notebook containing full analysis, model training, hyperparameter tuning, and results evaluations.
- `final_project_functions.ipynb`: Contains the customized `plot_confusion_matrix` function. 
- `SDSS.csv`: Input dataset containing photometric and stellar parameter information from SDSS.
- `Astro416_WIP_Talk_Yanbo.pdf`: Work in progress presentation.

The scientific goal of this project is to use neural networks to classify stars into different spectral classes based on features like magnitude, colors, effective temperature, metallicity, etc. A neural network was trained using cross-validation and hyperparameter tuning via Keras Tuner. The final model achieves good classification performance. The final architecture features multiple hidden layers, dropout regularization, and a softmax output layer (more discussion can be found in the reflection section). 

Dataset:
The dataset used (SDSS.csv) includes the following features:
- Photometric magnitudes: `u`, `g`, `r`, `i`, `z`
- Dereddened magnitudes: `dered_u`, `dered_g`, `dered_r`, `dered_i`, `dered_z`
- Physical parameters: `elodieTEff`, `elodieLogG`, `elodieFeH`
- Spectral label from ELODIE: `elodieSpType`


How to reproduce:
- `git clone https://github.com/yanbopanastro/UM-Astro-416-final-project.git`
- Install dependencies: `pip install numpy pandas scikit-learn tensorflow keras keras-tuner matplotlib`

<img src="https://github.com/user-attachments/assets/41b9fb49-fd25-45c0-9f8a-4661adb613d8" width="500"/>
