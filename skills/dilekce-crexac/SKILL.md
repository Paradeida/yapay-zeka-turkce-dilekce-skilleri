---
name: dilekce-crexac
description: >-
  CREXAC (Conclusion → Rule → Explanation → Example → Application → Conclusion /
  Sonuç → Kural → Açıklama → Emsal Örnek → Uygulama → Sonuç) yöntemiyle Türk
  hukukunda dilekçe ve savunma hazırlamak için kullanılır. Tetikleyiciler:
  "CREXAC yöntemiyle/şemasıyla dilekçe", "CREXAC ile dava/cevap/savunma yaz",
  "emsal-örnek odaklı dilekçe", "benzer olayda mahkeme şöyle değerlendirdi
  dilekçesi", "Conclusion-Rule-Explanation-Example-Application-Conclusion".
  Emsal kararın güçlü olduğu, kuralın benzer bir olayda nasıl uygulandığını
  göstermenin tezi taşıdığı dosyalarda kullanılır. Çıktı docx/html/udf/pdf üretilir.
---

# CREXAC ile Dilekçe Oluşturma

CREXAC, CREAC şemasına **emsal örnek (Example)** katmanını ekleyen bir analiz/yazım
şemasıdır: kuralı soyut açıklamakla yetinmez, kuralın **benzer bir olayda** nasıl
uygulandığını gösteren bir emsal karara veya örnek olaya dayanır. Emsal kararın
güçlü olduğu, "benzer olayda mahkeme şöyle değerlendirdi" denilebilen dosyalarda;
tezi emsalle pekiştirip somut olaya tatbik etmek için güçlüdür.

## Ne zaman kullanılır

- Davayı taşıyan güçlü bir emsal karar veya örnek olay var; kuralın benzer olguda nasıl uygulandığı tezi destekliyor.
- "Benzer bir uyuşmazlıkta mahkeme şöyle değerlendirdi" diyerek somut olayla paralellik kurulabiliyor.
- Soyut kural anlatımının tek başına yetmediği, emsalle örneklemenin ikna gücünü artırdığı dosyalar.
- Dava, cevap, replik, düplik veya ceza savunması — tür fark etmez.

## CREXAC mantığı

1. **C — Sonuç (Conclusion):** Vardığın sonucu/talebi baştan net koy.
2. **R — Kural (Rule):** Uygulanacak mevzuat hükmü/içtihat/ilke.
3. **E — Açıklama (Explanation):** Kuralın anlamını ve unsurlarını soyut olarak aç.
4. **X — Emsal Örnek (Example):** Kuralın **benzer bir olayda** nasıl uygulandığını gösteren emsal karar veya örnek olay — kısa atıf + ilke.
5. **A — Uygulama (Application):** Kuralı **ve emsali** somut olaya tatbik et (işin kalbi); olgular arası paralelliği kur.
6. **C — Sonuç (Conclusion):** Açılışla tutarlı kapanış sonucu; NETİCE VE TALEP'te pekiştirilir.

## Çalışma akışı

1. **Dilekçe türünü belirle** (dava/cevap/replik/düplik/savunma) — `references/bicim-ve-cikti.md`.
2. **Bilgileri topla:** mahkeme ve dosya no, taraflar, konu, talepler, vakıalar, deliller.
   Eksikleri `AskUserQuestion` veya kısa sorularla tamamla. Dava dosyası verildiyse oku:
   `.udf` → `udf-cli udf2md`; çok sayfalı `.tiff/.tif` → sayfalara böl, tek tek oku; PDF/foto/metin → doğrudan oku.
3. **Emsali tespit et:** somut olayla paralel, güçlü bir emsal karar/örnek olay belirle; uydurma karar no kullanma.
4. **CREXAC iskeletini kur** — adım tanımları ve eşleme tablosu için `references/cerceve-yapisi.md`.
5. **Çıktıyı üret** (docx/html/udf/pdf) — `references/bicim-ve-cikti.md`.
6. **Doğrula ve sun.**

## CREXAC adımlarının dilekçe bölümlerine eşlemesi

| CREXAC adımı | Dilekçe bölümü | İçerik |
|--------------|----------------|--------|
| Sonuç | AÇIKLAMALAR / GİRİŞ | Baştan konan sonuç/tez (tek cümle) |
| Kural | HUKUKİ NEDENLER (+ gövdede atıf) | Dayanak mevzuat/içtihat/ilke |
| Açıklama | AÇIKLAMALAR (kural izahı) | Kuralın anlamı ve unsurları |
| Emsal Örnek | AÇIKLAMALAR (emsal/benzer olay) | Emsal kararın kısa atfı + ilke |
| Uygulama | AÇIKLAMALAR (irdeleme) | Kuralın + emsalin somut olaya tatbiki |
| Sonuç | Bölüm sonu + NETİCE VE TALEP | Pekiştirilen kesin sonuç/talep |

## Çıktı formatları

docx (varsayılan) · html (standalone) · udf (UYAP) · pdf. Ayrıntı: `references/bicim-ve-cikti.md`.

## Doğrulama listesi

- Sonuç → Kural → Açıklama → Emsal Örnek → Uygulama → Sonuç adımları tam mı; emsal kısa atıfla verildi mi (karar yığını değil), uydurma karar no kullanılmadı mı?
- Emsal ile somut olay arasındaki paralellik açıkça kuruldu mu (olgular örtüşüyor mu)?
- Açılış sonucu ile kapanış sonucu ve NETİCE VE TALEP birbirini tutuyor mu?
- Talep, açıklama ve dayanak birbirini tutuyor mu?
- Süreler gözetildi mi (cevap, dilekçe teatisi, kanun yolu)?
- Kişisel veri taşınmadı; eksik bilgiler `[yer tutucu]` mı?
- TDK yazımı ve doğru kapanış kalıbı (tekil/çoğul) kullanıldı mı?
- Çıktı biçimi (yazı tipi, başlık, imza bloğu) düzgün mü?

## İlkeler

- TDK yazımı; resmî, ölçülü, saygılı üslup.
- Yer tutucu mantığı; gerçek kişisel veri yok (KVKK) — `references/bicim-ve-cikti.md`.
- İçtihat: karar yığını değil, kısa atıf + ilke; uydurma karar no kullanılmaz.
- Üretilen taslağın hukuki sorumluluğu kullanıcıya (avukata) aittir; son kontrol ve imza ondadır.
