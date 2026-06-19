---
name: dilekce-crac
description: >-
  CRAC (Conclusion → Rule → Application → Conclusion / Sonuç → Kural → Uygulama →
  Sonuç) yöntemiyle Türk hukukunda dilekçe ve savunma hazırlamak için kullanılır.
  Tetikleyiciler: "CRAC yöntemiyle/şemasıyla dilekçe", "CRAC ile dava/cevap/savunma",
  "sonuç-merkezli / Conclusion-Rule-Application-Conclusion dilekçe",
  "kısa-net dilekçe/beyan". Sonucu baştan koyan; kuralın tartışmasız olduğu
  hızlı/doğrudan dilekçelerde, ara ve beyan dilekçelerinde meseleyi kısa ve net
  ortaya koyar. Çıktı docx/html/udf/pdf üretilir.
---

# CRAC ile Dilekçe Oluşturma

CRAC, CREAC'in **sadeleştirilmiş** hâlidir: ayrı bir **Explanation/açıklama**
katmanı yoktur. **Sonucu baştan koyar**, kuralı anar, somut olaya uygular ve sonucu
yineler. Kuralın tartışmasız olduğu, hızlı ve doğrudan ifade gerektiren
dilekçelerde; iddianın daha ilk cümlede net görünmesini sağlar.

## Ne zaman kullanılır

- Uygulanacak kural tartışmasız; uzun bir kural açıklamasına (Explanation) gerek yok.
- Dilekçenin kısa, doğrudan ve sonuç-merkezli olması isteniyor.
- Ara dilekçeler, beyan dilekçeleri, basit talepler ve hızlı yanıtlar.
- Dava, cevap, replik, düplik veya ceza savunması — tür fark etmez.

## CRAC mantığı

1. **C — Sonuç (Conclusion):** Varılması istenen sonucu/iddiayı baştan, tek cümlede net koy.
2. **R — Kural (Rule):** Uygulanacak mevzuat/içtihat/ilke (kısa; ayrı açıklama katmanı yok).
3. **A — Uygulama (Application):** Kuralı somut olaya tatbik et (işin kalbi).
4. **C — Sonuç (Conclusion):** Baştaki sonucu pekiştirerek talebe bağla.

## Çalışma akışı

1. **Dilekçe türünü belirle** (dava/cevap/replik/düplik/savunma) — `references/bicim-ve-cikti.md`.
2. **Bilgileri topla:** mahkeme ve dosya no, taraflar, konu, talepler, vakıalar, deliller.
   Eksikleri `AskUserQuestion` veya kısa sorularla tamamla. Dava dosyası verildiyse oku:
   `.udf` → `udf-cli udf2md`; çok sayfalı `.tiff/.tif` → sayfalara böl, tek tek oku; PDF/foto/metin → doğrudan oku.
3. **CRAC iskeletini kur** — adım tanımları ve eşleme tablosu için `references/cerceve-yapisi.md`.
4. **Gövdeyi yaz:** İddiayı baştan koy; AÇIKLAMALAR'ı `C → R → A → C` akışıyla kur. Gereksiz
   açıklama katmanı ekleme; her hukuki mesele için ayrı, kısa bir CRAC bloğu yeterlidir.
5. **Çıktıyı üret** (docx/html/udf/pdf) — `references/bicim-ve-cikti.md`.
6. **Doğrula ve sun.**

## CRAC adımlarının dilekçe bölümlerine eşlemesi

| CRAC adımı | Dilekçe bölümü | İçerik |
|------------|----------------|--------|
| Sonuç (baştaki) | KONU + AÇIKLAMALAR başı | Baştan konulan iddia/sonuç cümlesi |
| Kural | HUKUKİ NEDENLER (+ gövdede atıf) | Dayanak mevzuat/içtihat/ilke |
| Uygulama | AÇIKLAMALAR (irdeleme) | Kuralın somut olaya tatbiki |
| Sonuç (sondaki) | NETİCE VE TALEP | Baştaki sonucun talebe bağlanması |

## Çıktı formatları

docx (varsayılan) · html (standalone) · udf (UYAP) · pdf. Ayrıntı: `references/bicim-ve-cikti.md`.

## Doğrulama listesi

- Sonuç → Kural → Uygulama → Sonuç adımları tam mı; iddia baştan net konuldu mu, gereksiz açıklama katmanı eklenmedi mi?
- Baştaki sonuç ile sondaki sonuç (NETİCE VE TALEP) birbiriyle tutarlı mı?
- Kural kısa ve doğrudan mı verildi; karar/mevzuat yığını yapılmadı mı?
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
