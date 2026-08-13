# Eko-Denge 2053 — COP31 İklim Stratejisti

2026'dan 2053'e on sekiz iklim politikası kararı. Emisyonu düşürürken bütçeyi, enerji arzını ve
kalkınmayı ayakta tutabilir misiniz? Doksan saniye sürer, telefonda çalışır.

**XOX Games** · T.C. Çevre, Şehircilik ve İklim Değişikliği Bakanlığı için · COP31 Antalya, 9–20 Kasım 2026

---

## ⚠️ Kurulum: iki adım kaldı

Bu depo şu an boş. Oyun dosyalarını yükleyip Pages'i açmanız gerekiyor — toplam ~1 dakika.

### 1. Dosyaları yükleyin

`Eko-Denge-2053_Web-Yayin-Paketi.zip` dosyasını bilgisayarınızda açın. İçinden çıkan **5 dosyayı**
bu deponun köküne yükleyin:

| Dosya | Ne işe yarar |
|---|---|
| `index.html` | Oyunun tamamı — tek dosya, 462 KB, görseller içinde gömülü |
| `og-onizleme.jpg` | Bağlantı paylaşınca çıkan önizleme kartı |
| `404.html` | Yanlış adrese gireni ana sayfaya yollar |
| `robots.txt` | Arama motorlarına açık |
| `qr.html` | Bağlantı kiti — adresi yapıştırın, QR ve sunum metinleri üretsin |

**Nasıl:** Yukarıdaki **Add file → Upload files** düğmesine basın, beş dosyayı sürükleyip bırakın,
sayfanın altındaki **Commit changes** düğmesine basın.

### 2. Pages'i açın

**Settings** → sol menüden **Pages** → *Source* altında **Deploy from a branch** →
Branch: **main**, klasör: **/ (root)** → **Save**.

Bir iki dakika içinde adresiniz hazır olur:

```
https://tarikbugra2323.github.io/eko-denge-2053/
```

---

## Yayından sonra

**Önizleme görselini tam adrese çevirin.** `index.html` içinde `og:image` ve `twitter:image`
satırları `og-onizleme.jpg` dosyasını göreli adresle gösteriyor. WhatsApp, Slack, LinkedIn ve
Telegram bunu çözer; her platformda garanti olsun isterseniz iki satırı da şununla değiştirin:

```html
content="https://tarikbugra2323.github.io/eko-denge-2053/og-onizleme.jpg"
```

**QR kodu üretin.** `qr.html` sayfasını açın, yukarıdaki adresi yapıştırın. QR'ı PNG olarak indirir,
üç uzunlukta hazır sunum metni verir. Sunumda QR en az 5 cm olmalı.

**Kendi alan adınızı bağlayabilirsiniz.** Settings → Pages → Custom domain kısmına
`ekodenge.xoxgames.io` yazıp DNS'te bir CNAME kaydı açmanız yeterli. Adres değişse de
oyun aynı kalır.

---

## Adres parametreleri

| Parametre | Etkisi |
|---|---|
| `?lang=tr` | Türkçe açılmaya zorlar |
| `?lang=en` | İngilizce açılmaya zorlar |
| `?tasarim=1` | Ergonomi bindirmesi ve tasarım panelini gösterir |

Parametre verilmezse tarayıcı diline bakar: Türkçe değilse İngilizce açılır.

---

## Teknik notlar

- Tek dosya, statik. Sunucu tarafı kod, veritabanı, çerez, harici istek yok.
- Ziyaretçiden hiçbir veri toplanmaz.
- Kart metinleri ve denge değerleri saha kioskuyla birebir aynıdır — ikisi de aynı kaynak
  modelden (`deck.py`) üretilir.
- 18 kart × 2 seçenek = 262.144 karar yolunun tamamı simüle edilerek denge doğrulanmıştır.
- Türkçe ve İngilizce tam yerelleştirme.
- Dokunma, kaydırma, klavye (← →) ve arcade buton girişleri desteklenir.
