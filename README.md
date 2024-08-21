# AustLII Legal Case Report

## Overview

**Keywords**: Australian law; Legal cases; Federal court of Australia

This dataset contains all **Australian legal cases** from the [Federal Court of Australia (FCA)](https://www.fedcourt.gov.au) during **2006 - 2009**, a **textual corpus** of **4000 legal cases** for automatic summarisation and citation analysis downloaded from [AustLII](https://www.austlii.edu.au/).

For each document, the dataset collected **catchphrases**, **citation sentences**, **citation catchphrases**, and **citation classes**:

- **Catchphrases** are found in the document. The dataset uses the catchphrases as the gold standard for the summarisation experiments.
- **Citation sentences** are found in later cases that cite the present case. The dataset uses citation sentences for summarization. 
- **Citation catchphrases** are the catchphrases (where available) of both later cases that cite the present case, and older cases cited by the present case.
- **Citation classes** are indicated in the document. They indicate the type of treatment given to the cases cited by the present case.


## Data Source
The original data is downloaded from [AustLII](https://www.austlii.edu.au/) and licensed with [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/deed.en). You can also find it from [UCI Machine Learning Repository - Legal Case Reports](https://archive.ics.uci.edu/dataset/239/legal+case+reports) and [Kaggle - Legal Case Reports in Australia](https://www.kaggle.com/datasets/thedevastator/legal-case-reports-in-australia-2006-2009?select=06_1041.xml).


## Dataset Structure

Under `AustLII-Legal-Case-Reports`, after unzipping `legal_case_reports.zip`, the dataset  `corpus` contains:
- `readme.txt`: An overview of the dataset.
- `citations_class`: 2754 `.xml` files that contain citation class elements for each case.
- `citations_summ`: 3891 `.xml` files that contain citation elements for each case.
- `fulltext`: 3890 `.xml` files that contain full text and the catchphrases of all the cases from the [FCA](https://www.fedcourt.gov.au).


## Download

You can download the dataset directly from [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Legal+Case+Reports) or [Kaggle](https://www.kaggle.com/datasets/thedevastator/legal-case-reports-in-australia-2006-2009?select=06_1041.xml). Or, you can download the dataset by using `curl` through your terminal:
```sh
source utils/download.sh [<save_path>]
```
If `<save_path>` is not provided, `legal_case_reports.zip` will be downloaded to the current directory.


## License

This repository is licensed under [MIT](https://opensource.org/license/mit).