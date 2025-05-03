# 🧠 Türkçe Duygu Analizi Uygulaması

Bu proje, Türkçe cümlelerdeki duyguları sınıflandırmak için eğitilmiş bir makine öğrenmesi modeline dayalı **interaktif bir Streamlit uygulamasıdır**.

---

## 🚀 Uygulama Özellikleri

- 📥 Kullanıcıdan metin girişi alır
- 🧹 Metni ön işler (küçük harfe çevirme, noktalama temizliği, İngilizce stopword filtreleme)
- 🧠 CountVectorizer ile vektörleştirir
- 🤖 Logistic Regression modeliyle duygu tahmini yapar
- 🎯 Tahmin sonucunu kullanıcıya açık bir şekilde sunar

---

## 💾 Kullanılan Teknolojiler

| Araç/Kitaplık           | Açıklama |
|------------------------|----------|
| `Streamlit`            | Web arayüzü oluşturmak için |
| `scikit-learn`         | ML modeli ve vektörleştirme için |
| `Pickle`               | Model ve vectorizer dosyalarını yüklemek için |
| `Python`               | Projenin dili |

---

## 🧪 Tahmin Edebilen Duygular

Model aşağıdaki 5 sınıfta tahmin yapar:

| Etiket | Duygu   |
|--------|---------|
| 0      | Korku   |
| 1      | Kızgın  |
| 2      | Mutlu   |
| 3      | Şaşkın  |
| 4      | Üzgün   |

---

## 📁 Klasör Yapısı

```bash
.
├── app
│   └── app.py                    # Streamlit arayüz kodu
├── model
│   ├── emotion_model.pkl         # Eğitilmiş Logistic Regression modeli
│   └── count_vectorizer.pkl      # CountVectorizer nesnesi
├── data
│   └── TurkishTweets.xlsx        # Ham veri (isteğe bağlı)
├── notebook
│   └── emotion_analysis.ipynb    # Eğitim süreci ve analiz not defteri
├── README.md                     # Bu belge
└── requirements.txt              # Gerekli kütüphaneler

# Gerekli kütüphaneleri yükleyin
pip install -r requirements.txt

# Uygulamayı başlatın
streamlit run app/app.py
```

🤝 Katkı

Katkıda bulunmak isterseniz PR (pull request) gönderebilir ya da issue açabilirsiniz.
