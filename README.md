# 1. Project Description

- **Title:** Assessment of consumer response to the Single-Use Plastics Directive
- This project uses data to strengthen the sustainability image of our beverage brand. We consider consumer opinions collected through a national survey and support our communications with high-quality, data-driven insights. The goal is to help consumers connect with and understand our new sustainability measures.  
  In addition, the project includes an analysis of global plastic-pollution data from Our World in Data. These external publicly available datasets provide a broader context and framework which allows for clearer interpretation of the national survey results.

# 2. Features / Capabilities
- **Exploratory Data Analysis (EDA) of the national survey dataset, including:**
  - Data wrangling and cleaning
  - Summary statistics
  - Visualization of key trends and insights
- **Tools to access and analyse public datasets from Our World in Data, including:**
  - API-based downloading/importing of pollution data
  - Visualization of pollution trends over time

# 3. Project Structure
- The repository is organized into the following folders and key files:
  - `eda_pollution_data.ipynb`  
    Notebook for exploratory data analysis of global plastic-pollution data retrieved from Our World in Data.
  - `eda_survey_data.ipynb`  
    Notebook for exploratory data analysis of the national consumer survey (data under embargo).
  - `labels.py`  
    Contains all translated variable labels, value-label dictionaries (sorted by variable name), helper functions that handle mixed data types, and the `translate()` function for converting full dataframes.  
    Import in Jupyter using:  
    ```python
    from labels import translated_labels, variable_labels, map_codes, translate
    ```

# 4. Installation Instructions
- This project requires **Python 3.12**. It is recommended to set up a virtual environment (e.g., using `venv`) to manage dependencies.

# 5. Key Libraries Used
- The project relies on the following Python libraries for data processing, analysis, and visualization:
  - **Data manipulation:** `pandas`, `numpy`
  - **Reading survey files:** `pyreadstat`
  - **Visualization:** `seaborn`, `matplotlib` (colors, patches)
  - **Statistical analysis:** `scipy.stats` (`chi2_contingency`)
  - **Other utilities:** `collections.Counter`  
- These libraries cover everything from cleaning and analysing data to creating advanced plots and statistical tests.
