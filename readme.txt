Project Title: Enhancing Image Processing through Pretext Learning with Transformation Prediction in Self-Supervised Learning: 
	       A Case Study in Medical Imaging

Project Overview: This project explores a Self-Supervised Learning (SSL) framework leveraging transformation-based pretext tasks 
for classifying retinal diseases using Optical Coherence Tomography (OCT) images. The approach reduces reliance on labeled 
datasets, making it suitable for medical imaging applications.

File Structure: All the following files are included in the source_file.zip archive:

	        readme.txt: Contains project details, instructions to run, and file structure information.

		Notebooks: 01. transform_oct.ipynb: Transformations and preprocessing for the OCT dataset.
			   02. ssl_pretext.ipynb: Implements pretext task training using geometric transformations.
			   03. ssl_downstream.ipynb: Fine-tuning for the downstream classification task.
	   		   04. ssl_evaluation.ipynb: Evaluation metrics and performance analysis.

		Report: CIS-6020_SSL_Pretext_Imaging.pdf: Full project report formatted for IEEE Transactions.

		Additional Files: DME-943690-9.jpeg: Sample image used for Grad-CAM visualization.
				  CIS-6020_SSL_Pretext_Imaging.zip: Contains the LaTeX code and markup exported 
								    from Overleaf, along with all associated images and resources used 
								    for the report.
				         
Dataset: OCT Dataset: Publicly available dataset used for training and evaluation. Link: https://data.mendeley.com/datasets/rscbjbr9sj/3

Libraries: Programming Language: Python 3
	   Libraries: TensorFlow, NumPy, Matplotlib, scikit-learn, OpenCV, zipfile, os, google.colab.drive, PIL (Pillow), shutil, signal

Environment: Tested on Google Colab with NVIDIA Tesla T4 GPU.

Instructions to Run: Ensure the necessary libraries are installed.
		     Open the notebooks in a Jupyter environment or Google Colab.
		     Update any file or dataset paths in the notebooks to match your local or cloud environment 
		     (specially google.colab.drive will not work in any other environment that google colab).
		     Run the notebooks in the following sequence: 01. transform_oct.ipynb
								  02. ssl_pretext.ipynb
								  03. ssl_downstream.ipynb
								  04. ssl_evaluation.ipynb

Contributions: Pretext learning implementation for retinal disease classification.
	       Downstream task fine-tuning with frozen layers for feature generalization.
	       Quantitative and qualitative analysis with Grad-CAM visualization.

Reused Components: Some of the evaluation techniques were adapted from a previous study, based on "Conv-Vit" published in MDPI 
                   (https://www.mdpi.com/2313-433X/9/7/140). The methodology, core implementation, and results discussed in 
                    this project are novel and tailored for this specific framework.

Acknowledgments: This project was completed as part of the CIS*6020: Artificial Intelligence course at the University of Guelph under the 
		 guidance of Professor Neil Bruce. I would like to thank the AI Enabled Medical Imaging Analysis Lab for their support and 
                 resources throughout the work.