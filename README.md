# Silent Protocol Automation

Skrip ini digunakan untuk otomatisasi ping dan pengecekan posisi dalam Silent Protocol Ceremony.

## 📌 Repository
Repository GitHub: [Silent-Protocol](https://github.com/isorganic/Silent-Protocol)

## ⚙️ Instalasi di Termux

### 1️⃣ Update dan Install Dependencies
```bash
pkg update && pkg upgrade -y
pkg install python -y
pkg install git -y
pip install requests
```

### 2️⃣ Clone Repository
```bash
git clone https://github.com/isorganic/Silent-Protocol.git
cd Silent-Protocol
```

### 3️⃣ Tambahkan Token
```bash
touch tokens.txt
nano tokens.txt
```
Tambahkan token ke dalam `tokens.txt`, satu token per baris, lalu simpan.

### 4️⃣ Jalankan Skrip
```bash
python automation.py
```
Jika menggunakan Python 3:
```bash
python3 automation.py
```

## 🚀 Menjalankan di Background
Untuk menjalankan skrip tanpa terputus:
```bash
apt install screen -y
screen -S Silent-Protocol
python3 automation.py
```
Tekan `CTRL + A`, lalu `D` untuk keluar dari screen tanpa menghentikan skrip.

Untuk kembali ke screen:
```bash
screen -r Silent-Protocol
```

## ⚙️ Instalasi di CMD Windows

### 1️⃣ Install Python dan Git
Unduh dan instal:
- [Python](https://www.python.org/downloads/)
- [Git](https://git-scm.com/downloads)

Pastikan Python dan pip telah ditambahkan ke `PATH`.

### 2️⃣ Clone Repository
Buka CMD dan jalankan:
```cmd
git clone https://github.com/isorganic/Silent-Protocol.git
cd Silent-Protocol
```

### 3️⃣ Install Dependencies
```cmd
pip install requests
```

### 4️⃣ Tambahkan Token
Buka file `tokens.txt` dengan Notepad atau editor teks lainnya, lalu masukkan token satu per baris.

### 5️⃣ Jalankan Skrip
```cmd
python automation.py
```
Jika menggunakan Python 3:
```cmd
python3 automation.py
```

## 📌 Catatan
- Pastikan token telah dimasukkan dengan benar ke dalam `tokens.txt`
- Jika ada error `ModuleNotFoundError: No module named 'requests'`, jalankan:
  ```cmd
  pip install requests
  ```

