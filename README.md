# 🔍 Açıklanabilir Zaman Serisi Tahmin Modeli (XAI)

Bu proje, finansal zaman serisi verileri üzerinde makine öğrenmesi modellerinin kararlarını analiz etmek ve açıklanabilir kılmak amacıyla geliştirilmiştir. Bitcoin (BTC-USD) günlük kapanış fiyatları kullanılarak geleceğe yönelik tahminler üretilmiş ve modelin tahminleri oyun teorisi tabanlı **SHAP (SHapley Additive exPlanations)** yöntemiyle açıklanmıştır.

Ayrıca kullanıcıların istedikleri tarihleri seçerek tahminleri ve model kararlarını interaktif olarak inceleyebilmeleri için bir **Gradio Dashboard** arayüzü entegre edilmiştir.

## 📋 Proje Akışı & Özellikler
- **Veri Kaynağı:** `yfinance` API kütüphanesi aracılığıyla çekilen Bitcoin geçmiş verileri.
- **Özellik Mühendisliği:** Zaman serisi analizine uygun Pencere Tabanlı (Windowing/Lag) özellik üretimi.
- **Model:** Gradyan arttırma tabanlı güçlü ve hızlı `LightGBM` algoritması.
- **Performans Ölçümü:** Tahmin başarısı RMSE, MAE ve MAPE skorları ile değerlendirilmiştir.
- **Açıklanabilir Yapay Zeka (XAI):** `SHAP TreeExplainer` kullanılarak geçmiş günlerdeki (Lag özellikleri) fiyat hareketlerinin anlık tahmini ne yönde ve ne kadar etkilediği global ve yerel düzeyde analiz edilmiştir.
- **Kullanıcı Arayüzü:** `Gradio` entegrasyonu ile interaktif grafik ve metin tabanlı dashboard.

## 🛠️ Kullanılan Teknolojiler
- Python 3
- LightGBM
- SHAP (SHapley Additive exPlanations)
- Optuna
- yfinance
- Gradio
- Pandas, NumPy, Matplotlib, Seaborn, Scikit-Learn

