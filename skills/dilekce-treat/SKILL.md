---
name: dilekce-treat
description: >-
  TREAT (Thesis → Rule → Explanation → Application → Thesis restated /
  Tez → Kural → Açıklama → Uygulama → Tezin Tekrarı) yöntemiyle Türk
  hukukunda dilekçe ve savunma hazırlamak için kullanılır. Tetikleyiciler:
  "TREAT yöntemiyle/şemasıyla dilekçe", "TREAT ile dava/cevap/savunma yaz",
  "tez-açıklama-uygulama-tez modeli", "Neumann modeli dilekçe/savunma".
  Tek güçlü tez etrafında kurgulanan; tezi okuyucunun zihnine yerleştirip
  sonda pekiştirerek "çerçeveleyen" dosyalarda güçlüdür. Çıktı docx/html/udf/pdf üretilir.
---

# TREAT ile Dilekçe Oluşturma

TREAT, IRAC'in geliştirilmiş bir biçimidir: **tezle açılır**, kuralı içtihat/öğretiyle
**açıklar (Explanation)** ve aynı tezi sonda **yeniden ifade ederek (restated)** kapatır.
Richard Neumann'ın savunduğu, brief/savunma yazımında popüler bu model; tek güçlü tez
etrafında kurgulanan dosyalarda tezi okuyucunun zihnine yerleştirip pekiştirerek güçlü
bir **çerçeveleme** etkisi yaratır.

## Ne zaman kullanılır

- Savunma/brief tek bir güçlü tez etrafında kurgulanacak; bu tez vurgulanarak öne çıkarılacak.
- Kuralın yalnızca anılması yetmiyor; içtihat ve öğreti ile **açıklanması (Explanation)** gerekiyor.
- Tezin okuyucunun zihnine baştan yerleştirilip sonda **pekiştirilerek tekrarlanması** isteniyor (çerçeveleme).
- Dava, cevap, replik, düplik veya ceza savunması — tür fark etmez.

## TREAT mantığı

1. **T — Tez (Thesis):** Savunduğun ana iddiayı baştan, tek ve net cümleyle koy.
2. **R — Kural (Rule):** Uygulanacak mevzuat/içtihat/ilke.
3. **E — Açıklama (Explanation):** Kuralı içtihat ve öğreti ile yorumla; nasıl uygulandığını aç.
4. **A — Uygulama (Application):** Açıklanan kuralı somut vakıalara tatbik et (işin kalbi).
5. **T — Tezin Tekrarı (Thesis restated):** Baştaki tezi pekiştirerek yeniden ifade et; çerçeveyi kapat.

## Çalışma akışı

1. **Dilekçe türünü belirle** (dava/cevap/replik/düplik/savunma) — `references/bicim-ve-cikti.md`.
2. **Bilgileri topla:** mahkeme ve dosya no, taraflar, konu, talepler, vakıalar, deliller.
   Eksikleri `AskUserQuestion` veya kısa sorularla tamamla. Dava dosyası verildiyse oku:
   `.udf` → `udf-cli udf2md`; çok sayfalı `.tiff/.tif` → sayfalara böl, tek tek oku; PDF/foto/metin → doğrudan oku.
3. **TREAT iskeletini kur** — adım tanımları ve eşleme tablosu için `references/cerceve-yapisi.md`.
4. **Gövdeyi yaz:** AÇIKLAMALAR'ı `T → R → E → A → T` akışıyla başlıklandır. Tez cümlesini
   bölümün başına koy; sonunda aynı tezi pekiştirerek tekrarla. Her hukuki mesele için ayrı
   bir TREAT bloğu kurabilirsin.
5. **Çıktıyı üret** (docx/html/udf/pdf) — `references/bicim-ve-cikti.md`.
6. **Doğrula ve sun.**

## TREAT adımlarının dilekçe bölümlerine eşlemesi

| TREAT adımı | Dilekçe bölümü | İçerik |
|-------------|----------------|--------|
| Tez | AÇIKLAMALAR başındaki tez cümlesi | KONU ile uyumlu ana iddia (tek cümle) |
| Kural | HUKUKİ NEDENLER (+ gövdede atıf) | Dayanak mevzuat/içtihat/ilke |
| Açıklama | AÇIKLAMALAR (kuralın açılımı) | Kuralın içtihat/öğreti ile yorumu |
| Uygulama | AÇIKLAMALAR (irdeleme) | Kuralın somut vakıalara tatbiki |
| Tezin Tekrarı | NETİCE VE TALEP | Tezin pekiştirilerek tekrarı |

## Çıktı formatları

docx (varsayılan) · html (standalone) · udf (UYAP) · pdf. Ayrıntı: `references/bicim-ve-cikti.md`.

## Doğrulama listesi

- Tez → Kural → Açıklama → Uygulama → Tez(tekrar) adımları tam mı; baştaki tez ile sondaki tez tutarlı mı?
- Açıklama (Explanation) gerçekten kuralı içtihat/öğreti ile yorumluyor mu, yoksa kuralı tekrar mı ediyor?
- Sondaki tez, NETİCE VE TALEP'teki kesin taleple tutarlı mı?
- Talep, açıklama ve dayanak birbirini tutuyor mu?
- Süreler gözetildi mi (cevap, dilekçe teatisi, kanun yolu)?
- Kişisel veri taşınmadı; eksik bilgiler `[yer tutucu]` mı?
- TDK yazımı ve doğru kapanış kalıbı (tekil/çoğul) kullanıldı mı?
- Çıktı biçimi (yazı tipi, başlık, imza bloğu) düzgün mü?

## İlkeler

- TDK yazımı; resmî, ölçülü, saygılı üslup.
- Yer tutucu mantığı; gerçek kişisel veri yok (KVKK) — `references/bicim-ve-cikti.md`.
- İçtihat: karar yığını değil, kısa atıf + ilke.
- Üretilen taslağın hukuki sorumluluğu kullanıcıya (avukata) aittir; son kontrol ve imza ondadır.
