# Semester Project Description
## Completion requirements
### Overview:

This project involves working with datasets to train models and make predictions as part of a Kaggle competition. You will use the provided data to analyze, train, and tune your models, then generate predictions for a test dataset, which will be evaluated via a Kaggle competition.

Background, Motivation:

"Context Infrastructure-as-code (IaC) is the DevOps strategy that allows management and provisioning of infrastructure through the definition of machine-readable files and automation around them, rather than physical hardware configuration or interactive configuration tools. On the one hand, although IaC represents an ever-increasing widely adopted practice nowadays, still little is known concerning how to best maintain, speedily evolve, and continuously improve the code behind the IaC strategy in a measurable fashion. On the other hand, source code measurements are often computed and analyzed to evaluate the different quality aspects of the software developed. In particular, Infrastructure-as-Code is simply "code", as such it is prone to defects as any other programming languages. This dataset targets the YAML-based Ansible language to devise defects prediction approaches for IaC based on Machine-learning.

The dataset contains metrics extracted from 86 open-source GitHub repositories based on the Ansible language that satisfied the following criteria: The repository has at least one push event to its master branch in the last six months; The repository has at least 2 releases; At least 11 of the files in the repository are IaC scripts; The repository has at least 2 core contributors; The repository has evidence of continuous integration practice, such as the presence of a .travis.yaml file; The repository has a comments ratio of at least 0.2; The repository has commit frequency of at least 2 per month on average; The repository has an issue frequency of at least 0.023 events per month on average; The repository has evidence of a license, such as the presence of a LICENSE.md file The repository has at least 190 source lines of code.

Metrics are grouped into three categories: IaC-oriented: metrics of structural properties derived from the source code of infrastructure scripts; Delta: metrics that capture the amount of change in a file between two successive releases, collected for each IaC-oriented metric; Process: metrics that capture aspects of the development process rather than aspects about the code itself.

Inspiration What source code properties and properties about the development process are good predictors of defects in Infrastructure-as-Code scripts?"

Acknowledgement: OpenML.org repository, Elif Ceren Gok.

### Available Files on Moodle:

X_train.csv: Features for training, tuning, and validating your models locally.

y_train.csv: Target values corresponding to X_train.csv for model training, tuning, and validation.

X_test.csv: Features for which you will make predictions to upload in the Kaggle competition.

y_baseline.csv: Baseline predictions for X_test.csv using a simple model; this file serves as a reference for the format you must use when uploading predictions to Kaggle.

### Project Tasks:

- Train and tune your model using the training data (X_train and y_train).
- Make predictions for the test dataset (X_test).
- Upload your predictions to the Kaggle competition.
- Analyze and describe the provided datasets.

### Rules:

Use pc_X_train.csv and pc_y_train.csv for training, selecting, and tuning your model.
Upload your predictions for pc_X_test.csv to the private Kaggle competition.
An example solution (y_baseline.csv) is provided to help you format your submission correctly.
The evaluation metric is Balanced Accuracy Score.
You may submit up to 2 times per day.
Kaggle uses a split test set: part public (for real-time leaderboard evaluation) and part private (for final evaluation after the competition).

### Important Notes:

External Code & Ideas: If you use any external code or ideas (e.g., from public competitions), they must be clearly stated and referenced.
External Datasets: You may only use the datasets provided by the course. Using external datasets -- even for internal investigations --  will invalidate your project and result in failure to receive a "signature" in Neptun.
Generative AI: If you use generative AI for any aspect of your work (coding, documentation, etc.), you must clearly state this in your report. Include the exact prompts used, and provide this information in an appendix, which will not count towards the required page count.

### Submission Deadline and Requirements:

Deadline: December 14th, 11:59 PM (local time).
Report Length: Minimum 10 pages.
Expected Deliverables:

### Report (PDF format):

Name your file as: SURNAME_NEPTUNCODE.pdf.
The report should include a detailed analysis of your modeling process, without repeating general algorithm descriptions from lectures. If you use algorithms not covered, provide a brief description and reference literature.
Include your Kaggle username on the title page (unless it's your real name).

### Jupyter Notebooks:

Name each file as SURNAME_NEPTUNCODE_xxx.ipynb, where xxx describes its content (e.g., SURNAME_NEPTUNCODE_dataexploration.ipynb).
Ensure that the notebooks contain all output and can be run independently.
Document all parameter settings and model configurations used, ensuring the results are reproducible.
Fix and document any random seeds used in your algorithms.
### General Guidelines:

Include exploratory data analysis, preprocessing steps, details of the algorithms used, model tuning, and a summary of your model’s performance.

Discuss the number of algorithms/variations you tested, your tuning process, and the results.

Simplicity and interpretability of models are valued; "white-box" models are preferred if they don't compromise performance.

Focus on both the performance and the elegance of your solution.

### Evaluation Criteria:

- Modeling Effort: Variety of algorithms, experiments, and parameter tuning.
- Report Quality: Should include data exploration, preprocessing, model selection, tuning, and conclusions.
- Prediction Performance: Based on the final Kaggle leaderboard results.
- Model Elegance: Preference for simpler, interpretable models if performance remains competitive.
- scikit-learn, xgboost, pandas, numpy, matplotlib, seaborn