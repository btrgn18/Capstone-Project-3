# CAPSTONE MODULE 03 - DAEGU APARTMENT
>`AIMAR MOHAMMAD BUTRAGUENO`

# **Context**
<blockquote style="text-align: justify">
Apartments have become the primary solution to meet housing needs in urban areas due to limited land availability and the high intensity of business activities in cities. In Daegu, determining the selling price of an apartment is crucial to ensure that owners gain optimal profit without losing competitiveness in the market. Mispricing can lead to difficulties in selling apartment units or result in suboptimal profits. Therefore, an analytical approach is needed to predict the right price based on various factors such as apartment size, available facilities, transportation access, and the surrounding environment.
</blockquote>

# **Problem Statement**
<blockquote style="text-align: justify">
In the urban area of Daegu, determining the appropriate selling price of apartments is a critical challenge due to the complex interplay of internal and external factors influencing property value. Apartment owners often struggle to set competitive prices that balance profitability with market demand. Without a data-driven pricing strategy, there is a risk of overpricing, which can deter buyers, or underpricing, which leads to financial losses. Therefore, there is a need for an accurate predictive model that can analyze historical apartment sales data and identify key factors—such as size, facilities, transportation access, and neighborhood conditions—to estimate optimal apartment prices and support informed decision-making in the real estate market.
</blockquote>

# **Goals**
<blockquote style="text-align: justify">

- To develop an accurate apartment price prediction model based on historical data.
- To identify the features or factors that most significantly influence apartment prices in Daegu.
- To provide optimal price recommendations that apartment owners can use for selling decisions.
</blockquote>

# **Analytical Approach**
<blockquote style="text-align: justify">

- Utilizing regression techniques to predict apartment prices.
- Conducting Exploratory Data Analysis (EDA) to understand the characteristics of the data.
- Performing data preprocessing including handling missing values, encoding categorical variables, and normalizing numerical features.
- Evaluating multiple regression models such as Linear Regression, Decision Tree Regression, and Random Forest Regression to select the best-performing model.
- Applying feature importance techniques to identify the most influential factors affecting apartment prices.
</blockquote>

# **Evaluation Metrics**
<blockquote style="text-align: justify">

- Root Mean Squared Error (RMSE) to evaluate prediction accuracy.
- Mean Absolute Error (MAE) as an additional indicator to understand the average prediction error.
- R-squared (R²) to measure the extent to which independent variables explain the variability of apartment prices.
</blockquote>

# **Stakeholder**
<blockquote style="text-align: justify">

Store Manager dan Marketing & Sales Teams
<blockquote>
  
# **Data Dictionary**
<blockquote style="text-align: justify">

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
<blockquote>

# **Metodologi**
<blockquote style="text-align: justify">
1. **Data Understanding & EDA**
2. **Data Preprocessing**
3. **Feature Engineering**
4. **Baseline Modeling:** (Linear Regression, Decision Tree, Random Forest)
5. **Cross-Validation (5-fold)** (MAE, RMSE, R²)
6. **Hyperparameter Tuning** (RandomizedSearchCV)
7. **Feature Importance Analysis**
8. **Residual Analysis**

---

# **Kesimpulan**
Project ini bertujuan untuk membangun model prediktif yang mampu mengestimasi harga apartemen di Kota Daegu secara akurat, serta mengidentifikasi faktor-faktor utama yang memengaruhi nilai pasar properti tersebut.

Melalui serangkaian proses seperti eksplorasi data, preprocessing, feature engineering, modeling baseline, dan hyperparameter tuning, diperoleh model final berbasis `Random Forest Regressor` yang telah dioptimalkan menggunakan `RandomizedSearchCV`.

Hasil evaluasi menunjukkan bahwa model tersebut memiliki performa yang sangat baik, dengan skor sebagai berikut:

> `MAE` = 33.171

> `RMSE` = 42.004

> `R²` = 0.8335

Untuk memastikan stabilitas dan keadilan prediksi model, dilakukan juga `Residual Analysis`. Hasil visualisasi residual menunjukkan bahwa:

- Error menyebar secara acak dan merata di seluruh rentang prediksi
- Distribusi residual mendekati normal
- Tidak ditemukan pola sistematis atau bias terhadap harga rendah atau tinggi

Hal ini membuktikan bahwa model tidak hanya akurat secara metrik, tapi juga stabil dan valid secara statistik.
Model ini dapat dijadikan acuan dalam sistem pricing apartemen yang lebih objektif dan berbasis data.

# **Rekomendasi Bisnis**
Berdasarkan hasil analisis modeling dan interpretasi fitur terpenting, beberapa rekomendasi yang dapat diberikan antara lain:

1. Fokus pada aspek ukuran unit (`Size`)
Luas apartemen adalah faktor paling dominan dalam menentukan harga. Developer dapat menekankan desain unit yang lebih luas dan efisien.

2. Perhatikan desain interior dan hallway
`HallwayType` terbukti menjadi fitur penting. Desain lorong dan akses antar unit dapat memengaruhi persepsi nilai dari konsumen.

3. Pertimbangkan faktor usia bangunan
Unit yang lebih baru memiliki harga jual lebih tinggi. Untuk unit lama, strategi renovasi dan modernisasi bisa menjadi solusi untuk meningkatkan nilai pasar.

4. Gunakan model ini sebagai alat bantu pricing
Model `Random Forest` ini dapat digunakan oleh agen properti dan pemilik apartemen sebagai panduan objektif dalam menentukan harga yang kompetitif dan realistis, tanpa underprice maupun overprice.

---

# Link Video Presentation
https://drive.google.com/drive/folders/1VchuMrBBn9zXMOAdGgQkBdylilccQikx?usp=sharing

# Link PPT Canva
https://www.canva.com/design/DAGmfMbJVMI/Dhy6FWmv_AOMIK9FkhG-mQ/edit?utm_content=DAGmfMbJVMI&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton
