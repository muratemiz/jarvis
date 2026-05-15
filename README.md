<div align="center">

# J.A.R.V.I.S

**Gemini Live API destekli macOS kişisel AI asistanı**

[![Python](https://img.shields.io/badge/Python-3.11+-3776AB?style=flat&logo=python&logoColor=white)](https://python.org)
[![Gemini](https://img.shields.io/badge/Gemini-Live_API-4285F4?style=flat&logo=google&logoColor=white)](https://ai.google.dev)
[![macOS](https://img.shields.io/badge/macOS-12+-000000?style=flat&logo=apple&logoColor=white)](https://apple.com/macos)
[![License](https://img.shields.io/badge/Lisans-MIT-green?style=flat)](LICENSE)

*Yapımcı: [Murat Temiz](https://linkedin.com/in/temizmurat) · [GitHub](https://github.com/muratemiz)*

</div>

---

## Özellikler

| Kategori | Yetenekler |
|---|---|
| **Yapay Zeka** | Sesli & yazılı komut, Türkçe/İngilizce, ekran analizi |
| **Takvim & Hatırlatıcı** | Apple Takvim & Hatırlatıcılar okuma/ekleme/silme |
| **Müzik & Medya** | YouTube, Spotify, Apple Music kontrolü |
| **WhatsApp** | Mesaj gönderme, rehber kaydetme |
| **Tarayıcı** | Google arama, URL açma, hava durumu |
| **Uygulama Açma** | Yüklü tüm Mac uygulamalarını sesli açma |
| **Sistem Bilgisi** | Pil, CPU, RAM, disk, saat |
| **Bellek** | Konuşmalar arası kalıcı hafıza |
| **Terminal** | Güvenli shell komutları çalıştırma |
| **YouTube Analiz** | Kanal istatistikleri ve video performansı |

---

## Kurulum

### 1. Gereksinimler

- macOS 12+
- Python 3.11+
- [Gemini API Key](https://aistudio.google.com/app/apikey)

### 2. Kurulum

```bash
git clone https://github.com/muratemiz/jarvis.git
cd jarvis

# Sanal ortam oluştur ve aktif et
python3 -m venv venv
source venv/bin/activate

# Bağımlılıkları yükle
pip install -r requirements.txt
```

### 3. API Anahtarını Ayarla

```bash
cp config/api_keys.example.json config/api_keys.json
```

`config/api_keys.json` dosyasını düzenle:

```json
{
  "gemini_api_key": "BURAYA_GEMINI_API_KEY",
  "voice": "Charon",
  "youtube_api_key": "",
  "youtube_channel_handle": ""
}
```

### 4. Çalıştır

```bash
source venv/bin/activate
python main.py
```

---

## Kullanım

| Komut Örneği | Eylem |
|---|---|
| `"Spotify'ı aç"` | Spotify'ı açar |
| `"Hava durumu nedir?"` | Bulunduğun şehrin hava durumunu söyler |
| `"Yarın takvimimde ne var?"` | Apple Takvim'i okur |
| `"Annem'e iyi geceler mesajı gönder"` | WhatsApp ile mesaj atar |
| `"YouTube'da lo-fi çal"` | YouTube'da müzik açar |
| `"Pil durumu nedir?"` | Pil yüzdesini söyler |
| `"Ekranda ne var?"` | Ekran görüntüsü alıp analiz eder |
| `"Bunu hatırla: ..."` | Kalıcı belleğe kaydeder |

**Kısayollar:** `F4` veya `Cmd+M` → Mikrofonu sustur/aç

---

## Bağımlılıklar

```
google-genai
SpeechRecognition
pyaudio
psutil
Pillow
requests
```

---

## Lisans

MIT License — dilediğin gibi kullanabilirsin.
