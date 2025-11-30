# KARAKTER TABANLI HAYATTA KALMA SİMÜLATÖRÜ

Bu proje, C dili kullanılarak geliştirilmiş metin tabanlı bir **hayatta
kalma oyunu**dur. Oyuncu; sağlık, enerji, yemek ve konum gibi değerleri
yöneterek hayatta kalmaya çalışır. Oyunda komut sistemi, döngüler,
koşullar, fonksiyonlar ve rastgelelik kullanılmıştır.

## 🎮 Oyun Özeti

Oyuncu şu eylemleri yapabilir: - Avlanmak - Dinlenmek - Tehlike
dalgasından kaçmak - Şifre çözerek ilerlemek - Vakit geçirmek -
Envanteri görüntülemek - Haritada ilerlemek

Her komut sağlık, enerji ya da envanter üzerinde etkiler oluşturur.

## 🔧 Kullanılan Yapılar

-   Fonksiyonlar\
-   Switch-Case\
-   If-Else\
-   For döngüsü\
-   Do-While döngüsü\
-   Global değişkenler\
-   Rastgele sayı üretimi (rand(), srand())

## 📌 Komutlar

  Komut   Açıklama
  ------- ---------------------
  A       Avlan
  V       Vakit geçir
  S       Saklan
  R       Dinlen
  E       Envanteri görüntüle
  F       Tehlike dalgası
  P       Şifreli ilerleme
  X       Oyundan çık

## 💥 Önemli Mekanikler

### Avlanma

-   %60 başarı şansı\
-   Başarı -\> 1--3 yemek\
-   Enerji azalır

### Saklanma
Başarılı olma ihtimali şu şartlara bağlıdır:

silah_var == 1 || (harita_konumu < 3 && enerji > 90)

Başarılı olursa +3 enerji, başarısız olursa -5 sağlık.

### Dinlenme
- Sağlık +10
- Enerji +15

### Envanter
- Yemek sayısı ve silah durumu görüntülenir.

### Tehlike Dalgası

-   5 aşamalı saldırı simülasyonu\
-   %70 kaçma şansı\
-   Kacılmazsa artan hasar\
-   Kritik durumda otomatik yemek kullanılır

### Şifreli İlerleme

-   Doğru karakter girilene kadar döngü devam eder\
-   Yanlışsa enerji kaybı olur


    ├── main.c
    └── README.md

## 📝 Lisans

Eğitim amaçlıdır, serbestçe kullanılabilir.
