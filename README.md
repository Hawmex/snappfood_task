# SnapFood Data Cleaning Challenge

This repository contains the materials for the SnapFood Data Cleaning Challenge, an interview task completed by Hamed Araab. The project focuses on cleaning and analyzing a dataset of dining establishments in Ahvaz, Iran, and presenting insights through visualizations and a grading system.

## Repository Contents

- **presentation.pdf**: A slide deck summarizing the data cleaning process, grading system, data visualization, and key insights derived from the analysis.
- **task_report.ipynb**: A Jupyter Notebook detailing the data preprocessing steps, including code for data cleaning, normalization, and visualization, along with a grading system implementation using clustering.

## Project Overview

The SnapFood Data Cleaning Challenge involves processing a dataset of dining establishments, ensuring data integrity, and deriving meaningful insights. The key objectives are:

1. **Data Cleaning**:

   - Remove leading/trailing whitespace from string columns.
   - Check for and ensure no duplicate restaurant names.
   - Normalize `Rate`, `Review`, and `Phone` columns, converting Persian digits and formats to standard English formats.
   - Remove rows with missing values.

2. **Grading System**:

   - Implement a 3-means clustering model based on `Rate` and `Review` features.
   - Assign grades (A, B, C, or Unrated) to establishments based on cluster proximity and specific conditions (e.g., `Rate = 0` results in "Unrated").

3. **Data Visualization**:

   - Generate visual insights, including:
     - Proportion of Super Type and Grade categories.
     - Grade distribution by Marketing Area and Super Type.
     - Super Type and Subtype distribution by Marketing Area.

4. **Data Analysis Insights**:
   - Highlight key findings, such as the dominance of restaurants (58.7% of Super Type), concentration in areas like 1-Kianpars and 15-AkharAsfalt, and a significant number of unrated establishments.

## Prerequisites

To run the Jupyter Notebook (`task_report.ipynb`), you need the following Python libraries:

- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `phonenumbers`
- `arabic_reshaper`
- `bidi`
- `scikit-learn`

Install these dependencies using:

```bash
pip install numpy pandas matplotlib seaborn phonenumbers arabic_reshaper python-bidi scikit-learn
```

## Usage

1. **Clone the Repository**:

   ```bash
   git clone <repository-url>
   cd <repository-directory>
   ```

2. **Run the Jupyter Notebook**:

   ```bash
   jupyter notebook task_report.ipynb
   ```

   The notebook is self-contained and includes:

   - Data loading and preprocessing steps.
   - Code for normalizing `Rate`, `Review`, and `Phone` columns.
   - Implementation of the grading system using K-Means clustering.
   - Visualizations of data distributions and insights.

3. **View the Presentation**:
   Open `presentation.pdf` to review the summarized findings, including objectives, data cleaning steps, grading methodology, and visualized insights.

## Key Insights

- **Market Dominance**: Restaurants dominate the dataset (58.7%), with 1-Kianpars and 15-AkharAsfalt being key areas.
- **Grade Distribution**: A significant portion of establishments are unrated (21.7%), indicating potential for increased customer engagement or data collection.
- **Subtype Trends**: The "traditional" subtype is prevalent among restaurants, while "unspecified" is common in catering services.
- **Opportunities**: The high number of unrated establishments suggests opportunities for further data collection or customer feedback initiatives.

## License

This project is for demonstration purposes as part of an interview task and is not licensed for public use.
