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

## 🖼 Örnek Akış Diyagramı

*(Buraya akış görselinizi ekleyebilirsiniz)*  
`![AI Çeviri Akış Diyagramı](images/flow-diagram.png)`

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






🌍 Translate Your Documents Automatically with an AI Translation Agent

In this tutorial, you’ll learn how to build an AI Translation Agent using n8n.
The goal is to automatically translate your documents into multiple languages, preserve original formatting, and connect the entire process with end-to-end automation.

---

## 📚 What You’ll Learn in This Video

✅ How to set up an AI translation agent in n8n

✅ Methods to automatically translate documents into multiple languages

✅ Techniques to preserve original document formatting

✅ How to trigger workflows and process files automatically

✅ Best practices for building AI-powered automation in n8n

---

## 🛠 Tools Used

🔹 **n8n** – Open-source workflow automation tool

🔹 **DeepL API** – AI-powered translation service

🔹 **Google Drive or Local File Trigger** – To automatically detect new file

🔹 **AI Agent Design Patterns** – For building flexible and reusable translation systems

---

## 🚀 Workflow Steps
1. **Define Google Drive folder** – Upload the documents you want to translate into a specific folder.
2. **Download the file** – n8n automatically downloads the file for processing.
3. **Identify file type** – Using a Switch node to detect whether it’s PDF, audio, etc. 
4. **Extract text from PDF** – Convert the PDF content into text format. 
5. **Transcribe audio files** – Use an HTTP Request node to get transcripts from an AI API.  
6. **Format text** – Normalize all outputs into a consistent format with Edit Fields.
7. **Translation process** – Translation process –
8. **AI Agent integration** – Send the translated content to Google Drive as a new document 
9. **Update final document** – Complete the process by updating the translated content in Google Docs.

---

## 🎯 Outcome

Now all you need to do is drop your file into the Google Drive folder.
n8n will automatically download the file, extract the text, translate it with DeepL, and generate a new Google Docs file with the translated content.

---

## 💡 Tips

- Language Detection: Automatically detect the source language to speed up the process without requiring extra user input.
- Batch Processing: Set up workflows to translate multiple documents sequentially or in parallel.
- Error Handling: Add error-catching nodes to manage API limits or connection issues.

---

## 📂 Resources

- [n8n Official Website](https://n8n.io)  
- [DeepL API Documentation](https://developers.deepl.com/)  

> ⚡ This project was created for educational purposes. You can customize the workflow according to your own use case.
