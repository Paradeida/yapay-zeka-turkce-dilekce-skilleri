---
name: dilekce-ilac
description: >-
  ILAC (Issue → Law → Application → Conclusion / Mesele → Mevzuat → Uygulama →
  Sonuç) yöntemiyle Türk hukukunda dilekçe ve savunma hazırlamak için kullanılır.
  Tetikleyiciler: "ILAC yöntemiyle/şemasıyla dilekçe", "ILAC ile dava/cevap/savunma yaz",
  "mevzuat-merkezli dilekçe", "Issue-Law-Application-Conclusion dilekçe".
  Çözümü açık kanun hükmüne dayanan, içtihat tartışması az dosyalarda mevzuat
  maddesini öne çıkararak meseleyi netleştirir. Çıktı docx/html/udf/pdf üretilir.
---

# ILAC ile Dilekçe Oluşturma

ILAC, IRAC'in "Rule" basamağını **"Law" (Mevzuat)** olarak konumlandıran,
çözümü büyük ölçüde **açık kanun hükmüne** dayandıran mevzuat-merkezli bir
analiz/yazım şemasıdır (Avustralya/İngiltere ekolü). İçtihat ve öğreti
tartışmasının az, çözümün doğrudan kanun lafzından çıktığı dosyalarda; kanun
maddesini öne çıkararak meseleyi netleştirmek için güçlüdür.

## Ne zaman kullanılır

- Çözüm açık bir kanun hükmüne dayanıyor; içtihat/öğreti tartışması sınırlı.
- Uyuşmazlık süre, şekil şartı veya açık emredici hüküm gibi lafzı belirgin bir hükümle çözülüyor.
- Kanun maddesinin (lafzı/amacı) dilekçenin merkezine yerleştirilmesi tercih ediliyor.
- Dava, cevap, replik, düplik veya ceza savunması — tür fark etmez.

## ILAC mantığı

1. **I — Mesele (Issue):** Çözülecek hukuki soruyu net koy.
2. **L — Mevzuat (Law):** Çözümü doğrudan veren kanun hükmünü (lafzı/amacı) öne çıkar.
3. **A — Uygulama (Application):** Kanun hükmünü somut olaya tatbik et (işin kalbi).
4. **C — Sonuç (Conclusion):** Hükmün uygulanmasından çıkan kesin sonucu kur.

## Çalışma akışı

1. **Dilekçe türünü belirle** (dava/cevap/replik/düplik/savunma) — `references/bicim-ve-cikti.md`.
2. **Bilgileri topla:** mahkeme ve dosya no, taraflar, konu, talepler, vakıalar, deliller.
   Eksikleri `AskUserQuestion` veya kısa sorularla tamamla. Dava dosyası verildiyse oku:
   `.udf` → `udf-cli udf2md`; çok sayfalı `.tiff/.tif` → sayfalara böl, tek tek oku; PDF/foto/metin → doğrudan oku.
3. **ILAC iskeletini kur** — adım tanımları ve eşleme tablosu için `references/cerceve-yapisi.md`.
4. **Gövdeyi yaz:** AÇIKLAMALAR'ı `I → L → A → C` akışıyla başlıklandır. Her hukuki
   mesele için ayrı bir ILAC bloğu kurabilirsin; uygulanan kanun hükmünü açıkça göster.
5. **Çıktıyı üret** (docx/html/udf/pdf) — `references/bicim-ve-cikti.md`.
6. **Doğrula ve sun.**

## ILAC adımlarının dilekçe bölümlerine eşlemesi

| ILAC adımı | Dilekçe bölümü | İçerik |
|------------|----------------|--------|
| Mesele | Her bölümün başı | Çözülecek hukuki soru (tek cümle) |
| Mevzuat | HUKUKİ NEDENLER (ağırlıkla) + gövde atıfı | Çözümü veren kanun hükmü (lafzı/amacı) |
| Uygulama | AÇIKLAMALAR (irdeleme) | Kanun hükmünün somut olaya tatbiki |
| Sonuç | Bölüm sonu + NETİCE VE TALEP | Hükümden çıkan kesin sonuç |

## Çıktı formatları

docx (varsayılan) · html (standalone) · udf (UYAP) · pdf. Ayrıntı: `references/bicim-ve-cikti.md`.

## Doğrulama listesi

- Mesele → Mevzuat → Uygulama → Sonuç adımları tam mı; uygulanan kanun hükmü açıkça gösterildi mi?
- Çözüm gerçekten kanun lafzına/amacına dayandırıldı mı (gereksiz içtihat yığını eklenmedi mi)?
- Sonuç, NETİCE VE TALEP'teki kesin taleple tutarlı mı?
- Talep, açıklama ve dayanak birbirini tutuyor mu?
- Süreler gözetildi mi (cevap, dilekçe teatisi, kanun yolu)?
- Kişisel veri taşınmadı; eksik bilgiler `[yer tutucu]` mı?
- TDK yazımı ve doğru kapanış kalıbı (tekil/çoğul) kullanıldı mı?
- Çıktı biçimi (yazı tipi, başlık, imza bloğu) düzgün mü?

## İlkeler

- TDK yazımı; resmî, ölçülü, saygılı üslup.
- Yer tutucu mantığı; gerçek kişisel veri yok (KVKK) — `references/bicim-ve-cikti.md`.
- Mevzuat-merkezlilik: çözümü açık kanun hükmüne dayandır; içtihat gerekiyorsa karar yığını değil, kısa atıf + ilke.
- Üretilen taslağın hukuki sorumluluğu kullanıcıya (avukata) aittir; son kontrol ve imza ondadır.
