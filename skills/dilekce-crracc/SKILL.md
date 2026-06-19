---
name: dilekce-crracc
description: >-
  CRRACC (Conclusion → Rule → Rule explanation → Application → Counterargument →
  Conclusion / Sonuç → Kural → Kuralın Açıklaması → Uygulama → Karşı argüman →
  Sonuç) yöntemiyle Türk hukukunda dilekçe ve savunma hazırlamak için kullanılır.
  Tetikleyiciler: "CRRACC yöntemiyle/şemasıyla dilekçe", "menfaat/policy
  argümanlı çok katmanlı dilekçe", "karşı argüman + hakkaniyet dengesi içeren
  dilekçe", "Conclusion-Rule-Ruleexplanation-Application-Counterargument-Conclusion
  ile dava/cevap/savunma yaz". Karmaşık, çok yönlü ve menfaat dengesi/hakkaniyet
  gerektiren meselelerde kuralı içtihatla açıklar, karşı argümanı çürütür ve
  policy boyutunu işler. Çıktı docx/html/udf/pdf üretilir.
---

# CRRACC ile Dilekçe Oluşturma

CRRACC, CREAC'in en katmanlı türevidir: kuralı ayrı bir adımda **içtihat/öğretiyle
açıklar** ve "Counterargument" adımında yalnızca karşı tarafın iddiasını çürütmekle
kalmayıp **menfaat/hakkaniyet/kamu yararı (policy)** argümanını da işler. İki sonuç
katmanı vardır: başta tezi ortaya koyan **Sonuç**, sonda onu pekiştiren **Sonuç**.
Karmaşık, çok yönlü ve menfaat dengesi gerektiren dosyalarda güçlüdür.

## Ne zaman kullanılır

- Mesele karmaşık ve çok yönlü; tek katmanlı şema (IRAC/CREAC) yetersiz kalıyor.
- Karşı tarafın güçlü bir iddiası var; bunu açıkça karşılayıp çürütmek gerekiyor.
- Menfaat dengesi / hakkaniyet / kamu yararı (policy) argümanı belirleyici.
- Kuralın anlamı içtihat veya öğretiyle ayrıca açıklanmayı gerektiriyor.
- Dava, cevap, replik, düplik veya ceza savunması — tür fark etmez.

## CRRACC mantığı

1. **C — Sonuç (Conclusion):** Varılacak sonucu/tezi baştan, tek cümleyle ortaya koy.
2. **R — Kural (Rule):** Uygulanacak mevzuat hükmü/içtihat/ilke.
3. **R — Kuralın Açıklaması (Rule explanation):** Kuralı içtihat ve öğretiyle yorumla; anlamını ve kapsamını netleştir.
4. **A — Uygulama (Application):** Açıklanan kuralı somut vakıalara tatbik et (işin kalbi).
5. **C — Karşı argüman (Counterargument):** Karşı tarafın iddiasını karşıla ve çürüt; menfaat/hakkaniyet/kamu yararı dengesini ortaya koy.
6. **C — Sonuç (Conclusion):** Baştaki tezi, karşı argüman ve menfaat dengesiyle pekiştirilmiş olarak yinele.

## Çalışma akışı

1. **Dilekçe türünü belirle** (dava/cevap/replik/düplik/savunma) — `references/bicim-ve-cikti.md`.
2. **Bilgileri topla:** mahkeme ve dosya no, taraflar, konu, talepler, vakıalar, deliller.
   Eksikleri `AskUserQuestion` veya kısa sorularla tamamla. Dava dosyası verildiyse oku:
   `.udf` → `udf-cli udf2md`; çok sayfalı `.tiff/.tif` → sayfalara böl, tek tek oku; PDF/foto/metin → doğrudan oku.
3. **CRRACC iskeletini kur** — adım tanımları ve eşleme tablosu için `references/cerceve-yapisi.md`.
4. **Gövdeyi yaz:** AÇIKLAMALAR'ı `C → R → R → A → C → C` akışıyla başlıklandır. Her hukuki
   mesele için ayrı bir CRRACC bloğu kurabilirsin; karşı argüman adımında menfaat/hakkaniyet
   dengesini mutlaka işle.
5. **Çıktıyı üret** (docx/html/udf/pdf) — `references/bicim-ve-cikti.md`.
6. **Doğrula ve sun.**

## CRRACC adımlarının dilekçe bölümlerine eşlemesi

| CRRACC adımı | Dilekçe bölümü | İçerik |
|--------------|----------------|--------|
| Sonuç (baş) | KONU / iddia | Varılacak tez, tek cümleyle |
| Kural | HUKUKİ NEDENLER (+ gövdede atıf) | Dayanak mevzuat/içtihat/ilke |
| Kuralın Açıklaması | AÇIKLAMALAR (yorum) | Kuralın içtihat/öğretiyle yorumu |
| Uygulama | AÇIKLAMALAR (irdeleme) | Açıklanan kuralın vakıalara tatbiki |
| Karşı argüman | AÇIKLAMALAR ("karşı tarafın iddiasının aksine...") | İddianın çürütülmesi + menfaat/hakkaniyet dengesi |
| Sonuç (son) | NETİCE VE TALEP | Pekiştirilmiş kesin talep |

## Çıktı formatları

docx (varsayılan) · html (standalone) · udf (UYAP) · pdf. Ayrıntı: `references/bicim-ve-cikti.md`.

## Doğrulama listesi

- Sonuç → Kural → Açıklama → Uygulama → Karşı argüman(+menfaat) → Sonuç adımları tam mı; karşı argüman ve menfaat dengesi ele alındı mı?
- Kuralın açıklaması içtihat/öğretiyle yapıldı mı; sadece hüküm anılıp geçilmedi mi?
- Baştaki Sonuç ile sondaki Sonuç tutarlı mı; iki katman birbirini pekiştiriyor mu?
- Karşı tarafın iddiası açıkça karşılanıp çürütüldü mü (varsayımsal değil, somut)?
- Talep, açıklama ve dayanak birbirini tutuyor mu?
- Süreler gözetildi mi (cevap, dilekçe teatisi, kanun yolu)?
- Kişisel veri taşınmadı; eksik bilgiler `[yer tutucu]` mı?
- TDK yazımı ve doğru kapanış kalıbı (tekil/çoğul) kullanıldı mı?
- Çıktı biçimi (yazı tipi, başlık, imza bloğu) düzgün mü?

## İlkeler

- TDK yazımı; resmî, ölçülü, saygılı üslup.
- Yer tutucu mantığı; gerçek kişisel veri yok (KVKK) — `references/bicim-ve-cikti.md`.
- İçtihat: karar yığını değil, kısa atıf + ilke.
- Karşı argüman çürütücü olmalı, ama menfaat dengesi tarafsız ve hakkaniyetli kurulmalı.
- Üretilen taslağın hukuki sorumluluğu kullanıcıya (avukata) aittir; son kontrol ve imza ondadır.
