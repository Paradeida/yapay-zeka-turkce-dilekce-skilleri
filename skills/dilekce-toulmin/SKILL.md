---
name: dilekce-toulmin
description: >-
  Toulmin Modeli (Claim → Grounds → Warrant → Backing → Qualifier → Rebuttal /
  İddia → Dayanak → Gerekçe/Köprü → Destek → Çekince → Çürütme) çerçevesiyle Türk
  hukukunda dilekçe ve savunma hazırlamak için kullanılır. Tetikleyiciler:
  "Toulmin modeliyle dilekçe", "Toulmin ile itiraz/bilirkişiye itiraz",
  "iddia-dayanak-gerekçe(warrant) analizi", "karşı tarafın argümanındaki köprüyü
  hedefleyen dilekçe". Vakıayı talebe bağlayan örtük hukuki köprüyü (warrant)
  görünür kılar; karşı tarafın argümanındaki zayıf halkayı hedeflemekte güçlüdür.
  Çıktı docx/html/udf/pdf üretilir.
---

# Toulmin Modeli ile Dilekçe Oluşturma

Toulmin Modeli, katı bir şema değil **esnek bir argüman iskeletidir**. Bir iddianın
(Claim) hangi vakıaya (Grounds) dayandığını ve bu ikisini birbirine bağlayan örtük
hukuki gerekçeyi — **warrant (köprü)** — açık eder. Argümanın "neden geçerli olduğunu"
görünür kıldığı için, karşı tarafın argümanındaki **zayıf veya eksik köprüyü** hedeflemekte
güçlüdür.

## Ne zaman kullanılır

- Karşı tarafın argümanındaki zayıf halkayı (eksik/yanlış warrant) görünür kılmak gerekiyor.
- İtiraz dilekçesi, bilirkişi raporuna itiraz veya red talebi yazılacak.
- Vakıa ile talep arasındaki hukuki köprünün (warrant) ayrıca ve açıkça gösterilmesi isteniyor.
- Dava, cevap, replik, düplik veya ceza savunması — tür fark etmez.

## Toulmin mantığı

1. **Claim — İddia:** Mahkemeden istenen sonuç; ulaşılmak istenen talep/nitelendirme.
2. **Grounds — Dayanak:** İddiayı taşıyan maddi vakıa ve deliller.
3. **Warrant — Gerekçe/Köprü:** Vakıayı (Grounds) iddiaya (Claim) bağlayan örtük hukuki gerekçe; işin kalbi.
4. **Backing — Destek:** Warrant'ın kendisini ayakta tutan dayanak (mevzuat/içtihat/ilke).
5. **Qualifier — Çekince:** İddianın kesinlik derecesi ("kural olarak", "büyük olasılıkla").
6. **Rebuttal — Çürütme:** Karşı tarafın warrant'ını/argümanını hedefleyen karşı değerlendirme.

## Çalışma akışı

1. **Dilekçe türünü belirle** (dava/cevap/replik/düplik/savunma) — `references/bicim-ve-cikti.md`.
2. **Bilgileri topla:** mahkeme ve dosya no, taraflar, konu, talepler, vakıalar, deliller.
   Eksikleri `AskUserQuestion` veya kısa sorularla tamamla. Dava dosyası verildiyse oku:
   `.udf` → `udf-cli udf2md`; çok sayfalı `.tiff/.tif` → sayfalara böl, tek tek oku; PDF/foto/metin → doğrudan oku.
3. **Toulmin iskeletini kur** — her iddia için Claim–Grounds–Warrant–Backing–Qualifier–Rebuttal
   unsurlarını çıkar; adım tanımları ve eşleme tablosu için `references/cerceve-yapisi.md`.
4. **Gövdeyi yaz:** AÇIKLAMALAR'ı `Claim → Grounds → Warrant → Backing → Qualifier → Rebuttal`
   akışıyla kur. **Warrant'ı (vakıayı talebe bağlayan köprü) ayrıca ve açıkça göster;** karşı
   tarafın argümanını çürütürken doğrudan onun warrant'ını hedefle.
5. **Çıktıyı üret** (docx/html/udf/pdf) — `references/bicim-ve-cikti.md`.
6. **Doğrula ve sun.**

## Toulmin adımlarının dilekçe bölümlerine eşlemesi

| Toulmin adımı | Dilekçe bölümü | İçerik |
|---------------|----------------|--------|
| Claim (İddia) | KONU / NETİCE VE TALEP | Mahkemeden istenen sonuç/talep |
| Grounds (Dayanak) | AÇIKLAMALAR | Maddi vakıa + deliller |
| Warrant (Gerekçe/Köprü) | AÇIKLAMALAR (irdeleme) | Vakıayı talebe bağlayan hukuki gerekçe |
| Backing (Destek) | HUKUKİ NEDENLER | Warrant'ın dayanağı: mevzuat/içtihat |
| Qualifier (Çekince) | İlgili bölümde ifade | "kural olarak / büyük olasılıkla" çekincesi |
| Rebuttal (Çürütme) | AÇIKLAMALAR (karşı argüman) | Karşı tarafın warrant'ını/argümanını çürütme |

## Çıktı formatları

docx (varsayılan) · html (standalone) · udf (UYAP) · pdf. Ayrıntı: `references/bicim-ve-cikti.md`.

## Doğrulama listesi

- Claim/Grounds/Warrant/Backing/Qualifier/Rebuttal unsurları ele alındı mı; özellikle warrant (vakıayı talebe bağlayan köprü) açıkça gösterildi mi?
- Grounds (vakıa + delil) ile Claim (talep) arasındaki bağ warrant üzerinden kurulabiliyor mu?
- Backing, warrant'ı gerçekten destekliyor mu (mevzuat/içtihat atıfı yerinde mi)?
- Rebuttal, karşı tarafın argümanındaki doğru zayıf halkayı (warrant'ı) hedefliyor mu?
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
