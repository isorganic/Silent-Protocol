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

## 📌 Catatan
- Pastikan token telah dimasukkan dengan benar ke dalam `tokens.txt`
- Jika ada error `ModuleNotFoundError: No module named 'requests'`, jalankan:
  ```bash
  pip install requests
  ```

