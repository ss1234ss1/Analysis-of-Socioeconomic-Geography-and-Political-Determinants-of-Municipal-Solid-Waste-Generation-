# Analysis of Socioeconomic, Geographic, and Political Determinants of Municipal Solid Waste Generation in OECD Countries (1997-2021)

##  Overview
This project examines the socioeconomic, geographic, and political factors influencing **municipal solid waste (MSW) generation** in **OECD countries** from **1997 to 2021**. Using **panel regression, OLS regression, and ANOVA**, the study identifies key determinants that affect waste production and provides policy recommendations for sustainable waste management.

###  **Why Study Municipal Solid Waste (MSW)?**
- **Environmental Impact**: MSW contributes significantly to **greenhouse gas emissions** and pollution.
- **Economic Costs**: Inefficient waste management leads to increased **public spending**.
- **Policy Implications**: Understanding the drivers of MSW generation helps shape **effective environmental policies**.

---

## Data and Preprocessing
### **Dataset**
- **Scope**: 25 OECD countries
- **Time Period**: 1997 - 2021
- **Data Sources**: 
  - **OECD**, **World Bank**, **UNDP**, **Global Data Lab**
- **Key Variables**:
  - **Dependent Variable**: MSW generation per capita (kg)
  - **Independent Variables**:
    - **Socioeconomic**: GNI, household spending, life expectancy, mean years of schooling
    - **Demographic/Geographic**: Urban population, population density, fertility rate, temperature
    - **Political**: Environmental tax, waste recovery operations, environmental policy stringency

### **Data Preprocessing**
- **Data Cleaning**: Addressed missing values using interpolation.
- **Feature Scaling**: Normalized variables where necessary.
- **Multicollinearity Check**: Removed highly correlated variables (VIF > 10).
- **Log Transformation**: Considered but not applied due to minimal skewness.

---

##  Methodology
### **1️⃣ Panel Regression (Fixed Effects)**
- **Controls for time-invariant country-specific factors**.
- **Identifies key drivers** of MSW generation over time.
- **Significant Predictors**:
  - Household spending per capita (+)
  - Life expectancy (-)
  - Urban population (-)
  - Waste recovery operations per capita (+)
  - Environmental tax per capita (-)
  
### **2️⃣ OLS Regression (Time & Space Controls)**
- **Addresses non-stationary variables**.
- **Finds overall trends** in MSW generation.
- **Key Insights**:
  - Higher **household spending per capita** leads to more waste.
  - **Environmental technology** has a small but negative impact on MSW.
  - Higher **life expectancy** is linked to lower waste production.

### **3️⃣ ANOVA (Group Comparisons)**
- **Tests differences** in MSW across countries and political factors.
- **Findings**:
  - Environmental policy stringency **reduces** MSW in some countries but has **low explanatory power** overall.

---

##  Results and Evaluation
| **Model**         | **R² Score** | **Key Findings** |
|------------------|------------|------------------|
| **Panel Regression**  | 0.43 (Within) | Household spending and policy matter |
| **OLS Regression**  | 0.89 | Socioeconomic factors drive MSW |
| **ANOVA**  | 0.06 - 0.53 | Political factors vary by country |

### **Key Insights**
- **Consumption behaviors** are a major driver of MSW.
- **Higher environmental taxes** are effective in reducing waste.
- **Urban areas in OECD countries** have better waste management systems.

---

