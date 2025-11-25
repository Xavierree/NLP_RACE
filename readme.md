# 🧠 NLP Project: Topic Modelling pada RACE Dataset

**Nama:** Eideltha Xavierre Sembiring Kembaren  
**NIM:** 36230034  
**Kelas:** 5PDS1  
**Mata Kuliah:** DSF06 - Natural Language Processing  

---

## 📌 Deskripsi Proyek

Proyek ini bertujuan untuk melakukan *Topic Modelling* pada dataset **RACE (Reading Comprehension Dataset from Examinations)** menggunakan berbagai algoritma Machine Learning.  
Tujuan utama proyek adalah mengekstrak dan menganalisis topik tersembunyi dari kumpulan teks artikel/bacaan.

Model yang digunakan dan dibandingkan dalam proyek ini:

| Model | Metode | Deskripsi |
|-------|--------|-----------|
| **LSA** | Linear Algebra (SVD) | Menguraikan hubungan kata-topik menggunakan dekomposisi matriks |
| **NMF** | Linear Algebra | Faktor non-negatif untuk analisis komponen topik |
| **LDA** | Probabilistic Model | Model generatif berbasis distribusi Dirichlet |
| **BERTopic** | Transformer + c-TF-IDF | Membentuk topik berbasis embedding BERT |

---

## 📂 Dataset

Dataset yang digunakan: **RACE Dataset (TensorFlow Datasets)**  
Dataset diambil otomatis melalui `tensorflow_datasets` tanpa mengunduh file manual.

---

## 🚀 Cara Menjalankan Proyek

### **☁ Opsi A — Google Colab (Disarankan)**

Karena Colab menyediakan **GPU gratis**, metode ini optimal untuk BERTopic.

1️⃣ Upload file berikut ke Colab:
- `UAS_NLP_Topic_Modelling.ipynb`
- `requirements.txt`

2️⃣ Aktifkan GPU:  
> Runtime → Change runtime type → T4 GPU → Save

3️⃣ Instal library:
```bash
pip install -r requirements.txt && python -m nltk.downloader stopwords punkt wordnet omw-1.4 punkt_tab
