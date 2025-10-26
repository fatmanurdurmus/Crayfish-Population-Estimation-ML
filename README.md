# Crayfish-Population-Estimation-ML
Machine learning project estimating crayfish population using regression and feature selection methods (Google Colab version).


## 🇹🇷  🦞 Kerevit Popülasyonu Tahmini (Makine Öğrenmesi)
Bu proje, **kerevit (Astacus leptodactylus)** popülasyonunu tahmin etmek için farklı makine öğrenmesi algoritmalarını kullanır.  
Veri ön işleme, korelasyon/varyans/LASSO tabanlı özellik seçimi ve **Doğrusal Regresyon, Karar Ağacı, Rastgele Orman, SVM, PCA+LR, MLPRegressor** gibi modelleri içerir.  
Değerlendirme metrikleri: **MAE, MSE, RMSE, R²** ve **Uyum İndeksi (C-index)**.  
Son olarak, aylık popülasyon değişimlerini simüle eden bir grafik üretilir.

## ⚙️ Kullanılan Teknolojiler ve Kütüphaneler
- **Python**  
- **pandas**, **numpy** – veri işleme  
- **matplotlib**, **seaborn** – veri görselleştirme  
- **scikit-learn** – makine öğrenmesi modelleri (Linear Regression, Decision Tree, Random Forest, SVM, PCA, MLPRegressor)  
- **lifelines** – C-index metriği için  
- **openpyxl** – Excel dosyası okuma  

---

## 🧠 Kullanılan Yöntemler
### 🔹 Özellik Seçimi
- Korelasyon tabanlı seçim  
- Varyans eşiği (VarianceThreshold)  
- LASSO regresyon tabanlı seçim  

### 🔹 Modeller
- Doğrusal Regresyon (Linear Regression)  
- Karar Ağaçları (Decision Tree Regressor)  
- Rastgele Orman (Random Forest Regressor)  
- Destek Vektör Makineleri (SVR)  
- PCA (Temel Bileşenler Analizi)  
- MLPRegressor (Yapay Sinir Ağı modeli)

### 🔹 Değerlendirme Metrikleri
- MAE (Ortalama Mutlak Hata)  
- MSE (Ortalama Kare Hatası)  
- RMSE (Karekök Ortalama Kare Hatası)  
- R² (Determinasyon Katsayısı)  
- C-index (Uyum İndeksi)

---

## 📊 Çıktılar
- Konsolda metrik sonuçları (MAE, MSE, RMSE, R², C-index)  
- Özellik önem grafikleri (feature importance)  
- Aylık popülasyon değişim grafikleri (toplam, dişi, erkek, avlanabilir)  

---

## 📦 Veri Seti Hakkında
Proje **örnek bir veri seti** ile geliştirilmiştir.  
Veri seti (`DataSet.xlsx`) Colab üzerinde yüklenmiş olup **GitHub’a yüklenmemiştir.**  
İstersen kendi Excel dosyanı aynı isimle (`DataSet.xlsx`) ekleyip kodu çalıştırabilirsin.

> 🔸 Veri setinde `TA` hedef değişken olarak kullanılmış, `TB` bazı analizlerde referans olarak alınmıştır.  
> Kendi verinde sütun adları farklıysa kod içinde güncelleyebilirsin.

### ⚙️ Colab Uyumluluğu
Bu kod **Google Colab** ortamında geliştirilmiştir.  
Bu nedenle `!pip install` ve `google.colab.files.upload()` gibi bazı satırlar Colab’a özeldir.  
Kodu bilgisayarında çalıştırmak istersen:
- Bu satırları kaldır veya yorum satırı haline getir.  
- Gerekli kütüphaneleri şu komutla yükle: `pip install -r requirements.txt`

 
---

📌 **Prepared by:** Fatma Nur Durmuş  
🎓 *Software Engineering Student – Atatürk University*  


---
## 🇬🇧  🦞 Crayfish Population Estimation (Machine Learning)
This project uses various **machine learning algorithms** to estimate the population of **crayfish (Astacus leptodactylus)**.  
It includes data preprocessing, correlation/variance/LASSO-based feature selection, and models such as **Linear Regression, Decision Tree, Random Forest, SVM, PCA+LR, and MLPRegressor**.  
Evaluation metrics include **MAE, MSE, RMSE, R²**, and **Concordance Index (C-index)**.  
Finally, a simulation graph visualizes monthly population changes.

## ⚙️ Technologies and Libraries Used
- **Python**  
- **pandas**, **numpy** – data processing  
- **matplotlib**, **seaborn** – data visualization  
- **scikit-learn** – machine learning models (Linear Regression, Decision Tree, Random Forest, SVM, PCA, MLPRegressor)  
- **lifelines** – for C-index metric  
- **openpyxl** – to read Excel files  

---

## 🧠 Methods Used
### 🔹 Feature Selection
- Correlation-based selection  
- Variance threshold (VarianceThreshold)  
- LASSO regression-based selection  

### 🔹 Models
- Linear Regression  
- Decision Tree Regressor  
- Random Forest Regressor  
- Support Vector Machine (SVR)  
- PCA (Principal Component Analysis)  
- MLPRegressor (Neural Network model)

### 🔹 Evaluation Metrics
- MAE (Mean Absolute Error)  
- MSE (Mean Squared Error)  
- RMSE (Root Mean Squared Error)  
- R² (Coefficient of Determination)  
- C-index (Concordance Index)

---

## 📊 Outputs
- Console metrics (MAE, MSE, RMSE, R², C-index)  
- Feature importance plots  
- Monthly population variation graphs (total, female, male, harvestable)  

---

## 📦 Dataset Information
The project was developed using a **sample dataset**.  
The dataset (`DataSet.xlsx`) was uploaded and used in Colab, but **not included in the GitHub repository**.  
You can use your own Excel file with the same name (`DataSet.xlsx`) to run the code.

> 🔸 The dataset uses `TA` as the target variable and `TB` as a reference in some analyses.  
> If your dataset uses different column names, you can update them directly in the code.

### ⚙️ Colab Compatibility
This code was developed in **Google Colab**.  
Therefore, some lines such as `!pip install` and `google.colab.files.upload()` are specific to Colab.  
If you want to run it locally:
- Remove or comment out these lines.  
- Install the required libraries using: `pip install -r requirements.txt`
