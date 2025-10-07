## 🎹 Klavye Girdi Dinleme (Keyboard Input Logger)

## 🎯 Proje Amacı
Bu proje, **C# Windows Forms** platformunda global klavye tuş dinleme (keyboard hook) mantığını öğretmek amacıyla hazırlanmıştır.  
Amaç, klavyeden girilen karakterleri algılayarak bir metin içinde toplamak ve belirli koşullarda bu veriyi işleyebilmektir.  

> ⚠️ **Not:** Bu proje yalnızca **öğrenme, eğitim ve araştırma** amaçlıdır. Kullanıcının haberi olmadan veri toplamak **kesinlikle yasaktır.**

---

## 🧩 Kullanılan Teknolojiler

| Teknoloji / Kütüphane | Açıklama |
|------------------------|-----------|
| **C# (.NET Framework)** | Ana programlama dili |
| **Windows Forms** | Görsel arayüz ve olay yönetimi |
| **HootKeys** | Global klavye hook işlemleri için |
| **System.Net.Mail** | E-posta gönderimi örneği |
| **user32.dll (DllImport)** | Windows API üzerinden tuş olaylarını dinlemek için |

---

## ⚙️ Çalışma Mantığı

1. Program açıldığında `TuslariDinle()` metodu çalışır ve tüm harf, rakam ve özel karakterleri dinlemeye başlar.  
2. Kullanıcı bir tuşa bastığında `TusKombinasyonu()` metodu devreye girer.  
3. Bu metot, hangi tuşa basıldığına göre `log` değişkenine karakter ekler.  
4. **CapsLock** durumuna göre büyük/küçük harf belirlenir.  
5. 30 karakter girildiğinde `Mail()` fonksiyonu tetiklenir (örnek amaçlı e-posta gönderimi).  

---

## 🧠 Öğrenme Noktaları

- `globalKeyboardHook` kullanımı ile **global klavye dinleme**  
- `DllImport("user32.dll")` ile **Windows API erişimi**  
- `KeyEventArgs` kullanımı ile **klavye olaylarını yakalama**  
- **Türkçe karakter desteği (ğ, ü, ş, ç, ö, İ)** ekleme  
- `System.Net.Mail` ile basit **SMTP üzerinden e-posta gönderme**

---

## 📁 Proje Dosya Yapısı

Logger/
│
├── Form1.cs → Klavye dinleme ve loglama kodları
├── Form1.Designer.cs → Form bileşenleri
├── Program.cs → Ana giriş noktası
└── Logger.csproj → Proje yapı dosyası

yaml
Kodu kopyala

---

## 📬 E-Posta Gönderimi (Öğretimsel Amaçlı)

Projede bulunan `Mail()` metodu, **SMTP protokolü** kullanarak `System.Net.Mail` kütüphanesi üzerinden bir e-posta gönderimi örneği içerir.  
Bu, **iletişim kurma veya veri aktarma mantığını öğretmek** için örnek olarak eklenmiştir.  
Gerçek kullanıcı verilerinin bu yöntemle gönderilmesi **etik değildir**.

---

## ⚖️ Yasal ve Etik Uyarı

Bu yazılım yalnızca **akademik eğitim** amacıyla kullanılmalıdır.  
İzinsiz olarak kişisel verilerin izlenmesi veya kaydedilmesi, **Türk Ceza Kanunu (TCK)** ve **KVKK** kapsamında suç teşkil eder.  
Kod, **“keylogger” mantığını öğretimsel olarak göstermek** için hazırlanmıştır.  

> ❌ Bu projenin izinsiz, kötüye yönelik veya zararlı kullanımı geliştirici tarafından **kesinlikle desteklenmemektedir.**

---

## 👨‍💻 Geliştirici Bilgisi

**👤 Ad:** Enver ALAŞ  
**🧱 Proje Türü:** C# Windows Forms Uygulaması  
**📘 Konu:** Klavye Girdilerini Dinleme ve Analiz Etme  
**🎓 Hazırlanma Amacı:** Yazılım geliştirmede olay yönetimi ve sistem girdisi dinleme mantığını göstermek  

---

## 🧾 Örnek Ekran Görüntüsü (isteğe bağlı)
*(Form1 penceresi veya kod ekranı görseli buraya eklenebilir)*

---
Çalıştığına dair YouTube Video linki :
https://youtu.be/iiL1ex8Xy4E
⭐ Eğer bu projeyi beğendiysen, GitHub’da yıldız vermeyi unutma!
