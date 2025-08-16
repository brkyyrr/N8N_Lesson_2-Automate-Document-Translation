# AI Çeviri Ajanı ile Belgelerinizi Otomatik Olarak Çevirin

Bu eğitimde, **n8n** kullanarak bir **AI Çeviri Ajanı** oluşturmayı öğreneceksiniz.  
Amacımız, farklı dillerdeki belgelerinizi otomatik olarak çevirmek, orijinal biçimlendirmeyi korumak ve tüm süreci uçtan uca otomasyona bağlamaktır.

---

## 📚 Bu Videoda Öğrenecekleriniz

✅ n8n üzerinde AI çeviri ajanı kurulum adımları  
✅ Belgeleri birden fazla dile otomatik olarak çevirme yöntemleri  
✅ Orijinal belge biçimlendirmesini koruma teknikleri  
✅ İş akışlarını tetikleme ve dosyaları otomatik olarak işleme süreci  
✅ n8n üzerinde AI destekli otomasyon kurulumunda en iyi uygulamalar

---

## 🛠 Kullanılan Araçlar

🔹 **n8n** – Açık kaynak iş akışı otomasyon aracı  
🔹 **DeepL API** – Yapay zeka destekli çeviri hizmeti  
🔹 **Google Drive** veya Yerel Dosya Tetikleyici – Belgeleri otomatik algılamak için  
🔹 **AI Agent Design Patterns** – Daha esnek ve yeniden kullanılabilir çeviri sistemleri kurmak için

---

## 🚀 Sürecin Adımları

1. **Google Drive klasörü tanımlama** – Çevirmek istediğiniz dosyaları belirli bir klasöre yüklüyorsunuz.  
2. **Dosyayı indirme** – n8n dosyayı işlemek üzere indiriyor.  
3. **Dosya türünü ayırt etme** – Switch node ile eklenen dosyanın türünü kontrol ediyoruz (PDF, ses, vb.).  
4. **PDF’den metin çıkarma** – PDF içeriği text dosyasına dönüştürülüyor.  
5. **Ses dosyalarını metne çevirme** – HTTP Request ile AI API üzerinden transcript alınıyor.  
6. **Text düzenleme** – Tüm çıktılar `Edit Fields` ile tek formatta hazırlanıyor.  
7. **Çeviri işlemi** – DeepL API kullanılarak farklı dillere çeviri yapılıyor.  
8. **AI Agent entegrasyonu** – Çevrilen içerik Google Drive üzerinde yeni bir dokümana aktarılıyor.  
9. **Son dokümanı güncelleme** – Çevrilmiş içerik ile Google Docs üzerinde dosya tamamlanıyor.  


---

## 🎯 Sonuç
Artık sadece dosyayı Google Drive klasörüne atmanız yeterli.  
n8n, dosyayı otomatik indirir, metne çevirir, DeepL ile istediğiniz dile aktarır ve Google Docs üzerinde düzenlenmiş halini oluşturur.  

---

## 💡 İpuçları

- **Dil Algılama**: Kaynak dili otomatik tespit ederek kullanıcıdan ekstra bilgi istemeden süreci hızlandırabilirsiniz.  
- **Toplu İşleme**: Birden fazla belgeyi sırayla veya paralel olarak çevirecek iş akışları kurabilirsiniz.  
- **Hata Yönetimi**: API limitleri veya bağlantı hataları için hata yakalama düğümleri ekleyin.

---

## 📂 Kaynaklar

- [n8n Resmi Sitesi](https://n8n.io)  
- [DeepL API Dokümantasyonu](https://developers.deepl.com/)  


---

> Bu proje eğitim amaçlı hazırlanmıştır. Akışınızı kendi kullanım senaryonuza göre özelleştirebilirsiniz.
