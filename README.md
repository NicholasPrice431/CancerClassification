Overview
------

This is the final project for COP4630. This project trains and employs a CNN (ResNet50) to automatically detect a variety of cancers in processed CT scans. The cancer varieties are as follows:
- all pro
- all benign
- all early
- all pre
- brain menin
- brain glioma
- brain tumor
- breast benign
- breast malignant
- oral normal
- oral scc
- kidney tumor
- kidney normal
- lymph fl
- lymph cll
- lymph mcl
- lymph koc
- cervix sfi
- cervix dyk
- cervix pab
- cervic mep
- lung scc
- lung bnt
- colon bnt
- colon aca
- lung aca

Dependencies
------
torch

torchvision

torchaudio

numpy

pandas

pillow

scikit-learn

seaborn

matplotlib

tqdm

gitpython

nbformat

kagglehub

Implementation
  ----

Download the 4630_Final_005 .ipynb file. That file is the back-end code and is used for training the model and acquiring model metrics.
The model was created using the T4 GPU on colab. This considerably cuts down on training time assuming your system is not better.
When running, make sure your file paths match the file paths in the code. If not, edit your paths to match your system. If you'd like to skip the training, download the latest checkpoint from the checkpoint
folder and start at the cell titled "Model Initialization".

To run the Cancer Image Classifier, create a new folder (for example, cancer_classifier) and open it in your IDE. Inside that folder, create app.py, cancer_model.py, and classes.json, then paste the provided code into each file and place your model checkpoint (e.g., best_model_epoch5.pt) in the same folder. Open a terminal, navigate to this folder with cd "path/to/cancer_classifier", and install dependencies using pip install -r requirements.txt or pip install flask torch torchvision pillow. Once that’s done, start the app by running python app.py, then open a browser and go to http://127.0.0.1:5000/ to upload an image and see the model’s cancer subtype prediction and probabilities.

  

