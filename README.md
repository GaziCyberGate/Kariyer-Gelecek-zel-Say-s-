<div align="center">

# 🛡️ ShadowScan  
### **Multi-Threaded Port Scanner**  
**“Ağlarınızdaki gölgeleri aydınlatın.”**

<img src="https://img.shields.io/badge/Python-3.10+-blue.svg" />
<img src="https://img.shields.io/badge/Status-Active-brightgreen.svg" />
<img src="https://img.shields.io/badge/License-MIT-yellow.svg" />

</div>

---

## 📖 Proje Hakkında  

ShadowScan, ağ yapılarındaki açık portları hızlı ve verimli bir şekilde tespit etmek amacıyla geliştirilmiş çok iş parçacıklı bir port tarayıcıdır.  
Soket programlamayı ve ağ protokollerini derinlemesine anlamak için tasarlanmış olan bu araç, klasik port tarayıcılara göre çok daha hızlı çalışır ve sonuçları anlık olarak raporlar.

Bu proje; siber güvenlik meraklıları, sistem yöneticileri ve ağ analiz süreçlerini hızlandırmak isteyen herkes için güçlü bir yardımcıdır.

---

## ✨ Özellikler

### 🚀 **Hızlı Çoklu Tarama**
- Multi-threading yapısı sayesinde aynı anda **100 portu** tarayabilir.  
- Bekleme sürelerini minimize eder, sonuçları eşzamanlı sunar.

### 🔍 **Servis Tespiti (Banner Grabbing)**
- Açık portlarda çalışan servisleri otomatik olarak analiz eder.  
- Hangi servisin hangi imzayı verdiğini tespit ederek keşif sürecini hızlandırır.

### 🎯 **Hedefe Yönelik Tarama Modları**
- Tekil IP taraması  
- IP aralığı taraması  
- Manuel port aralığı belirtme  

### 📝 **Raporlama ve Loglama**
- Sonuçları `.txt` veya `.csv` formatında dışa aktarabilir.  
- Büyük ağlarda log saklama ve analiz süreçlerini kolaylaştırır.

### ⚡ Hafif ve Esnek Tasarım
- Minimal bağımlılık ile çalışır.  
- Hızlı kurulum, kolay kullanım.

---

## ▶️ Kullanım Rehberi

🔸 Temel Tarama

Belirli bir hedef IP adresini hızlıca tarar:

```bash
python shadowscan.py -t 192.168.1.10 
 ```

🔸 Port Aralığı Belirleme

Kapalı/açık kontrolü için özel port aralığı:

```bash
python shadowscan.py -t 192.168.1.10 -p 1-1000
 ```
🔸 IP Aralığı Taraması

Geniş ağ bloklarının keşfi için:

```bash
python shadowscan.py -r 192.168.1.1-192.168.1.255
 ```

🔸 IP Aralığı Taraması

Geniş ağ bloklarının keşfi için:

```bash
python shadowscan.py -r 192.168.1.1-192.168.1.255
 ```

🔸 Rapor Çıktısı Alma

Sonuçları .csv formatında saklama:

```bash
python shadowscan.py -t 192.168.1.10 --export results.csv
 ```

## 📦 Kurulum

ShadowScan, Python 3.10+ ile uyumlu olacak şekilde geliştirilmiştir.


### 1️⃣ Depoyu Klonlayın

```bash
git clone https://github.com/kullaniciadi/ShadowScan.git
cd ShadowScan bash
 ```

### 2️⃣ Gerekli Bağımlılıkları Yükleyin

```bash
pip install -r requirements.txt

 ```

## 📂 Proje Yapısı

```bash
ShadowScan/
│
├── shadowscan.py       
├── utils/               
│   ├── scanner.py
│   ├── reporter.py
│   └── banners.py
│
├── reports/             
│
├── README.md            
├── requirements.txt     
└── LICENSE              

 ```






