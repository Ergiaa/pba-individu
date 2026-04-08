# PBA Individu

Proyek analisis teks dan pemrosesan data untuk mata kuliah PBA (Pengolahan Bahasa Alami).

## Deskripsi

Proyek ini berisi serangkaian notebook Jupyter untuk analisis sentimen dan pengolahan teks pada data ulasan aplikasi Spotify. Workflow meliputi:

1. **Scraping Data** - Mengambil data ulasan dari Google Play Store
2. **Exploratory Data Analysis (EDA)** - Analisis awal data
3. **Preprocessing** - Pembersihan dan normalisasi teks
4. **Bag of Words (BoW)** - Ekstraksi fitur dan representasi teks

## Struktur File

File-file yang tersedia dalam repository ini:

| File | Deskripsi |
|------|-----------|
| `week-2/1-scrapping.ipynb` | Notebook untuk scraping data ulasan dari Google Play Store |
| `week-2/2-eda.ipynb` | Notebook EDA (Exploratory Data Analysis) tahap awal |
| `week-3/3-preprocessing.ipynb` | Notebook preprocessing data teks |
| `week-4/4-bow.ipynb` | Notebook implementasi Bag of Words |
| `week-4/5-eda.ipynb` | Notebook EDA tambahan setelah preprocessing |
| `pyproject.toml` | Konfigurasi proyek Python dan dependensi |
| `uv.lock` | File lock untuk dependensi UV |
| `.python-version` | Versi Python yang digunakan |
| `.gitignore` | File konfigurasi git ignore |

## Output Files

File hasil proses (dataset mentah, dataset bersih, hasil BoW, dan insight) tidak disimpan di repository ini karena ukurannya yang besar. Output files dapat diakses di Google Drive:

**[Google Drive - Output Files](https://drive.google.com/drive/folders/1BhoomVQcRz5PXx-7BoPT_z1ok_ROB1uE?usp=sharing)**

File output yang tersedia:
- `rawdata_spotify_id.csv` - Dataset mentah hasil scraping
- `cleandata_spotify.csv` - Dataset setelah preprocessing
- `bow_positif_spotify.csv` - Hasil BoW untuk ulasan positif
- `bow_negatif_spotify.csv` - Hasil BoW untuk ulasan negatif
- `regex_insight_spotify.csv` - Insight dari analisis regex

## Requirements

- Python >= 3.12
- Dependencies terdaftar di `pyproject.toml`

## Cara Menjalankan

1. Install dependensi menggunakan UV:
   ```bash
   uv sync
   ```

2. Aktifkan virtual environment:
   ```bash
   source .venv/bin/activate
   ```

3. Jalankan notebook menggunakan Jupyter:
   ```bash
   jupyter notebook
   ```
