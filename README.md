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
| [1. Ambil Doa](#1-ambil-doa) | ✅
| [2. Blackbox](#2-blackbox) | ✅
| [3. Carbon](#3-carbon) | ✅
| [4. Cat](#4-cat) | ✅
| [5. Chatbot](#5-chatbot) | ✅
| [6. Cohere](#6-cohere) | ✅
| [7. Dare](#7-dare) | ✅
| [8. Dog](#8-dog) | ✅
| [9. Github Search](#9-github-search) | ✅
| [10. Hug](#10-hug) | ✅
| [11. Kapan Libur](#11-kapan-libur) | ✅
| [12. Password](#12-password) | ✅
| [13. Truth](#13-truth) | ✅


## 🎓 How to Use Each Function

### 1. Ambil Doa

**Description**:
Mengambil data doa dari API ItzPire berdasarkan nama doa.

**Args:**
  - **nama_doa (str)**: Nama doa yang ingin diambil.

**Returns:**
  - **str**: Teks doa yang diformat dengan rapi termasuk doa, ayat, latin, dan artinya.

```python
from ApiNyaEr import apinya

result = await apinya.ambil_doa(nama_doa='Tidur')
print(result)
```

#### Expected Output

```text
Doa sebelum tidur
Ayat: بِسْمِكَ االلّٰهُمَّ اَحْيَا وَبِاسْمِكَ اَمُوْتُ
Latin: Bismikallaahumma ahyaa wa ammuut
Artinya: Dengan menyebut nama Allah, aku hidup dan aku mati
```

### 2. Blackbox

**Description**:
Interact with the Blackbox AI API for generating content. 🧠

**Args:**
  - **args (str)**: The input text to interact with the Blackbox AI chat API.

**Returns:**
  - **requests.Response**: The response object from the API request.

```python
from ApiNyaEr import apinya

result = await apinya.blackbox(args='Tidur')
print(result)
```

#### Expected Output

```json
{
    "results": "",
    "join": "@Er_Support_Group",
    "success": true
}
```

### 3. Carbon

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
/home/runner/work/ApiNyaEr/ApiNyaEr/downloads/carbon_dp1AvJt7.png
```

### 4. Cat

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
https://cdn2.thecatapi.com/images/b0b.jpg
```

### 5. Chatbot

**Description**:
Interact with a chatbot to get a response based on the provided input text.

**Args:**
**Description**:
args (str): The text input to the chatbot for generating a response.

**Returns:**
**Description**:
str: The response from the chatbot based on the input text.

**Description**:
Example usage: >>> from MukeshAPI import api >>> user_input = "Hello, how are you?" >>> response = api.chatbot(user_input) >>> print(response)

```python
from ApiNyaEr import apinya

result = await apinya.chatbot(args='Tidur')
print(result)
```

#### Expected Output

```text
Dengan siapa tidur tu?
```

### 6. Cohere

**Description**:
Mengambil respons dari API AI ItzPire berdasarkan pertanyaan yang diberikan menggunakan metode POST.

**Args:**
  - **pertanyaan (str)**: Teks pertanyaan yang akan dikirim ke AI.

**Returns:**
  - **str**: Respons yang dihasilkan oleh AI.

```python
from ApiNyaEr import apinya

result = await apinya.cohere(pertanyaan='Tidur')
print(result)
```

#### Expected Output

```json
{
    "error": "Request failed with status code 429"
}
```

### 7. Dare

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
isi mulut penuh dengan air dan harus tahan hingga dua putaran. Jika tertawa dan tumpah atau terminum, maka harus ngisi ulang dan ditambah satu putaran lagi.
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
https://random.dog/ace571c3-c47e-4c52-93f3-9e3247c62ca9.jpg
```

### 9. Github Search

**Description**:
Pencarian GitHub untuk beberapa tipe konten.

**Args:**
  - **query (str)**: query Pencarian.
  - **search_type (str, optional)**: Type pencarian, terdiri dari:
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

result = await apinya.github_search(query='Tidur', search_type='repositories', max_results=3)
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

### 10. Hug

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
        "anime_name": "Darker Than Black: Ryuusei no Gemini",
        "url": "https://nekos.best/api/v2/hug/1dcc8b20-6420-476f-888e-17c7e09a11fb.gif"
    }
]
```

### 11. Kapan Libur

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

### 12. Password

**Description**:
This function generates a random password by combining uppercase letters, lowercase letters, punctuation marks, and digits.

**Description**:
Parameters: - num (int): The length of the generated password. Default is 12 if not specified.

**Returns:**
**Description**:
- str: A randomly generated password consisting of characters from string.ascii_letters, string.punctuation, and string.digits.'

```python
from ApiNyaEr import apinya

result = await apinya.password(num=12)
print(result)
```

#### Expected Output

```text
)R':fKS-Yz1j
```

### 13. Truth

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
Kapan terakhir kali menangis dan mengapa?
```


This Project is Licensed under [GNU General Public License](https://github.com/ErRickow/ApiNyaEr/blob/Er/LICENSE)