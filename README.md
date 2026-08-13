# Eko-Denge 2053 — COP31 İklim Stratejisti

2026'dan 2053'e on sekiz iklim politikası kararı. Emisyonu düşürürken bütçeyi, enerji arzını ve
kalkınmayı ayakta tutabilir misiniz? Doksan saniye sürer, telefonda çalışır.

**XOX Games** · T.C. Çevre, Şehircilik ve İklim Değişikliği Bakanlığı için · COP31 Antalya, 9–20 Kasım 2026

---

## ⚠️ Yayına almak için iki adım kaldı — toplam ~1 dakika

`404.html` ve `robots.txt` yüklendi. Geriye üç dosya ve tek bir ayar kaldı.

### 1. Üç dosyayı yükleyin

`YUKLE-BU-3-DOSYAYI.zip` dosyasını açın, içinden çıkan üç dosyayı bu deponun köküne yükleyin:

| Dosya | Boyut | Ne işe yarar |
|---|---|---|
| `index.html` | 452 KB | **Oyunun tamamı.** Tek dosya, görseller içinde gömülü |
| `og-onizleme.jpg` | 142 KB | Bağlantı paylaşınca çıkan önizleme kartı |
| `qr.html` | 27 KB | Bağlantı kiti — QR ve sunum metinleri üretir |

**Nasıl:** Bu sayfadaki **Add file → Upload files** düğmesine basın · üç dosyayı pencereye
sürükleyip bırakın · aşağıdaki yeşil **Commit changes** düğmesine basın.

### 2. Pages'i açın

**Settings** → sol menüde **Pages** → *Source*: **Deploy from a branch** →
Branch: **main**, klasör: **/ (root)** → **Save**

İki üç dakika içinde adres hazır olur:

### 🔗 https://tarikbugra2323.github.io/eko-denge-2053/

---

## Yayından sonra üç şey

**QR kodunu üretin.** `https://tarikbugra2323.github.io/eko-denge-2053/qr.html` adresini açın,
oyunun adresini yapıştırın. QR'ı PNG olarak indirir; slayt altı, sunum notu ve basın bülteni için
üç uzunlukta hazır metin verir. Sunumda QR en az 5 cm, ekranda göstereceksiniz 10 cm olmalı.

**Önizleme görselini tam adrese çevirin.** `index.html` içinde `og:image` ve `twitter:image`
satırları dosyayı göreli adresle gösteriyor. WhatsApp, Slack, LinkedIn ve Telegram bunu çözer;
her platformda garanti olsun isterseniz iki satırı da şununla değiştirin:

```html
content="https://tarikbugra2323.github.io/eko-denge-2053/og-onizleme.jpg"
```

**Kendi alan adınızı bağlayın.** Sunumda `ekodenge.xoxgames.io` görünmesi, bir GitHub adresinden
daha iyi durur. Settings → Pages → *Custom domain* kısmına yazın, DNS'te bir CNAME kaydı açın.
Oyun aynı kalır, sadece adres değişir — QR'ı bir kez, alan adı bağlandıktan sonra üretin.

---

## Adres parametreleri

| Parametre | Etkisi |
|---|---|
| `?lang=tr` | Türkçe açılmaya zorlar |
| `?lang=en` | İngilizce açılmaya zorlar |
| `?tasarim=1` | Ergonomi bindirmesini ve tasarım panelini gösterir |

Parametre yoksa tarayıcı diline bakar: Türkçe değilse İngilizce açılır.

---

## Sunum öncesi kontrol listesi

- [ ] Adresi telefonda açın — dikey tam ekran gelmeli
- [ ] Bir kartı sağa, bir kartı sola kaydırın
- [ ] Kartın sağ ve sol yarısına dokunarak da karar verin
- [ ] Adresi kendinize WhatsApp'tan gönderin — önizleme kartı çıkmalı
- [ ] `?lang=en` ile açıp İngilizce metinleri kontrol edin
- [ ] QR'ı yazdırıp telefonla okutun

---

## Teknik notlar

- Tek dosya, tamamen statik. Sunucu tarafı kod, veritabanı, çerez, harici istek yok.
- Ziyaretçiden hiçbir veri toplanmaz.
- Kart metinleri ve denge değerleri COP31 saha kioskuyla birebir aynıdır — ikisi de aynı
  kaynak modelden üretilir.
- 18 kart × 2 seçenek = **262.144 karar yolunun tamamı** simüle edilerek denge doğrulanmıştır;
  21 seçenek çiftinin 21'i de gerçek takas içerir, tek taraflı kart yoktur.
- Türkçe ve İngilizce tam yerelleştirme.
- Dokunma, kaydırma, klavye (← →) ve arcade buton girişleri desteklenir.
- Her kartın dayandığı resmî belge ekranda kaynak etiketi olarak gösterilir.
