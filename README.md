# SSL-with-Transformation-Prediction-based-Pretext-Learning

## Project Overview
This project explores a **Self-Supervised Learning (SSL)** framework leveraging transformation-based pretext tasks for classifying retinal diseases using Optical Coherence Tomography (OCT) images. The approach reduces reliance on labeled datasets, making it suitable for medical imaging applications.

## File Structure

- **Notebooks**:
  - `01.transform_oct.ipynb`: Transformations and preprocessing for the OCT dataset.
  - `02.ssl_pretext.ipynb`: Implements pretext task training using geometric transformations.
  - `03.ssl_downstream.ipynb`: Fine-tuning for the downstream classification task.
  - `04.ssl_evaluation.ipynb`: Evaluation metrics and performance analysis.
- **Report**: `CIS-6020_SSL_Pretext_Imaging.pdf`: Full project report formatted for IEEE Transactions.
- **Additional Files**:
  - `DME-943690-9.jpeg`: Sample image used for Grad-CAM visualization.
  - `CIS-6020_SSL_Pretext_Imaging.zip`: Contains LaTeX code and markup exported from Overleaf, with associated images and resources.

## Dataset
- **OCT Dataset**: Publicly available dataset used for training and evaluation.  
  - Link: [OCT Dataset on Mendeley](https://data.mendeley.com/datasets/rscbjbr9sj/3)

## Libraries
- **Programming Language**: Python 3
- **Key Libraries**: TensorFlow, NumPy, Matplotlib, scikit-learn, OpenCV, zipfile, os, google.colab.drive, PIL (Pillow), shutil, signal.

## Environment
- **Tested on**: Google Colab with NVIDIA Tesla T4 GPU.

## Instructions to Run
1. Ensure the necessary libraries are installed.
2. Open the notebooks in a Jupyter environment or Google Colab.
3. Update file or dataset paths to match your environment (e.g., `google.colab.drive` paths will not work elsewhere).
4. Execute the notebooks in the following sequence:
   - `01.transform_oct.ipynb`
   - `02.ssl_pretext.ipynb`
   - `03.ssl_downstream.ipynb`
   - `04.ssl_evaluation.ipynb`

## Contributions
- Pretext learning implementation for retinal disease classification.
- Downstream task fine-tuning with frozen layers for feature generalization.
- Quantitative and qualitative analysis with Grad-CAM visualization.

## Reused Components
- Some evaluation techniques were adapted from **Conv-Vit** published in MDPI.  
  - Link: [Conv-Vit on MDPI](https://www.mdpi.com/2313-433X/9/7/140)  
  The methodology, core implementation, and results are novel and tailored for this specific framework.

## Reference
This work was presented on The 2025 IGT x ImNO Joint Symposium [Find the abstract here] (https://www.igtximno.ca/wp-content/uploads/ImNO-2025-Proceedings.pdf) [Explore the poster here](https://www.researchgate.net/publication/391459808_Self-Supervised_Learning_for_Retinal_Disease_Classification_Reducing_Annotation_Dependency_with_Transformation-Based_Pretext_Learning_with_Limited_Labels)

If you use this code or model in your research, please cite the abstract to acknowledge the original work.

## Acknowledgments
This project was completed as part of the **CIS*6020: Artificial Intelligence** course at the **University of Guelph** under the guidance of Professor **Neil Bruce**. Thanks to the **AI Enabled Medical Imaging Analysis Lab** for their support and resources throughout this work.

