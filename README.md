# CAPSTONE MODULE 03 - DAEGU APARTMENT
>`AIMAR MOHAMMAD BUTRAGUENO`

# **Context**
Apartments have become the primary solution to meet housing needs in urban areas due to limited land availability and the high intensity of business activities in cities. In Daegu, determining the selling price of an apartment is crucial to ensure that owners gain optimal profit without losing competitiveness in the market. Mispricing can lead to difficulties in selling apartment units or result in suboptimal profits. Therefore, an analytical approach is needed to predict the right price based on various factors such as apartment size, available facilities, transportation access, and the surrounding environment.

# **Problem Statement**
In the urban area of Daegu, determining the appropriate selling price of apartments is a critical challenge due to the complex interplay of internal and external factors influencing property value. Apartment owners often struggle to set competitive prices that balance profitability with market demand. Without a data-driven pricing strategy, there is a risk of overpricing, which can deter buyers, or underpricing, which leads to financial losses. Therefore, there is a need for an accurate predictive model that can analyze historical apartment sales data and identify key factors—such as size, facilities, transportation access, and neighborhood conditions—to estimate optimal apartment prices and support informed decision-making in the real estate market.

# **Goals**
- To develop an accurate apartment price prediction model based on historical data.
- To identify the features or factors that most significantly influence apartment prices in Daegu.
- To provide optimal price recommendations that apartment owners can use for selling decisions.

# **Analytical Approach**
- Utilizing regression techniques to predict apartment prices.
- Conducting Exploratory Data Analysis (EDA) to understand the characteristics of the data.
- Performing data preprocessing including handling missing values, encoding categorical variables, and normalizing numerical features.
- Evaluating multiple regression models such as Linear Regression, Decision Tree Regression, and Random Forest Regression to select the best-performing model.
- Applying feature importance techniques to identify the most influential factors affecting apartment prices.

# **Evaluation Metrics**
- Root Mean Squared Error (RMSE) to evaluate prediction accuracy.
- Mean Absolute Error (MAE) as an additional indicator to understand the average prediction error.
- R-squared (R²) to measure the extent to which independent variables explain the variability of apartment prices.

# **Stakeholder**
- Apartment Owners
- Sales Agents
- Apartment Developers

# **Data Dictionary**
**FEATURES**
| Column | Description (EN) | Deskripsi (ID)
| -- | --- | ---
| HallwayType | Apartment type | Tipe apartemen
| TimeToSubway | Time needed to the nearest subway station | Waktu yang dibutuhkan ke stasiun subway terdekat
| SubwayStation | The name of the nearest subway station | Nama stasiun subway terdekat
| N_FacilitiesNearBy (ETC) | The number of facilities nearby | Jumlah fasilitas umum di sekitar
| N_FacilitiesNearBy (PublicOffice) | The number of public office facilities nearby | Jumlah kantor pemerintahan di sekitar
| N_SchoolNearBy (University) | The number of universities nearby | Jumlah universitas di sekitar
| N_Parkinglot (Basement) | The number of the parking lot | Jumlah tempat parkir (di basement)
| YearBuilt | The year the apartment was built | Tahun pembangunan apartemen
| N_FacilitiesInApt | Number of facilities in the apartment | Jumlah fasilitas di dalam apartemen
| Size (sqf) | The apartment size (in square feet) | Ukuran apartemen (dalam kaki persegi)
| SalePrice | The apartment price (Won) | Harga apartemen (dalam Won)

# **Methodology**
1. **Data Understanding & EDA**
2. **Data Preprocessing**
3. **Feature Engineering**
4. **Baseline Modeling:** (Linear Regression, Decision Tree, Random Forest)
5. **Cross-Validation (5-fold)** (MAE, RMSE, R²)
6. **Hyperparameter Tuning** (RandomizedSearchCV)
7. **Feature Importance Analysis**
8. **Residual Analysis**

---

# **Conclusion**
This project aims to develop a predictive model capable of accurately estimating apartment prices in Daegu City, as well as identifying the key factors that influence the market value of these properties.

Through a series of processes including data exploration, preprocessing, feature engineering, baseline modeling, and hyperparameter tuning, a final model based on the `Random Forest Regressor` was obtained and optimized using `RandomizedSearchCV`.

Evaluation results show that the model performs very well, with the following scores:
> `MAE` = 33.171

> `RMSE` = 42.004

> `R²` = 0.8335

To ensure the stability and fairness of the model's predictions, a `Residual Analysis` was also conducted. The residual visualization results indicate that:
- Errors are randomly and evenly distributed across the entire prediction range

- The residuals follow a near-normal distribution

- No systematic patterns or biases were found toward low or high prices

These findings demonstrate that the model is not only accurate in terms of metrics, but also statistically stable and valid.
This model can serve as a reference for a more objective and data-driven apartment pricing system.

# **Business Recommendations**
Based on the modeling results and interpretation of the most important features, several recommendations can be made:

1. Focus on unit size (`Size`)

  Apartment size is the most dominant factor in determining price. Developers should emphasize designing more spacious and efficient units.

2. Pay attention to interior and hallway design

  `HallwayType` has proven to be an important feature. The layout and accessibility of hallways can influence consumer perception of value.

3. Consider the age of the building

  Newer units tend to have higher selling prices. For older units, renovation and modernization strategies can be effective in increasing market value.

4. Utilize this model as a pricing support tool

  The `Random Forest` model can be used by real estate agents and apartment owners as an objective guide for setting competitive and realistic prices—avoiding both underpricing and overpricing.
  
---

# Link Video Presentation
https://drive.google.com/drive/folders/1VchuMrBBn9zXMOAdGgQkBdylilccQikx?usp=sharing

# Link PPT Canva
https://www.canva.com/design/DAGmfMbJVMI/Dhy6FWmv_AOMIK9FkhG-mQ/edit?utm_content=DAGmfMbJVMI&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
