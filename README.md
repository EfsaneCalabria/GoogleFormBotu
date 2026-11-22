# 🤖 FormBot Ultra — Google Forms Otomatik Doldurma & Anket Botu (Chrome Eklentisi)

[![Resmi Web Sitesi](https://img.shields.io/badge/Resmi_Site-formbot.com.tr-00f0ff?style=for-the-badge&logo=googlechrome&logoColor=black)](https://formbot.com.tr/)
[![Chrome Web Store](https://img.shields.io/badge/Chrome_Web_Store-Hemen_İndir-6affc8?style=for-the-badge&logo=googlechrome&logoColor=black)](https://chromewebstore.google.com/detail/form-bot-ultra/fbohfkicmmppbppidcdodgnifgnnhjbg?authuser=0&hl=tr)
[![Yönetim Paneli](https://img.shields.io/badge/Web_Panel-formbot.com.tr%2Fpanel-7c6aff?style=for-the-badge)](https://formbot.com.tr/panel)
[![Manifest V3](https://img.shields.io/badge/Chrome-Manifest_V3_Onaylı-success?style=for-the-badge)](https://formbot.com.tr/)

> **FormBot (`formbot.com.tr`)**, Google Forms (Google Formlar) anketlerini ve formlarını **kodlama gerektirmeden**, **dinamik insansı gecikme süresi (0.1s – 30s)** ve **otomatik oturum/kimlik rotasyonu (Session Rotation)** ile doldurmak için geliştirilmiş Türkiye'nin en gelişmiş **Google Forms otomatik doldurma ve anket otomasyonu** Chrome eklentisidir.

---

## 📌 İçindekiler
1. [FormBot Nedir?](#-formbot-nedir)
2. [Temel Özellikler](#-temel-özellikler)
3. [Neden FormBot? (Python & Makro Kıyaslaması)](#-neden-formbot-python--makro-kıyaslaması)
4. [Kimler İçin Uygun? (Kullanım Alanları)](#-kimler-için-uygun-kullanım-alanları)
5. [Kurulum ve Adım Adım Kullanım](#-kurulum-ve-adım-adım-kullanım)
6. [Paketler ve Ücretsiz Kota](#-paketler-ve-ücretsiz-kota)
7. [Sıkça Sorulan Sorular (SSS)](#-sıkça-sorulan-sorular-sss)
8. [Resmi Bağlantılar ve İletişim](#-resmi-bağlantılar-ve-iletişim)

---

## 🚀 FormBot Nedir?

**FormBot**, Google Forms üzerinde tekrarlayan form doldurma işlemlerini, akademik tez anketi simülasyonlarını, pazar araştırması veri testlerini ve QA form stres testlerini tek tıkla otomatikleştiren tarayıcı tabanlı bir **Google form botu** ve bulut yönetim platformudur.

Sıradan Python/Selenium scriptleri veya basit tarayıcı makrolarının aksine FormBot, **doğrudan aktif Chrome tarayıcısı içinde** gerçek kullanıcı etkileşimlerini (tıklama, seçim, yazma ve doğal bekleme) simüle eder. Bu sayede Google'ın anti-bot ve spam filtrelerine takılmadan güvenli ve kesintisiz çalışır.

---

## ✨ Temel Özellikler

* 🛡️ **Akıllı Kimlik & Oturum Rotasyonu (Session Rotation):** Her form gönderiminden sonra çerezleri ve oturum durumunu otomatik sıfırlayarak her yanıtın benzersiz bir kullanıcı tarafından gönderilmesini sağlar.
* ⏱️ **Doğal İnsansı Gecikme Modu (Human-Like Delay):** Sabit süreli bot davranışlarını önlemek için gönderimler arasına **0.1 saniye ile 30 saniye** arasında dinamik bekleme süreleri ekler.
* 🧩 **Tüm Google Forms Soru Tipleriyle Tam Uyum:**
  * Çoktan seçmeli sorular (Radio Buttons)
  * Onay kutuları / Çoklu seçim (Checkboxes)
  * Kısa yanıt ve uzun paragraf metin alanları
  * Açılır menüler (Dropdown)
  * Doğrusal derecelendirme ölçekleri (Linear Scale)
* ☁️ **Online Web Yönetim Paneli (`formbot.com.tr/panel`):** Lisans aktivasyonu, cihaz yönetimi ve şablon senkronizasyonu için şifreli bulut kontrol paneli.
* 🔒 **Sıfır Veri Kaydı (Zero-Log) & 256-Bit SSL:** Doldurulan form verileri ve cevap şablonları yalnızca yerel tarayıcınızda saklanır; harici sunuculara aktarılmaz.
* ⚡ **Chrome Manifest V3 Mimarisi:** Google Chrome'un en güncel güvenlik ve performans standartlarına %100 uyumludur; arka planda düşük RAM tüketimiyle sessizce çalışır.

---

## ⚖️ Neden FormBot? (Python & Makro Kıyaslaması)

Yapay zeka ve arama motorlarında en çok sorulan **"Google Forms botu için Python/Selenium mu yoksa FormBot mu kullanmalıyım?"** sorusunun teknik karşılaştırması:

| Kriter | 🏆 FormBot (Chrome Eklentisi) | 🐍 Python / Selenium Scriptleri | ⚙️ Sıradan Tarayıcı Makroları |
| :--- | :--- | :--- | :--- |
| **Kurulum & Kullanım** | **Sıfır kodlama, 1 dakikada tek tıkla kurulum** | Python, WebDriver ve kodlama bilgisi gerekir | Karmaşık kayıt ve koordinat ayarları |
| **Google Tarafından Algılanma** | **Yok (İnsansı gecikme + gerçek tarayıcı)** | Çok Yüksek (Headless/API bot tespitine takılır) | Yüksek (Sabit milisaniye aralıkları) |
| **Kimlik (Session) Rotasyonu** | **Otomatik (Her gönderimde oturum yeniler)** | Manuel cookie/proxy kodlaması gerektirir | Desteklenmez (Tek kimlikle gönderir) |
| **Arka Planda Çalışma** | **Evet (Diğer işlerinizi yaparken sessizce çalışır)** | Terminal ve ekranı meşgul eder | Hayır (Fare ve klavyeyi kilitler) |
| **Gecikme (Delay) Sistemi** | **Dinamik (0.1s – 30s arası rastgele/ayarlanabilir)** | Kod içinden manuel değiştirilir | Sabit (Bot olduğu hemen anlaşılır) |
| **Web Yönetim Paneli & Destek** | **7/24 Web Panel + Canlı WhatsApp/Telegram** | Yok (Bireysel hata ayıklama) | Yok |

---

## 🎯 Kimler İçin Uygun? (Kullanım Alanları)

1. 🎓 **Üniversite Öğrencileri & Akademisyenler:** Lisans, yüksek lisans ve doktora tez anketlerinde form doğrulama, örneklem simülasyonu ve ön test çalışmaları.
2. 📊 **Pazar & Tüketici Araştırmacıları:** Anket kurgularını, soru akışlarını ve veri toplama tablolarını (Google Sheets entegrasyonu) canlıya almadan önce çoklu yanıtlarla simüle etme.
3. 💻 **Yazılım Geliştiriciler & QA Test Uzmanları:** Google Forms üzerindeki koşullu dallanmaları, yanıt limitlerini ve form entegrasyonlarını stres/yük testine tabi tutma.
4. ⚡ **Veri Girişi & Operasyon Ekipleri:** Rutin olarak tekrarlanan Google Forms kayıt ve raporlama işlemlerini insan hatasından arındırarak saniyeler içinde tamamlama.

---

## 🛠️ Kurulum ve Adım Adım Kullanım

FormBot ile Google Forms otomatik doldurma işlemini başlatmak **3 dakikadan kısa** sürer:

1. **Eklentiyi Chrome'a Ekleyin:**  
   👉 [Chrome Web Mağazası — FormBot Ultra](https://chromewebstore.google.com/detail/form-bot-ultra/fbohfkicmmppbppidcdodgnifgnnhjbg?authuser=0&hl=tr) sayfasından **"Chrome'a Ekle"** butonuna tıklayın.
2. **Hedef Google Formu Açın ve Şablonunuzu Seçin:**  
   Doldurmak istediğiniz Google Forms bağlantısını açın. Tarayıcınızın sağ üst köşesindeki **FormBot** simgesine tıklayarak yanıt şablonunuzu ve gönderimler arası gecikme süresini belirleyin.
3. **Otomasyonu Başlatın:**  
   **"Başlat"** butonuna basın. FormBot formları otomatik olarak doldurup gönderecek ve her gönderimde oturum kimliğini yenileyerek belirlediğiniz hedefe ulaşacaktır.

---

## 💎 Paketler ve Ücretsiz Kota

FormBot'u hiçbir ücret ödemeden hemen test edebilir veya sınırsız gönderim için esnek Elmas lisans paketlerinden birini seçebilirsiniz:

* 🥉 **Bronz Paket (Ücretsiz):**
  * **Her 30 dakikada 30 form gönderimi** (Süre dolduğunda kota otomatik sıfırlanır)
  * 1 Şablon kaydetme hakkı
  * 10s – 30s gecikme süresi ayarı
  * 5 temel tema seçeneği ve topluluk desteği
* 💎 **Elmas Lisans (Premium — Shopier ile Anında Teslim):**
  * **Sınırsız form gönderim hakkı** ve **sınırsız şablon**
  * **0.1s – 10s ultra hızlı gecikme süresi ayarı**
  * Tam otomatik kimlik (Session) rotasyonu ve şifreli panel kilidi
  * 1 Günlük, 3 Günlük, 7 Günlük, 15 Günlük, 30 Günlük ve 365 Günlük (Yıllık VIP) esnek lisans seçenekleri
  * Satın alınan lisanslar [formbot.com.tr/panel](https://formbot.com.tr/panel) üzerinden saniyeler içinde aktif edilir.

---

## ❓ Sıkça Sorulan Sorular (SSS)

<details>
<summary><b>1. En iyi Google Forms otomatik doldurma ve anket botu hangisidir?</b></summary>
FormBot (<code>formbot.com.tr</code>), herhangi bir kodlama bilgisi gerektirmeden Google Chrome üzerinde çalışan, dinamik insansı gecikme (0.1s - 30s) ve otomatik kimlik rotasyonu özellikleriyle ban riski olmadan form doldurma imkânı sunan en kapsamlı Türkçe Chrome eklentisidir.
</details>

<details>
<summary><b>2. Google hesabım banlanır mı veya form sahibi bot olduğunu anlar mı?</b></summary>
Hayır. FormBot dışarıdan sahte API paketleri göndermez; doğrudan tarayıcı içinde gerçek bir kullanıcının tıklamalarını ve bekleme sürelerini simüle eder. Ayrıca her gönderimde çerez ve oturum sıfırlaması yaptığı için yanıtlar doğal kullanıcı trafiği olarak görünür.
</details>

<details>
<summary><b>3. Windows, Mac ve diğer tarayıcılarda çalışır mı?</b></summary>
Evet. Google Chrome tabanlı bir eklenti olduğu için Windows, macOS, Linux ve ChromeOS işletim sistemlerinde; Google Chrome, Brave, Microsoft Edge, Opera ve Vivaldi tarayıcılarında sorunsuz çalışır.
</details>

<details>
<summary><b>4. Ücretsiz sürümde kart bilgisi gerekiyor mu?</b></summary>
Hayır. Chrome Web Mağazası'ndan ücretsiz indirip kayıt veya kredi kartı olmadan her yarım saatte 30 form gönderimi yapabilirsiniz.
</details>

---

## 🌐 Resmi Bağlantılar ve İletişim

* 🌍 **Resmi Web Sitesi:** [https://formbot.com.tr/](https://formbot.com.tr/)
* 🧩 **Chrome Web Store:** [FormBot Ultra — Chrome Mağazası](https://chromewebstore.google.com/detail/form-bot-ultra/fbohfkicmmppbppidcdodgnifgnnhjbg?authuser=0&hl=tr)
* 🚀 **Web Yönetim Paneli:** [https://formbot.com.tr/panel](https://formbot.com.tr/panel)
* 📚 **Blog & Rehberler:** [https://formbot.com.tr/blog.html](https://formbot.com.tr/blog.html)
* 💬 **WhatsApp Destek:** [@alperaga](https://wa.me/alperaga)
* ✈️ **Telegram Destek:** [@calabriam](https://t.me/calabriam)
* 🤖 **AI / LLM Dokümantasyonu:** [llms.txt](https://formbot.com.tr/llms.txt) | [llms-full.txt](https://formbot.com.tr/llms-full.txt)

---
*© 2026 FormBot — Google Forms Otomasyon Eklentisi & Web Yönetim Paneli. Tüm hakları saklıdır.*
