# nRF24L01_Button_LED
nRF24L01 ile butonla LED kontrolü yapan Arduino projesi.
# 🚀 Arduino ile Kablosuz LED Kontrol Sistemi | nRF24L01 Projesi

Bu projede, **iki Arduino** ve **nRF24L01** modülü kullanarak **butona basıldığında uzaktaki bir LED'in yanması** sağlanmıştır. Kablosuz iletişimle haberleşme gerçekleştirilmiştir.

## 🎥 Demo Videosu

🔗 [YouTube'da İzle](https://youtube.com/shorts/GKl5gDIJ_Pc?si=fzDZyPGvHIjpchd7)

## 🧰 Kullanılan Malzemeler

- Arduino UNO (2 adet)
- nRF24L01 Modülü (2 adet)
- Push Button (1 adet)
- LED + 220Ω direnç
- Breadboard ve jumper kablolar

## 📡 Proje Amacı

> Bir Arduino'daki butona basıldığında, diğer Arduino'daki LED yanar. Bu iletişim nRF24L01 üzerinden **kablosuz** olarak gerçekleşir.

## 🔌 Devre Şeması

**Verici (Transmitter):**
- Buton: D2 pinine
- nRF24L01: CE → D9, CSN → D10, VCC → 3.3V

**Alıcı (Receiver):**
- LED: D7 pinine
- nRF24L01: CE → D9, CSN → D10, VCC → 3.3V

## 🧠 Kod Yapısı

- `transmitter.ino` → Buton bilgisi okunur, kablosuz olarak gönderilir.
- `receiver.ino` → Gelen bilgiye göre LED açılır veya kapanır.

## 🛠️ Nasıl Kullanılır?

1. Arduino IDE ile `.ino` dosyalarını yükle.
2. Devreleri şemaya göre kur.
3. Her iki Arduino'yu farklı portlara bağla.
4. Güç verildiğinde sistem otomatik çalışacaktır.
![WhatsApp Görsel 2025-07-17 saat 05 06 43_cefc56a3](https://github.com/user-attachments/assets/0df213e6-2e53-4c21-9cb7-3cb745d22c42)


## 📁 Dosyalar

- `transmitter.ino` – Verici kodu
- `receiver.ino` – Alıcı kodu
- `devre.jpg` – Bağlantı şeması

## 📢 Katkı

Proje geliştirmeye açıktır. Sorular, öneriler ve katkılar için pull request gönderebilirsiniz.

---

📌 **Bu basit proje ile kablosuz iletişimin temel mantığını öğrenebilir, daha büyük sistemler için temel oluşturabilirsiniz.**

