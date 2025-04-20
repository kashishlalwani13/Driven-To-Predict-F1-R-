# 🏎️ Driven to Predict: Racing Meets Statistics

This R‑based project analyzes Formula 1 data (2019–2024). Key tools and packages include dplyr, ggplot2, xgboost, cluster, and binom. The repository contains all R scripts (and/or RMarkdown), the final PDF report, and the raw CSV datasets needed to reproduce every analysis and visualization.

This R-based project analyzes Formula 1 data using statistical modeling, clustering, and machine learning to explore three key questions:

1. **Can we predict per-lap times for drivers based on race, track, and team features?**  
2. **Can we identify unique racing styles using k-means clustering on lap and pit data?**  
3. **How much does starting position influence race outcomes statistically?**


## 📥 Data

We use the “Formula 1 World Championship 1950–2020” dataset by **Rohan Rao** from Kaggle.

- 📦 Dataset: [Kaggle link](https://www.kaggle.com/datasets/rohanrao/formula-1-world-championship-1950-2020)

> ⚠️ **Note:** This dataset is used under its original license for academic/research purposes only.  
> We do **not** claim ownership or redistribute the data. All credits go to the original author.

To download the dataset locally (requires [Kaggle CLI](https://github.com/Kaggle/kaggle-api)):

```bash
kaggle datasets download rohanrao/formula-1-world-championship-1950-2020 \
  -p data/raw --unzip
```

📦 Installation

In R, install the required packages:
```{r}
install.packages(c(
  "here", "dplyr", "tidyr", "lubridate", "caret", "xgboost", "Matrix",
  "ggplot2", "ggthemes", "cowplot", "cluster", "factoextra",
  "knitr", "kableExtra", "vcd", "binom", "readr"
))
```

👥 Authors

Kashish Deepak Lalwani
Shubham Kishore Kale
Parth Satish Chavan
Naman Deep

📄 License

This project’s code is under the MIT License.
Dataset is not ours and is credited to its creator, Rohan Rao (Kaggle).
