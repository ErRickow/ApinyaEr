# ApiNyaEr
what

---

# 📘 API Documentation

Welcome to the **ErApi**! This library allows you to easily interact with the API using both **synchronous** and **asynchronous** options.

- **Sync**: `from ApiNyaEr.sync import apinya`
- **Async**: `from ApiNyaEr import apinya`

Below, we’ll cover each function, providing examples and expected results so you can get started quickly! Let’s dive in 🚀

## Status

| Function           | Status |
|--------------------|--------|
| [1. Ai](#1-ai) | ✅
| [2. Ai Image](#2-ai-image) | ❌
| [3. Blackbox](#3-blackbox) | ✅
| [4. Carbon](#4-carbon) | ✅
| [5. Cat](#5-cat) | ✅
| [6. Dare](#6-dare) | ✅
| [7. Doa](#7-doa) | ✅
| [8. Dog](#8-dog) | ✅
| [9. Fakta Unik](#9-fakta-unik) | ✅
| [10. Gemini](#10-gemini) | ✅
| [11. Github Search](#11-github-search) | ✅
| [12. Hug](#12-hug) | ✅
| [13. Kapan Libur](#13-kapan-libur) | ✅
| [14. Nama Epep](#14-nama-epep) | ✅
| [15. Password](#15-password) | ✅
| [16. Qanime](#16-qanime) | ✅
| [17. Qhacker](#17-qhacker) | ✅
| [18. Qislam](#18-qislam) | ✅
| [19. Qpubg](#19-qpubg) | ✅
| [20. Truth](#20-truth) | ✅


## 🎓 How to Use Each Function

### 1. Ai

**Description**:
Interaksi dengan AI Basis Text.

**Args:**
**Description**:
tanya (str): Text inputnya.

**Returns:**
**Description**:
str: Respon chatbotnya.

```python
from ApiNyaEr import apinya

result = await apinya.ai(tanya='Tidur')
print(result)
```

#### Expected Output

```text
Dengan siapa tidur tu?
```

### 2. Ai Image

**Description**:
Generate gambar dari text.

**Args:**
  - **teks (str)**: Kata yang ingin di generate.

**Returns:**
  - **bytes**: Generate di bytes format.

```python
from ApiNyaEr import apinya

result = await apinya.ai_image(teks='Tidur')
print(result)
```

#### Expected Output

```text
name 'time' is not defined
```

### 3. Blackbox

**Description**:
Berinteraksi dengan Blackbox AI untuk menghasilkan konten. 🧠

**Args:**
  - **tanya (str)**: Teks masukan untuk berinteraksi dengan API obrolan Blackbox AI.

**Returns:**
  - **requests.Response**: Objek respons dari permintaan API.

```python
from ApiNyaEr import apinya

result = await apinya.blackbox(tanya='Tidur')
print(result)
```

#### Expected Output

```json
{
    "results": "Generated by BLACKBOX.AI, try unlimited chat https://www.blackbox.ai\n\nTidur adalah proses fisiologis yang penting bagi kesehatan dan kesejahteraan manusia. Selama tidur, tubuh melakukan berbagai fungsi pemulihan, termasuk perbaikan sel, pengaturan hormon, dan penguatan sistem kekebalan tubuh. Tidur yang cukup juga berperan dalam konsolidasi memori dan pengolahan informasi.\n\nAda beberapa tips untuk mendapatkan tidur yang berkualitas:\n\n1. **Tetapkan Jadwal Tidur**: Cobalah untuk tidur dan bangun pada waktu yang sama setiap hari, bahkan di akhir pekan.\n2. **Ciptakan Lingkungan Tidur yang Nyaman**: Pastikan kamar tidur gelap, tenang, dan sejuk.\n3. **Batasi Paparan Layar**: Hindari penggunaan perangkat elektronik setidaknya satu jam sebelum tidur.\n4. **Hindari Kafein dan Makanan Berat**: Konsumsi kafein dan makanan berat menjelang waktu tidur dapat mengganggu kualitas tidur.\n5. **Relaksasi Sebelum Tidur**: Lakukan aktivitas yang menenangkan, seperti membaca atau meditasi, sebelum tidur.\n\nJika Anda memiliki masalah tidur yang berkepanjangan, sebaiknya konsultasikan dengan profesional kesehatan.",
    "join": "@Er_Support_Group",
    "success": true
}
```

### 4. Carbon

**Args:**
  - **query (str)**: Potongan kode yang akan dirender sebagai gambar.

**Description**:
Return: FilePath: Jalur file dari gambar yang disimpan.

```python
from ApiNyaEr import apinya

result = await apinya.carbon(query='Tidur')
print(result)
```

#### Expected Output

```text
/home/runner/work/ApiNyaEr/ApiNyaEr/downloads/carbon_DoVOhMOH.png
```

### 5. Cat

**Description**:
Generate random gambar kucing.

**Returns:**
  - **str or None**: Url random kucing ataupun None; None jika response
    tidak di terima.

```python
from ApiNyaEr import apinya

result = await apinya.cat()
print(result)
```

#### Expected Output

```text
https://cdn2.thecatapi.com/images/22b.jpg
```

### 6. Dare

**Description**:
Dapatkan Kata kata dare

**Returns:**
  - **str**: Random kata dare

```python
from ApiNyaEr import apinya

result = await apinya.dare()
print(result)
```

#### Expected Output

```text
Pake celana kebalik sampe besok paginya.
```

### 7. Doa

**Description**:
Mengambil data doa dari API ItzPire berdasarkan nama doa.

**Args:**
  - **nama_doa (str)**: Nama doa yang ingin diambil.

**Returns:**
  - **str**: Teks doa yang diformat dengan rapi termasuk doa, ayat, latin, dan artinya.

```python
from ApiNyaEr import apinya

result = await apinya.doa(nama_doa='Tidur')
print(result)
```

#### Expected Output

```text
Doa sebelum tidur
Ayat: بِسْمِكَ االلّٰهُمَّ اَحْيَا وَبِاسْمِكَ اَمُوْتُ
Latin: Bismikallaahumma ahyaa wa ammuut
Artinya: Dengan menyebut nama Allah, aku hidup dan aku mati
```

### 8. Dog

**Description**:
Dapatkan random foto anjing.

**Returns:**
  - **str or None**: Url Random anjing jika tersedia; None jika tidak ada
    response yang di terima.

```python
from ApiNyaEr import apinya

result = await apinya.dog()
print(result)
```

#### Expected Output

```text
https://random.dog/824745ce-712d-4085-8fbc-4ec6b8447b8e.jpg
```

### 9. Fakta Unik

**Description**:
Dapatkan random Seputar Fakta Unik

**Returns:**
  - **str**: Random Fakta

```python
from ApiNyaEr import apinya

result = await apinya.fakta_unik()
print(result)
```

#### Expected Output

```text
🌾 *Orang yang cerdas memiliki kadar seng dan tembaga di rambut mereka*
```

### 10. Gemini

**Description**:
Berinteraksi dengan Gemini AI. ✨

**Args:**
  - **tanya (str)**: Teks yang di berikan.

**Returns:**
  - **dict**: dictionaries yang berisi konten ai nya.

```python
from ApiNyaEr import apinya

result = await apinya.gemini(tanya='Tidur')
print(result)
```

#### Expected Output

```json
{
    "results": "**Proses Tidur**\n\nTidur adalah keadaan fisiologis kompleks yang ditandai dengan perubahan kesadaran, pengurangan aktivitas fisik, dan respons sensorik yang berkurang. Proses tidur melibatkan dua jenis tidur utama:\n\n* **Tidur Non-REM (NREM)**: Terdiri dari tiga tahap:\n    * **Tahap N1 (Tidur Ringan)**: Transisi antara bangun dan tidur.\n    * **Tahap N2 (Tidur Sedang)**: Berkurangnya aktivitas otak dan respons sensorik.\n    * **Tahap N3 (Tidur Gelombang Lambat)**: Tidur paling nyenyak, ditandai dengan gelombang otak yang lambat dan amplitudo tinggi.\n* **Tidur REM (Gerakan Mata Cepat)**: Ditandai dengan gerakan mata yang cepat, peningkatan aktivitas otak, dan kelumpuhan otot sementara. Tahap ini sering dikaitkan dengan mimpi.\n\n**Siklus Tidur**\n\nSiklus tidur terdiri dari beberapa tahapan NREM dan REM yang berulang sepanjang malam. Siklus ini biasanya berlangsung sekitar 90-110 menit, dengan 5-6 siklus dalam satu malam.\n\n**Fungsi Tidur**\n\nTidur sangat penting untuk kesehatan fisik dan mental. Beberapa fungsi tidurnya meliputi:\n\n* **Restorasi Fisik**: Memungkinkan tubuh memperbaiki jaringan, mengisi kembali energi, dan melepaskan hormon pertumbuhan.\n* **Fungsi Kognitif**: Penting untuk konsentrasi, memori, dan pembelajaran.\n* **Pengaturan Emosi**: Mengatur suasana hati dan mengurangi stres.\n* **Fungsi Kekebalan**: Memperkuat sistem kekebalan dan membantu melawan penyakit.\n\n**Gangguan Tidur**\n\nGangguan tidur terjadi ketika seseorang mengalami kesulitan tidur atau tetap tertidur. Gangguan umum meliputi:\n\n* Insomia\n* Apnea tidur\n* Sindrom kaki gelisah\n* Narkolepsi\n\nGangguan tidur dapat berdampak signifikan pada kesehatan dan kesejahteraan seseorang. Penting untuk mencari bantuan profesional jika Anda mengalami masalah dengan tidur.\n\n**Tips untuk Tidur yang Baik**\n\n* Tetapkan jadwal tidur yang teratur.\n* Ciptakan lingkungan tidur yang kondusif (gelap, tenang, sejuk).\n* Hindari kafein dan alkohol sebelum tidur.\n* Olahraga teratur (tetapi hindari olahraga berat sebelum tidur).\n* Hindari penggunaan layar (ponsel, tablet, komputer) sebelum tidur.\n* Jika Anda tidak bisa tidur setelah 20 menit, bangunlah dari tempat tidur dan lakukan aktivitas menenangkan sampai Anda merasa lelah.",
    "author": "@chakszzz",
    "success": true
}
```

### 11. Github Search

**Description**:
Pencarian GitHub untuk beberapa tipe konten.

**Args:**
  - **cari (str)**: untuk Pencarian.
  - **tipe (str, optional)**: Type pencarian, terdiri dari:
    - "repositories"
    - "users"
    - "organizations"
    - "issues"
    - "pull_requests"
    - "commits"
    - "topics"

**Description**:
Defaults ke "repositories". max_results (int, optional): Maximum nomor dari results untuk return. Defaultnya 3.

**Returns:**
  - **list**: List dari pencarian results atau pesan error.

```python
from ApiNyaEr import apinya

result = await apinya.github_search(cari='Tidur', tipe='repositories', max_results=3)
print(result)
```

#### Expected Output

```json
[
    {
        "name": "rs-bed-covid-indo-api",
        "full_name": "satyawikananda/rs-bed-covid-indo-api",
        "description": "API ketersediaan rumah sakit dan tempat tidur rumah sakit untuk pasien covid-19 ataupun non-covid yang berada di Indonesia",
        "url": "https://github.com/satyawikananda/rs-bed-covid-indo-api",
        "language": "TypeScript",
        "stargazers_count": 112,
        "forks_count": 25
    },
    {
        "name": "bed-covid-rs-indo",
        "full_name": "hendraaagil/bed-covid-rs-indo",
        "description": "Website yang memberikan informasi terkait ketersediaan rumah sakit dan tempat tidur rumah sakit untuk pasien covid-19 ataupun non-covid di Indonesia.",
        "url": "https://github.com/hendraaagil/bed-covid-rs-indo",
        "language": "JavaScript",
        "stargazers_count": 23,
        "forks_count": 3
    },
    {
        "name": "hobikoding.github.io",
        "full_name": "hobikoding/hobikoding.github.io",
        "description": ":rose: Hobikoding - Mari ngoding sambil tidur",
        "url": "https://github.com/hobikoding/hobikoding.github.io",
        "language": "Makefile",
        "stargazers_count": 3,
        "forks_count": 0
    }
]
```

### 12. Hug

**Description**:
Dapatkan gif Random pelukan dari Nekos.Best API.

**Args:**
  - **amount (int)**: Jumlah gambar nya, Defaultnya 1.

**Returns:**
  - **list**: List dari dictionaries tentang informasi neko image atau GIF.
    Type dictionaries:
    - anime_name (str): Nama anime.
    - url (str): Url gif nya.

```python
from ApiNyaEr import apinya

result = await apinya.hug(amount=1)
print(result)
```

#### Expected Output

```json
[
    {
        "anime_name": "Yuru Yuri",
        "url": "https://nekos.best/api/v2/hug/6ffba377-796c-4157-88a1-82e4b1198340.gif"
    }
]
```

### 13. Kapan Libur

**Description**:
Dapatkan informasi Hari libur kedepan.

**Returns:**
  - **str**: Hari Libur Berikutnya.

```python
from ApiNyaEr import apinya

result = await apinya.kapan_libur()
print(result)
```

#### Expected Output

```text
Hari liburberikutnya adalah Hari Natal yang jatuh di hari Rabu, 25 Desember 2024 (35 hari lagi)
```

### 14. Nama Epep

**Description**:
Dapatkan random nama ep ep

**Returns:**
  - **str**: Random nama ep epnya

```python
from ApiNyaEr import apinya

result = await apinya.nama_epep()
print(result)
```

#### Expected Output

```text
꧁༺༻꧂
```

### 15. Password

**Description**:
Fungsi ini menghasilkan kata sandi acak dengan menggabungkan huruf besar, huruf kecil, tanda baca, dan digit.

**Description**:
Parameters: - num (int): Panjang kata sandi yang dihasilkan. Default adalah 12 jika tidak ditentukan.

**Returns:**
**Description**:
- str: Kata sandi yang dihasilkan secara acak yang terdiri dari karakter dari string.ascii_letters, string.punctuation, dan string.digits.

```python
from ApiNyaEr import apinya

result = await apinya.password(num=12)
print(result)
```

#### Expected Output

```text
M4T>FZgVWbc:
```

### 16. Qanime

**Description**:
Dapatkan Kata kata anime

**Returns:**
  - **str**: Random kata anime

```python
from ApiNyaEr import apinya

result = await apinya.qanime()
print(result)
```

#### Expected Output

```json
{
    "\ud83c\udf81 *Quotes": "Aku tidak suka hubungan yang tidak jelas.*",
    "\ud83c\udf39 *Character": "Hitagi Senjougahara*",
    "\ud83c\udf41 *Anime": "Bakemonogatari*",
    "\ud83c\udf41 *Episode": "Episode 5*"
}
```

### 17. Qhacker

**Description**:
Dapatkan random Quotes Hacker

**Returns:**
  - **str**: Random Quotes Hacker

```python
from ApiNyaEr import apinya

result = await apinya.qhacker()
print(result)
```

#### Expected Output

```text
🃏 *We face cyber threats from state-sponsored hackers, hackers for hire, global cyber syndicates, and terrorists. They seek our state secrets, our trade secrets, our technology, and our ideas - things of incredible value to all of us. They seek to strike our critical infrastructure and to harm our economy.*
```

### 18. Qislam

**Description**:
Dapatkan random Quotes Islamic

**Returns:**
  - **str**: Random Quotes Islam

```python
from ApiNyaEr import apinya

result = await apinya.qislam()
print(result)
```

#### Expected Output

```text
📖 *Akan tiba saatnya sendiri ku menjadi kebahagiaan yang Hakiki*
```

### 19. Qpubg

**Description**:
Dapatkan random Quotes pubg

**Returns:**
  - **str**: Random Quotes Pubg

```python
from ApiNyaEr import apinya

result = await apinya.qpubg()
print(result)
```

#### Expected Output

```text
🏆 *Kami tidak ingin to be a girl’s heart winner. Kami hanya ingin get a chicken dinner*
```

### 20. Truth

**Description**:
Dapatkan Kata kata truth

**Returns:**
  - **str**: Random kata truth

```python
from ApiNyaEr import apinya

result = await apinya.truth()
print(result)
```

#### Expected Output

```text
Jika sebentar lagi kiamat, apa yg kamu lakukan ?
```


This Project is Licensed under [GNU General Public License](https://github.com/ErRickow/ApiNyaEr/blob/Er/LICENSE)