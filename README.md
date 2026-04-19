# Market-basket-analysis-project
# 🛒 Market Sepeti Analizi & Strateji Optimizasyonu

Bu proje, bir perakende işletmesinin satış verilerini kullanarak müşteri alışkanlıklarını analiz eder ve çapraz satış (cross-selling) stratejileri geliştirmeyi amaçlar.

## 📊 Metodoloji
Bu çalışmada **Apriori Algoritması** kullanılarak birliktelik kuralları (Association Rules) çıkarılmıştır. Analiz süreci şu aşamalardan oluşur:

1. **SQL Entegrasyonu:** Ham veriler SQLite veritabanına aktarılarak yapılandırılmış hale getirilmiştir.
2. **Veri Ön İşleme:** Python (Pandas) kullanılarak veriler algoritma formatına dönüştürülmüştür.
3. **Analiz Parametreleri:** - **Support (Destek):** 0.003
   - **Confidence (Güven):** 0.2
   - **Lift (Kaldıraç):** 3 (Minimum 3 kat anlamlı ilişki aranmıştır)

## 💡 Öne Çıkan Bulgular
Analiz sonucunda 9 anlamlı kural tespit edilmiştir. Bazı dikkat çekici eşleşmeler:
- **Bal & Beyaz Peynir:** En yüksek kaldıraç değerine (5.16) sahip kuraldır.
- **Krema & Tavuk:** Müşterilerin yemeklik kombinasyonlarındaki eğilimini göstermektedir.

## 📂 Dosya Yapısı
- `market_basket_analizi.ipynb`: Projenin Python kodları.
- `market_analizi.db`: SQL veritabanı dosyası.
- `Market_sepeti_analiz_raporu.xlsx`: Analiz sonuçlarının iş dünyasına yönelik raporu.
