# **Applied Statistics: 

This repository contains two Jupyter notebooks. The first notebook, titled **`project.ipynb`**, performs statistical analysis on the well-known **PlantGrowth** dataset. The notebook applies **t-test** and **ANOVA** methods to evaluate the impact of different treatment conditions on plant growth.   
The second notebook, titled **`tasks.ipynb`**, contains four sections analysing various different statistical methods - **Permutations and Combinations**, **Normal Distribution**, **$t$ tests** and **ANOVA**.

## **Project Overview**

The **PlantGrowth** dataset is commonly used for statistical analysis and machine learning exercises. It consists of the following variables:
- **Weight**: The weight of plants measured after a certain growth period.
- **Group**: The treatment group applied to the plants. It has three possible values: `ctrl` (control group), `trt1` (treatment 1), and `trt2` (treatment 2).

This notebook walks through the process of:
1. **Loading and exploring the PlantGrowth dataset**.
2. Performing **descriptive statistics**.
3. Conducting a **t-test** to compare the weight of plants between two treatment groups.
4. Performing a **one-way ANOVA** to assess the difference in means across all three groups.
5. Visualizing the results using plots.

## **Requirements**

To run the analysis in this notebook, you need to have the following Python packages installed:

- `numpy`
- `pandas`
- `scipy`
- `matplotlib`
- `seaborn`

You can install these dependencies using `pip`:

```bash
pip install numpy pandas scipy matplotlib seaborn
```

Alternatively, you can install all the required dependencies from the `requirements.txt` file (if provided):

```bash
pip install -r requirements.txt
```

## **Usage**

### **Steps to Run the Analysis**

1. Clone this repository:

   ```bash
   git clone https://github.com/PeeBs68/applied_statistics
   ```

2. Launch Jupyter Notebook:

   ```bash
   jupyter notebook project.ipynb
   ```

3. Open the notebook in your browser and run the cells to perform the analysis.

### **Notebook Workflow**

The **`project.ipynb`** notebook follows these key steps:

#### 1. **Data Loading and Preprocessing**
   - The notebook loads the **PlantGrowth** dataset (available through the `seaborn` library).
   - It displays the first few rows of the dataset to give an overview of its structure.

#### 2. **Descriptive Statistics**
   - Summary statistics (mean, median, standard deviation) for the plant weights are calculated.
   - Box plots and histograms are generated to visualize the distribution of plant weights across different treatment groups.

#### 3. **t-Test (Two-Sample Comparison)**
   - A **two-sample t-test** is performed to compare the plant weights between two groups, such as the **control group** (`trt1`) and **treatment 1** (`trt2`).
   - The notebook checks for the assumptions of normality and equal variances (for the t-test).
   - The p-value from the t-test helps in determining whether the difference in mean weights is statistically significant.

#### 4. **ANOVA (Analysis of Variance)**
   - A **one-way ANOVA** is performed to test whether there is a significant difference in plant weights between all three groups (**ctrl**, **trt1**, and **trt2**).
   - Post-hoc analysis (e.g., Tukey’s HSD test) is used if the ANOVA results indicate significant differences between groups.
   - The p-value from the ANOVA helps assess whether there is a statistically significant difference in plant weights across the three groups.

#### 5. **Visualization**
   - Visualizations such as **box plots** and **bar plots** are used to help interpret the results of the statistical tests.
   - These plots allow you to easily compare the plant weights across the groups and visually assess differences.

## **Example Output**

After running the notebook, you will obtain:
- **Descriptive statistics** for each treatment group.
- **t-test results** comparing specific pairs of treatment groups (e.g., `trt1` vs `trt2`).
- **ANOVA results** for testing differences across all three groups (`ctrl`, `trt1`, and `trt2`).
- **Visualizations** that depict the distribution of plant weights and highlight statistically significant differences.


## **Tasks Overview**

This notebook walks through the process of:
1. Investigating **Permutations and Combinations** using the "Lady Tasting Tea Experiment"
2. Validating the accurmacy of numpy's **Normal Distribution**
3. Using different methods to perform **$t$ tests**
4. Performing **ANOVA tests** and estimating possibilities of commiting a type II error.

## **Requirements**

To run the analysis in this notebook, you need to have the following Python packages installed:

- `numpy`
- `pandas`
- `scipy`
- `matplotlib`
- `seaborn`

You can install these dependencies using `pip`:

```bash
pip install numpy pandas scipy matplotlib seaborn
```

Alternatively, you can install all the required dependencies from the `requirements.txt` file (if provided):

```bash
pip install -r requirements.txt
```

## **Usage**

### **Steps to Run the Analysis**

1. Clone this repository:

   ```bash
   git clone https://github.com/PeeBs68/applied_statistics
   ```

2. Launch Jupyter Notebook:

   ```bash
   jupyter notebook tasks.ipynb
   ```

3. Open the notebook in your browser and run the cells to perform the analysis.

### **Notebook Workflow**

The **`tasks.ipynb`** notebook follows these key steps:

#### 1. **Permutations and COmbination**
   - Calculates the probability of selecting six correct cups from 12.
   - Investigates the probability of making at most one, then two errors.

#### 2. **numpy Normal Distribution**
   - Assess whether numpy.random.normal generates normal values.
   - Uses Histograms and Probability Density Function to graph the outputs.

#### 3. **t-Tests**
   - Performs a $t$ test on two groups of data
   - Compares the $t$ statistic produced using the standard formula and scipy.stats.

#### 4. **ANOVA and type II errors**
   - Using numpy.random.normal to produce sample data
   - Performs one way anova tests to generate $t$ statistic values
   - Calculates the probability of committing a type II error.

---

### **Acknowledgments**

- The **PlantGrowth** dataset is publicly available in the **`seaborn`** library and is often used for teaching and demonstrating statistical methods.
- This project was created as part of a Data Analytics college course and aims to showcase how statistical analysis can be performed using Python.
