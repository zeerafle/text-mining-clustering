# Text Mining dengan Clustering

## Mengakses Notebook
Notebook bisa langsung dibuka dengan download repositori ini sebagai zip, extract, kemudian buka notebooknya dengan Jupyter Notebook yang sudah terpasang. Untuk bisa menjalankan notebooknya pastikan juga sudah menginstall semua library yang dibutuhkan (terdapat di file *requirement.txt*). Caranya dengan buka terminal/CMD kemudian ketikkan perintah dibawah:
```bash
pip install <nama_library1> <nama_library2> <nama_library...>
```

Tapi cara yang disarankan adalah dengan membuat environtment jika Anda pernah menggunakan [Anaconda](https://www.anaconda.com/products/individual#Downloads) atau jalankan file notebooknya di [Google Colaboratory](https://colab.research.google.com/)

### Membuat Environtment dengan Conda
1. Download repository ini dengan klik tombol *Code* warna hijau diatas, kemudian *__Download ZIP__*. Atau jika sudah terinstall *git* di komputer Anda, cukup jalankan perintah dibawah dengan terminal/CMD.
    ```bash
    git clone https://github.com/zeerafle/text-mining-clustering
    ```

2. Kemudian buka *Anaconda Prompt*, lalu jalankan perintah berikut:
    ```bash
    conda env create -f environment.yml
    ```
    Biarkan berjalan, jika ada pertanyaan untuk konfirmasi cukup ketikkan `y` kemudian enter.

3. Setelah proses selesai aktifkan environment yang sudah dibuat
    ```bash
    conda activate textmining
    ```
    Pastikan nama environment (textmining) muncul didalam tanda kurung.

4. Selanjutnya install kernel. Jalankan perintah dibawah
    ```bash
    pip install ipykernel
    ```
    Kemudian jalankan lagi perintah dibawah. Untuk nilai dari parameter *name* (pada `--name=`) disesuaikan dengan nama environment (dalam hal ini adalah 'textmining')
    ```bash
    python -m ipykernel install --user --name=textmining
    ```

5. Proses instalasi selesai. Sekarang buka jupyter lab dengan ketikkan
    ```
    jupyter lab
    ```

### Buka Notebook dengan Google Colab
Dengan Google Colab, tidak perlu konfigurasi environment dan sebagainya. Hanya perlu menginstall library yang ingin dipakai setiap kali baru menjalan notebooknya.

1. Buka notebooknya di Google Colab
    - clustering-comparison-oriented.ipynb [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zeerafle/text-mining-clustering/blob/master/clustering-comparison-oriented.ipynb)
    - clustering-result-oriented.ipynb [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/zeerafle/text-mining-clustering/blob/master/clustering-result-oriented.ipynb)

2. Sebagian besar library sudah tersedia secara default di Colab, namun jika ingin menginstall library lain (misalnya *scikit-learn-extra*)tambahkan sel baru didalam Colab, ketikkan kode dibawah, kemudian jalankan selnya. 
    ```bash
    !pip install scikit-learn-extra
    ```
    Semua library yang diperlukan ada di file *requirements.txt*

---
##### Useful Resource
- [Cheat sheet for implementing 7 methods for selecting the optimal number of clusters in Python](https://towardsdatascience.com/cheat-sheet-to-implementing-7-methods-for-selecting-optimal-number-of-clusters-in-python-898241e1d6ad)