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
Tidur sama sama.
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
('Error:', 403)
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
    "results": "Generated by BLACKBOX.AI, try unlimited chat https://www.blackbox.ai\n\nTidur adalah proses fisiologis yang penting bagi kesehatan dan kesejahteraan manusia. Selama tidur, tubuh melakukan berbagai pemulihan dan regenerasi, termasuk pemulihan otot, penguatan sistem kekebalan tubuh, dan pengolahan informasi yang diperoleh selama hari. Tidur yang cukup dan berkualitas juga berperan dalam kesehatan mental, konsentrasi, dan suasana hati.\n\nAda beberapa tips untuk mendapatkan tidur yang berkualitas:\n\n1. **Tetapkan Jadwal Tidur**: Cobalah untuk tidur dan bangun pada waktu yang sama setiap hari, bahkan di akhir pekan.\n2. **Ciptakan Lingkungan Tidur yang Nyaman**: Pastikan kamar tidur gelap, tenang, dan sejuk.\n3. **Batasi Paparan Layar**: Hindari penggunaan perangkat elektronik seperti ponsel atau komputer setidaknya satu jam sebelum tidur.\n4. **Hindari Kafein dan Makanan Berat**: Batasi konsumsi kafein dan makanan berat menjelang waktu tidur.\n5. **Relaksasi Sebelum Tidur**: Lakukan aktivitas yang menenangkan seperti membaca, meditasi, atau mandi air hangat.\n\nJika Anda memiliki masalah tidur yang berkepanjangan, sebaiknya konsultasikan dengan profesional kesehatan.",
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
/home/runner/work/ApiNyaEr/ApiNyaEr/downloads/carbon_PRYBggln.png
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
https://cdn2.thecatapi.com/images/bsb.jpg
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
Tuker baju sama orang terdekat sampe ronde berikutnya.
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
https://random.dog/13973-10200-28695.jpg
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
🌾 *Hanya dengan mengurangi brightness dari televisi, anda mampu berhemat lebih dari Rp 1,5 juta setahun. [kompas]*
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
    "results": "**Proses Tidur**\n\nTidur adalah keadaan di mana kesadaran tertekan dan tubuh dan pikiran beristirahat. Ini adalah proses penting yang memungkinkan tubuh untuk memulihkan diri, memperbaiki jaringan, dan mempersiapkan diri untuk hari berikutnya.\n\nTidur melibatkan dua fase utama: tidur Rapid Eye Movement (REM) dan tidur non-Rapid Eye Movement (NREM).\n\n**Tidur NREM**\n\n* Fase terdalam tidur\n* Terdiri dari tiga tahap:\n\n    * **Tahap 1:** Transisi dari bangun ke tidur\n    * **Tahap 2:** Tidur ringan\n    * **Tahap 3:** Tidur nyenyak\n\n* Otot-otot rileks\n* Detak jantung dan pernapasan melambat\n* Suhu tubuh turun\n* Produksi hormon pertumbuhan meningkat\n\n**Tidur REM**\n\n* Tahap tidur yang lebih aktif\n* Dicirikan oleh gerakan mata yang cepat\n* Mimpi terjadi\n* Otot-otot lumpuh\n* Detak jantung dan pernapasan meningkat\n* Suhu tubuh sedikit meningkat\n\n**Siklus Tidur**\n\n* Siklus tidur biasanya berlangsung sekitar 90 menit\n* Terdiri dari beberapa siklus tidur NREM dan REM\n* Tahap tidur NREM menjadi lebih pendek seiring malam sementara tahap REM menjadi lebih panjang\n\n**Manfaat Tidur**\n\n* Pemulihan fisik dan mental\n* Perbaikan jaringan\n* Pengaturan hormon\n* Penguatan memori\n* Peningkatan fungsi kognitif\n* Pengurangan risiko penyakit kronis\n\n**Gangguan Tidur**\n\n* Insomnia (kesulitan tidur)\n* Sleep apnea (berhenti bernapas saat tidur)\n* Sindrom kaki gelisah\n* Tidur berjalan\n\n**Kebutuhan Tidur**\n\nKebutuhan tidur bervariasi tergantung pada usia dan individu. Namun, kebanyakan orang dewasa membutuhkan sekitar 7-9 jam tidur berkualitas setiap malam.\n\n**Tips untuk Tidur Nyenyak**\n\n* Pergi tidur dan bangun pada waktu yang sama setiap hari, bahkan di akhir pekan.\n* Ciptakan lingkungan tidur yang gelap, tenang, dan sejuk.\n* Hindari kafein dan alkohol sebelum tidur.\n* Olahraga teratur, tetapi hindari berolahraga terlalu dekat dengan waktu tidur.\n* Hindari penggunaan perangkat elektronik sebelum tidur karena cahaya biru dapat menekan produksi melatonin.\n* Buat rutinitas waktu tidur yang menenangkan, seperti mandi air hangat atau membaca buku.\n\nTidur yang nyenyak sangat penting untuk kesehatan dan kesejahteraan secara keseluruhan. Jika Anda mengalami kesulitan tidur, konsultasikan dengan dokter Anda untuk menyingkirkan gangguan mendasar.",
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
        "anime_name": "Naruto",
        "url": "https://nekos.best/api/v2/hug/28ba71e1-376d-4d4d-af5b-3aa3ba70943e.gif"
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
꧁฿ิีืÅβγ∞ÐθØŁ꧂
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
k$5TaY-93Dg%
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
    "\ud83c\udf81 *Quotes": "Ada hal yang tak pernah bisa dilihat sebelum melangkah. Karena itu, aku melangkah tanpa rasa takut.*",
    "\ud83c\udf39 *Character": "Itsuki Hashima*",
    "\ud83c\udf41 *Anime": "Imouto sae Ireba Ii.*",
    "\ud83c\udf41 *Episode": "Episode 12*"
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
🃏 *Hackers often describe what they do as playfully creative problem solving. Heather Brooke Problem Creative Often Computer hackers do not need to know each other's real names, or even live on the same continent, to steal millions in mere hours.*
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
📖 *Sahabat adalah orang yang ikhlas bersama kita dalam senang dan susah dan saling menasehati dalam ketaatan kepada Allah*
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
🏆 *Mengendalikan AIM-ku sama susahnya seperti Move On darimu*
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
Quote apa yang paling kamu ingat dan kamu suka?
```


This Project is Licensed under [GNU General Public License](https://github.com/ErRickow/ApiNyaEr/blob/Er/LICENSE)