---
name: dilekce-crupac
description: >-
  CRuPAC (Conclusion → Rule → Rule proof → Application → Conclusion /
  Sonuç → Kural → Kuralın İspatı → Uygulama → Sonuç) yöntemiyle Türk
  hukukunda dilekçe ve savunma hazırlamak için kullanılır. Tetikleyiciler:
  "CRuPAC yöntemiyle/şemasıyla dilekçe", "kuralın içtihatla ispatına dayanan
  dilekçe", "Conclusion-Rule-Ruleproof-Application-Conclusion ile yaz",
  "kural ispatı katmanlı dilekçe". Kuralın varlığı veya kapsamı tartışmalı
  olup yargı içtihadıyla desteklenmesi gereken dosyalarda kuralı ayrı bir
  adımda ispatlar. Çıktı docx/html/udf/pdf üretilir.
---

# CRuPAC ile Dilekçe Oluşturma

CRuPAC, CREAC'in "Explanation" katmanını daha sistematik kılan; kuralın varlığını
ve kapsamını ayrı bir **"Kuralın İspatı (Rule proof)"** adımıyla ortaya koyan bir
analiz/yazım şemasıdır. Uygulanacak kuralın kendisi tartışmalı olduğunda, kuralı
yargı içtihadı ve öğretiyle dayanağa oturtarak meseleyi sağlam bir zemine taşır.

## Ne zaman kullanılır

- Uygulanacak kuralın **varlığı veya kapsamı tartışmalı**; içtihatla desteklenmesi gerekiyor.
- Karşı taraf farklı bir kural yorumu öne sürüyor; kuralın doğru içeriğinin ispatı gerek.
- Sonucun en başta net konması, ardından kuralın gerekçelendirilmesi tercih ediliyor.
- Dava, cevap, replik, düplik veya ceza savunması — tür fark etmez.

## CRuPAC mantığı

1. **C — Sonuç (Conclusion):** Varılan sonucu en başta net koy (tez cümlesi).
2. **R — Kural (Rule):** Uygulanacak mevzuat hükmü/genel kural.
3. **Ru — Kuralın İspatı (Rule proof):** Kuralın varlığını ve kapsamını yargı içtihadı/öğretiyle ispatla (işin ayırt edici adımı).
4. **A — Uygulama (Application):** İspatlanmış kuralı somut vakıalara tatbik et.
5. **C — Sonuç (Conclusion):** Açılıştaki sonucu, ispat ve uygulamanın ışığında pekiştir.

## Çalışma akışı

1. **Dilekçe türünü belirle** (dava/cevap/replik/düplik/savunma) — `references/bicim-ve-cikti.md`.
2. **Bilgileri topla:** mahkeme ve dosya no, taraflar, konu, talepler, vakıalar, deliller.
   Eksikleri `AskUserQuestion` veya kısa sorularla tamamla. Dava dosyası verildiyse oku:
   `.udf` → `udf-cli udf2md`; çok sayfalı `.tiff/.tif` → sayfalara böl, tek tek oku; PDF/foto/metin → doğrudan oku.
3. **CRuPAC iskeletini kur** — adım tanımları ve eşleme tablosu için `references/cerceve-yapisi.md`.
4. **Gövdeyi yaz:** AÇIKLAMALAR'ı `C → R → Ru → A → C` akışıyla başlıklandır. Her hukuki
   mesele için ayrı bir CRuPAC bloğu kurabilirsin; kuralın ispatını kısa atıf + ilke biçiminde ver, karar yığını yapıştırma.
5. **Çıktıyı üret** (docx/html/udf/pdf) — `references/bicim-ve-cikti.md`.
6. **Doğrula ve sun.**

## CRuPAC adımlarının dilekçe bölümlerine eşlemesi

| CRuPAC adımı | Dilekçe bölümü | İçerik |
|--------------|----------------|--------|
| Sonuç (açılış) | AÇIKLAMALAR / bölüm başı | Varılan sonucun net tez cümlesi |
| Kural | HUKUKİ NEDENLER (+ gövdede atıf) | Dayanak mevzuat/genel kural |
| Kuralın İspatı | AÇIKLAMALAR (kural gerekçesi) | "Bu kural Yargıtay'ın yerleşik içtihadıyla da sabittir..." — kısa atıf + ilke |
| Uygulama | AÇIKLAMALAR (irdeleme) | İspatlanmış kuralın somut vakıaya tatbiki |
| Sonuç (kapanış) | Bölüm sonu + NETİCE VE TALEP | Açılış sonucunun pekiştirilmesi |

## Çıktı formatları

docx (varsayılan) · html (standalone) · udf (UYAP) · pdf. Ayrıntı: `references/bicim-ve-cikti.md`.

## Doğrulama listesi

- Sonuç → Kural → Kuralın İspatı → Uygulama → Sonuç adımları tam mı; kural içtihatla (kısa atıfla) ispatlandı mı, karar yığını yapıştırılmadı mı?
- Açılış sonucu ile kapanış sonucu tutarlı mı; ikisi aynı tezi mi savunuyor?
- Kuralın İspatı adımı gerçekten kuralın varlığını/kapsamını mı gerekçelendiriyor (yoksa uygulamaya mı kaymış)?
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
