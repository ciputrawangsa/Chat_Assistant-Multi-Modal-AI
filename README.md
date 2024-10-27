# Chat Assistant using Multi Modal AI 🚀

Repositori ini berisi proyek pembuatan Chat Assistant dengan AI multi modal.AI ini berjalan dengan perintah suara dan gambar yang memungkinkan pengguna untuk mendapatkan rekomendasi produk yang tersedia sesuai dengan hasil analisa suara atau gambar. Pengguna cukup mengucapkan perintah, atau menunjukkan produk yang dimaksud dengan mengucapkan salah satu kata yang bisa memicu model untuk menganalisa produk yang dimaksud melalui hasil tangkapan gambar, selanjutnya aplikasi memberikan rekomendasi menggunakan suara untuk menjawab kebutuhan user. Hal ini diharapkan bisa membuat user untuk merasakan experience belanja yang lebih baik dan bisa meningkatkan profit perusahaan.

## Daftar Isi 🗒️
1. [Link Terkait Project](#link-terkait-project-)
2. [Project Overview](#project-overview-)
3. [Latar Belakang Masalah](#latar-belakang-masalah-)
9. [File yang Tersedia](#file-yang-tersedia-)
10. [Cara Menggunakan Proyek Ini](#cara-menggunakan-proyek-ini-)
11. [Dependencies](#dependencies-)
12. [Libraries](#libraries-)
13. [Author](#author-)

## Link Terkait Project ⛓️‍💥

- [Slides](https://drive.google.com/file/d/1aQccLW8ePUUnN_wbKMIZbk9LVK3-M-Yu/view?usp=sharing)

## Project Overview 📝

Dalam proyek ini, saya menggunakan OpenAI model gpt-4o-mini, MongoDB sebagai database, dan beberapa library untuk kebutuhan LLM seperti Langchain, dan library untuk menjalankan fungsi laptop/komputer seperti cv2, SpeechRecognition, PyGame, dan base64 sebagai alat untuk encoding foto. Bebertapa tahapan yang dilakukan:

1. **Webscrapping**:
    - Digunakan untuk menjadi modal knowledge base AI. Webscrapping dilakukan di produk rumah tangga dari Tokopedia

2. **Data Cleaning**:
    - Untuk merapihkan format data hasil webscrapping

3. **Embedding**:
    - Proses memasukkan data/knowledge base ke dalam database MongoDB

4. **Model Building**:
    - Pembuatan model AI agar bisa berinteraksi menggunakan suara dan analisa foto produk yang ditunjukkan oleh user, respon AI didasarkan pada knowledge base yang sudah diatur sebelumnya

## Latar Belakang Masalah 🧐

Dalam industri e-commerce yang kompetitif, mempertahankan loyalitas pelanggan menjadi tantangan utama. Pelanggan
seringkali merasa kurang mendapatkan perhatian dan respons cepat saat menghadapi masalah, memiliki pertanyaan tentang
produk, atau memerlukan bantuan selama proses pembelian. Ketidakpuasan ini dapat mengurangi pengalaman pelanggan,
menurunkan tingkat retensi, dan mengakibatkan hilangnya peluang untuk menciptakan hubungan jangka panjang yang lebih
kuat dengan pelanggan.

## File yang Tersedia 📂

- `scrap_scratch.ipynb`: Jupyter Notebook yang berisi langkah-langkah dalam melakukan webscrappiing
- `csv_cleaning.ipynb`: Jupyter Notebook yang berisi langkah-langkah dalam merapihkan format csv yang akan dimasukkan ke dalam database.
- `embedding_to_mongo.ipynb`: Jupyter Notebook yang berisi proses embedding data knowledge base ke dalam database MongoDB
- `app.py`: File python yang memuat program chat assistant
- `requirements`: File .txt yang berisi library yang digunakan untuk menjalankan aplikasi
- `tes.csv`: file csv hasil webscrapping
- `cleaned_data.csv`: file csv yang berisi data yang siap dimasukkan ke dalam database MongoDB

## Cara Menggunakan Proyek Ini 💻

1. Buat file.env yang berisi API key dan server MongoDB:

OPENAI_API_KEY= ......
MONGODB_URI= ......

2. Lakukan instalasi library yang ada pada requirements.txt

3. Lakukan embedding data ke dalam database MongoDB

4. Jalankan file app.py

## Dependencies ⚙️
- ![Jupyter Notebook](https://img.shields.io/badge/Made%20with-Jupyter-orange?style=for-the-badge&logo=Jupyter)
- ![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)

## Libraries 📚
- OpenAI
- PyMongo
- Langchain
- cv2
- gtts
- pygame
- tenacity
- python-dotenv
- soundfile

## Author ✍️
**Ciputra Wangsa**

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/ciputra-wangsa/)