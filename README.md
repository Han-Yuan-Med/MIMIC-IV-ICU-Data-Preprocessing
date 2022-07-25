## MIMIC-IV-ICU-Data-Preprocessing

- [Aim](#aim)
- [Steps](#steps)
  - [Step (i): Download MIMIC-IV raw ICU data](#step-i-download-mimic-iv-raw-icu-data)
  - [Step (ii): Download this respiratory](#step-ii-download-this-respiratory)
  - [Step (iii): Run the preprocessing pipeline](#step-iii-run-the-preprocessing-pipeline)
  - [Step (iv): Check generated csv file](#step-iv-check-generated-csv-file)
- [Citation](#citation)
- [Contact](#contact)

## Aim
Larger-scale open-access medical datasets facilitate various research on discovering potential medical evidences, formulating novel medication and treatment plan, and supporting other decision-making via SOTA techniques. `MIMIC` series are the most popular benchamrk datasets, which provided critical care data for over 40,000 patients admitted to intensive care units (`ICU`) at the Beth Israel Deaconess Medical Center. As the latest verison of `MIMIC` family, `MIMIC-IV` highlights data provenance and facilitates both individual and combined use of disparate data sources. However, the information provided by `MIMIC-IV` is in separted `csv.gz` files, which requires certain time and expertise to preprocess and clean. This respiratory aims to prepare a static tabular dataset for `mortality` or `survival time` prediction in ICU. The input features contain `demographics`, XXX, etc. The pipeline processes the raw data downloaded from PhysioNet to a structured, outlier removed, missing imputed, and well-labelled data.

## Steps
### Step (i): Download MIMIC-IV raw ICU data
Follow the instructions on https://physionet.org/content/mimiciv/1.0/ to obtain access to MIMIC-IV 1.0 version

Click `Download the ZIP file` button

Check `mimic-iv-1.0.zip` in PC `Downloads` folder

![alt text](https://github.com/Han-Yuan-Med/MIMIC-IV-ICU-Data-Preprocessing/blob/main/Picture1.png)

### Step (ii): Download this respiratory
Click `Download ZIP button`

Check the `MIMIC-IV-ICU-Data-Preprocessing-main.zip` in PC `Downloads` folder

Unfold `MIMIC-IV-ICU-Data-Preprocessing-main.zip`

Unfold `mimic-iv-1.0.zip` to the same folder of `MIMIC-IV-ICU-Data-Preprocessing-main`

![alt text](https://github.com/Han-Yuan-Med/MIMIC-IV-ICU-Data-Preprocessing/blob/main/Picture2.png)

### Step (iii): Run the preprocessing pipeline
Open `MIMIC Preprocess` python script and run the code step by step

### Step (iv): Check generated csv file
Final processed data `MIMIC-IV-ICU.csv` is stored under the same folder of `MIMIC-IV-ICU-Data-Preprocessing-main`

A short description on the final data:

Input features

Output labels

Finally Done!!! You can explore various models for binary prediction using the `mortality` label and different methods for survival prediction using the `survival time` label. Using the data cleaned by this respiratory, we show how to self-distillate an interpretable clinical score table from black-box neural networks in this [paper]().

<p align="center">
  <img src="https://github.com/Han-Yuan-Med/MIMIC-IV-ICU-Data-Preprocessing/blob/main/dance-spongebob.gif" />
</p>


## Citation
If you use MIMIC-IV Preprocessing in a scientific publication, we would appreciate citations to the following paper.

Yuan H, Ahmed A, Kang L, Miao C, Wu Y. An empirical study of the effect of background data size on the stability of SHapley Additive exPlanations (SHAP) for deep learning models. arXiv. 2022. https:XXX.

## Contact
- Han Yuan (Email: <yuanhannku@163.com>)
