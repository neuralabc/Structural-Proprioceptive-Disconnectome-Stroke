# Patterns of Structural Disconnection Driving Proprioceptive Deficits in Chronic Stroke

This repository contains all data, analysis scripts, and derived results required to reproduce the analyses reported in our publication examining the relationship between white matter disconnection patterns and proprioceptive impairment following chronic sensorimotor stroke.

The repository is organized to support transparency, reproducibility, and reuse by both clinical and computational neuroscience researchers.

---

## Repository Structure

```
├── Disconnectomes/
├── Regression-Results-Images/
├── Scripts/
│   ├── APM_VGR_FMUL_correlations.ipynb
│   └── APMregression_covVGRAgeSex_MNI_5000perms.ipynb
├── Demographic-and-Behavioural-Data.csv
├── environmentrequirements.txt

```

---

## Folder and File Descriptions


### `Disconnectomes/`

Contains voxel-wise white matter disconnection maps generated for each participant using the tractography-based lesion assessment standard (TractLAS). These maps constitute the primary neuroanatomical predictors in the analyses.

### `Regression-Results-Images/`

Contains visual outputs derived from permutation-based regression analyses, including statistical maps used in the manuscript and supplementary materials.

### `Scripts/`

Contains Jupyter notebooks implementing all statistical analyses reported in the manuscript.

* **`APM_VGR_FMUL_correlations.ipynb`**
  Computes correlations between proprioceptive performance (Arm Position Matching; APM), motor performance (Visually Guided Reaching; VGR), and clinical measures (FM-UL) to characterize behavioural relationships.

* **`APMregression_covVGRAgeSex_MNI_5000perms.ipynb`**
  Performs voxel-wise regression analyses relating white matter disconnection to proprioceptive impairment while controlling for motor impairment, age, and sex. Statistical significance is assessed using nonparametric permutation testing (5,000 permutations) in MNI space.

### `Demographic-and-Behavioural-Data.csv`

Contains anonymized demographic and behavioural measures used in the analyses, including proprioceptive and motor task scores. These data serve as inputs for all statistical analyses.

### `environmentrequirements.txt`

Specifies the Python environment and package dependencies required to run the analysis scripts and reproduce the results reported in the manuscript.

---

## Analysis Environment

All analyses were conducted in Python. To recreate the analysis environment, install the required dependencies using:

```bash
pip install -r environmentrequirements.txt
```

The provided Jupyter notebooks are intended to be run using this environment. File paths within the notebooks reflect the original analysis setup and will need to be updated by users to match their own local file system when reproducing the analyses.

---

## Data Availability and Ethics

All shared data have been anonymized and are distributed in accordance with institutional ethical approvals and data-sharing agreements. No personally identifiable information is included in this repository. Raw neuroimaging data cannot be shared due to the ethical requirements of the University of Leipzig Ethics Committee.

---

## Citation

If you use this code or data, please cite the following publication:

Kaeja M, Iturria-Medina Y, Villringer A, Sehm B, Steele C.
*Patterns of Structural Disconnection Driving Proprioceptive Deficits in Chronic Stroke.*
**Stroke**. 2025. doi:10.1161/STROKEAHA.125.052266

---

## Contact
For questions regarding the data, analyses, or reuse of this repository, please contact: <a href="mailto:mika&#46;kaeja&#64;mail&#46;concordia&#46;ca">Mika Kaeja </a>
