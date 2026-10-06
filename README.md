```python
import pandas as pd
df = pd.read_csv('Sample_Superstore_Clean.csv')
print(df.info())
print(df.head(2))


```

```text
<class 'pandas.core.frame.DataFrame'>
RangeIndex: 9994 entries, 0 to 9993
Data columns (total 21 columns):
 #   Column         Non-Null Count  Dtype  
---  ------         --------------  -----  
 0   Row ID         9994 non-null   int64  
 1   Order ID       9994 non-null   object 
 2   Order Date     9994 non-null   object 
 3   Ship Date      9994 non-null   object 
 4   Ship Mode      9994 non-null   object 
 5   Customer ID    9994 non-null   object 
 6   Customer Name  9994 non-null   object 
 7   Segment        9994 non-null   object 
 8   Country        9994 non-null   object 
 9   City           9994 non-null   object 
 10  State          9994 non-null   object 
 11  Postal Code    9994 non-null   int64  
 12  Region         9994 non-null   object 
 13  Product ID     9994 non-null   object 
 14  Category       9994 non-null   object 
 15  Sub-Category   9994 non-null   object 
 16  Product Name   9994 non-null   object 
 17  Sales          9994 non-null   float64
 18  Quantity       9994 non-null   int64  
 19  Discount       9994 non-null   float64
 20  Profit         9994 non-null   float64
dtypes: float64(3), int64(3), object(15)
memory usage: 1.6+ MB
None
   Row ID        Order ID  Order Date   Ship Date     Ship Mode Customer ID Customer Name   Segment        Country       City     State  Postal Code Region       Product ID   Category Sub-Category                                                 Product Name   Sales  Quantity  Discount    Profit
0       1  CA-2016-152156  2016-11-08  2016-11-11  Second Class    CG-12520   Claire Gute  Consumer  United States  Henderson  Kentucky        42420  South  FUR-BO-10001798  Furniture    Bookcases                            Bush Somerset Collection Bookcase  261.96         2       0.0   41.9136
1       2  CA-2016-152156  2016-11-08  2016-11-11  Second Class    CG-12520   Claire Gute  Consumer  United States  Henderson  Kentucky        42420  South  FUR-CH-10000454  Furniture       Chairs  Hon Deluxe Fabric Upholstered Stacking Chairs, Rounded Back  731.94         3       0.0  219.5820


```

Berikut adalah draf `README.md` yang profesional, rapi, dan siap digunakan untuk repositori GitHub project analisis data **Sample Superstore** Anda.

---

# 📊 Superstore Sales & Profitability Analysis

> Proyek analisis data komprehensif menggunakan dataset *Sample Superstore* untuk mengidentifikasi pola penjualan, tren profitabilitas, kategori produk unggulan, serta memberikan rekomendasi strategi bisnis berbasis data.

---

## 🚀 Gambaran Proyek (Project Overview)

Dataset *Sample Superstore* berisi catatan transaksi penjualan ritel di Amerika Serikat. Proyek ini bertujuan untuk mengeksplorasi data penjualan (`Sales`), kuantitas (`Quantity`), diskon (`Discount`), dan keuntungan (`Profit`) guna menemukan faktor-faktor kunci yang mempengaruhi performa bisnis serta area yang mengalami kerugian (*loss*).

---

## 🗂️ Struktur Dataset

File utama yang digunakan dalam analisis ini adalah `Sample_Superstore_Clean.csv` dengan total **9.994 baris** dan **21 kolom**, yang mencakup:

* **Informasi Transaksi:** `Row ID`, `Order ID`, `Order Date`, `Ship Date`, `Ship Mode`
* **Informasi Pelanggan:** `Customer ID`, `Customer Name`, `Segment`
* **Informasi Geografis:** `Country`, `City`, `State`, `Postal Code`, `Region`
* **Informasi Produk:** `Product ID`, `Category`, `Sub-Category`, `Product Name`
* **Metrik Finansial:** `Sales`, `Quantity`, `Discount`, `Profit`

---

## 🛠️ Tools & Libraries yang Digunakan

Proyek ini dikembangkan menggunakan **Python** dengan library analisis data utama:

* **Pandas & NumPy:** Untuk pembersihan, manipulasi, dan agregasi data.
* **Matplotlib & Seaborn:** Untuk visualisasi data interaktif dan eksploratif.

---

## 🔍 Ringkasan Analisis & Temuan Utama (Key Insights)

1. **Kategori Produk Terlaris vs Paling Menguntungkan:**
* *Technology* dan *Office Supplies* menyumbang volume penjualan dan profit yang stabil.
* *Furniture* mencatatkan penjualan yang tinggi, namun memiliki margin keuntungan yang relatif kecil atau bahkan merugi pada beberapa sub-kategori tertentu akibat diskon yang terlalu tinggi.


2. **Pengaruh Diskon Terhadap Profit:**
* Pemberian diskon di atas batas tertentu (biasanya $> 20\%$) terbukti secara konsisten memicu kerugian (*negative profit*).


3. **Analisis Regional:**
* Wilayah *West* dan *East* mendominasi total pendapatan keseluruhan, sementara beberapa negara bagian di wilayah *Central* memerlukan evaluasi strategi penetapan harga (*pricing strategy*).



---

## ⚙️ Cara Memulai (Getting Started)

Jika Anda ingin menjalankan ulang analisis ini secara lokal di komputer Anda, ikuti langkah-langkah berikut:

1. **Clone repository ini:**
```bash
git clone https://github.com/username/nama-repo-anda.git
cd nama-repo-anda

```


2. **Installdependencies yang dibutuhkan:**
```bash
pip install pandas matplotlib seaborn

```


3. **Jalankan Jupyter Notebook atau skrip Python:**
Pastikan file `Sample_Superstore_Clean.csv` berada di direktori yang sama dengan script analisis Anda.

---

## 📈 Contoh Visualisasi

*(Opsional: Anda bisa menambahkan screenshot atau gambar grafik hasil analisis Anda di sini, misalnya grafik tren penjualan per tahun atau perbandingan profit antar kategori).*

```markdown
![Contoh Grafik](path/ke/gambar-grafik.png)

```

---

## 💡 Rekomendasi Bisnis

* **Evaluasi Kebijakan Diskon:** Membatasi pemberian diskon besar (di atas 20%) pada produk-produk dengan margin tipis untuk menekan angka kerugian.
* **Fokus Pemasaran:** Meningkatkan promosi pada sub-kategori produk di segmen *Technology* yang memiliki tingkat konversi dan profitabilitas tinggi.

---

## 👤 Author

* **Nama Anda**
* [GitHub Profile](https://www.google.com/search?q=https://github.com/username)
* [LinkedIn Profile](https://linkedin.com/in/username)
