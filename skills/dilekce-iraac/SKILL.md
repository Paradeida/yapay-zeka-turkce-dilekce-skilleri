---
name: dilekce-iraac
description: >-
  IRAAC / IRRAC (Issue → Rule → Application → (counter-)Application → Conclusion /
  Mesele → Kural → Uygulama → Karşı-Uygulama → Sonuç; varyant: Issue → Rule →
  (second) Rule → Application → Conclusion) yöntemiyle Türk hukukunda dilekçe ve
  savunma hazırlamak için kullanılır. Tetikleyiciler: "IRAAC yöntemiyle dilekçe",
  "IRRAC ile cevap/replik", "karşı argümanı çürüten dilekçe", "counter-analysis".
  İki taraflı ve tartışmalı meselelerde karşı tarafın olası argümanını öngörüp
  çürütmek (çift A) veya ikinci/alternatif kural ekseni kurmak (çift R) için
  güçlüdür. Çıktı docx/html/udf/pdf üretilir.
---

# IRAAC / IRRAC ile Dilekçe Oluşturma

IRAAC, IRAC'e ikinci bir **Uygulama (Application)** ekleyerek karşı tarafın olası
argümanını baştan öngörüp çürüten (counter-analysis); IRRAC ise ikinci bir
**Kural (Rule)** ekleyerek alternatif/ek dayanak ekseni kuran bir analiz/yazım
şemasıdır. İki taraflı, tartışmalı meselelerde — özellikle karşı tarafın
savunmasına önceden karşılık verilmek istendiğinde — güçlüdür.

## Ne zaman kullanılır

- İki taraflı ve tartışmalı mesele; karşı tarafın olası argümanını baştan çürütmek gerekiyor.
- Cevap, replik (cevaba cevap) veya düplik (ikinci cevap) yazılıyor; karşılıklı iddialar örülecek.
- Talep, ana kuralın yanında ikinci/alternatif bir hukuki dayanağa da bağlanacak (IRRAC).
- Karşı tarafın muhtemel savunması öngörülebiliyor ve önden kırılması taktik üstünlük sağlıyor (IRAAC).

## IRAAC / IRRAC mantığı

1. **I — Mesele (Issue):** Çözülecek hukuki soruyu net koy.
2. **R — Kural (Rule):** Uygulanacak mevzuat/içtihat/ilke.
3. **A — Uygulama (Application):** Kuralı somut vakıalara tatbik et (asıl iddia).
4. **A / R — Karşı-Uygulama veya İkinci Kural:**
   - **IRAAC (çift A):** Karşı tarafın olası argümanını öngör ve çürüt (counter-analysis).
   - **IRRAC (çift R):** Asıl kuralı destekleyen ikinci/alternatif kuralı ekle.
5. **C — Sonuç (Conclusion):** Asıl uygulama ile karşı-uygulama/ikinci kuralı birleştiren varış.

## Çalışma akışı

1. **Dilekçe türünü belirle** (dava/cevap/replik/düplik/savunma) — `references/bicim-ve-cikti.md`.
2. **Bilgileri topla:** mahkeme ve dosya no, taraflar, konu, talepler, vakıalar, deliller.
   Eksikleri `AskUserQuestion` veya kısa sorularla tamamla. Dava dosyası verildiyse oku:
   `.udf` → `udf-cli udf2md`; çok sayfalı `.tiff/.tif` → sayfalara böl, tek tek oku; PDF/foto/metin → doğrudan oku.
3. **Varyantı seç ve iskeleti kur:** Karşı argüman öngörülecekse **IRAAC** (çift A), ikinci/alternatif
   dayanak eklenecekse **IRRAC** (çift R). Adım tanımları ve eşleme için `references/cerceve-yapisi.md`.
4. **Gövdeyi yaz:** AÇIKLAMALAR'ı `I → R → A → A/R → C` akışıyla başlıklandır. IRAAC'te karşı
   tarafın olası iddiasını "Karşı tarafın iddiasının aksine..." alt başlığıyla öngörüp çürüt;
   IRRAC'te ikinci kuralı HUKUKİ NEDENLER'de ek dayanak olarak göster. Her mesele için ayrı blok kurabilirsin.
5. **Çıktıyı üret** (docx/html/udf/pdf) — `references/bicim-ve-cikti.md`.
6. **Doğrula ve sun.**

## IRAAC / IRRAC adımlarının dilekçe bölümlerine eşlemesi

| IRAAC/IRRAC adımı | Dilekçe bölümü | İçerik |
|-------------------|----------------|--------|
| Mesele | Her bölümün başı | Çözülecek hukuki soru (tek cümle) |
| Kural | HUKUKİ NEDENLER (+ gövdede atıf) | Dayanak mevzuat/içtihat/ilke |
| Uygulama | AÇIKLAMALAR (irdeleme) | Kuralın somut vakıalara tatbiki (asıl iddia) |
| Karşı-Uygulama (IRAAC) | AÇIKLAMALAR — "Karşı tarafın iddiasının aksine..." | Karşı argümanı öngörüp çürütme |
| İkinci Kural (IRRAC) | HUKUKİ NEDENLER (ek dayanak) | Alternatif/destekleyici hukuki eksen |
| Sonuç | Bölüm sonu + NETİCE VE TALEP | Asıl + karşı-uygulama/ikinci kuralı birleştiren varış |

## Çıktı formatları

docx (varsayılan) · html (standalone) · udf (UYAP) · pdf. Ayrıntı: `references/bicim-ve-cikti.md`.

## Doğrulama listesi

- Mesele → Kural → Uygulama → Karşı-Uygulama/İkinci Kural → Sonuç adımları tam mı; karşı tarafın olası argümanı öngörülüp çürütüldü mü?
- IRAAC'te karşı-uygulama gerçekten karşı argümanı çürütüyor mu (yalnızca asıl iddianın tekrarı değil)?
- IRRAC'te ikinci kural asıl kuralı destekliyor/alternatif sunuyor mu; HUKUKİ NEDENLER'de yer aldı mı?
- Sonuç, NETİCE VE TALEP'teki taleple tutarlı mı?
- Talep, açıklama ve dayanak birbirini tutuyor mu?
- Süreler gözetildi mi (cevap, dilekçe teatisi, kanun yolu)?
- Kişisel veri taşınmadı; eksik bilgiler `[yer tutucu]` mı?
- TDK yazımı ve doğru kapanış kalıbı (tekil/çoğul) kullanıldı mı?
- Çıktı biçimi (yazı tipi, başlık, imza bloğu) düzgün mü?

## İlkeler

- TDK yazımı; resmî, ölçülü, saygılı üslup.
- Yer tutucu mantığı; gerçek kişisel veri yok (KVKK) — `references/bicim-ve-cikti.md`.
- İçtihat: karar yığını değil, kısa atıf + ilke.
- Karşı argümanı çürütürken meslektaşa saygı; iddiayı çürüt, kişiyi değil.
- Üretilen taslağın hukuki sorumluluğu kullanıcıya (avukata) aittir; son kontrol ve imza ondadır.
