---
name: dilekce-treac
description: >-
  TREAC (Thesis → Rule → Explanation → Application → Conclusion / Tez → Kural →
  Açıklama → Uygulama → Sonuç) ve TREACC (... → Counterargument → Conclusion /
  karşı argüman katmanı eklenmiş) yöntemiyle Türk hukukunda dilekçe ve savunma
  hazırlamak için kullanılır. Tetikleyiciler: "TREAC yöntemiyle/şemasıyla
  dilekçe", "TREACC ile savunma yaz", "tez-merkezli dilekçe", "Thesis-Rule-
  Explanation-Application-Conclusion dilekçe", "kuralın yorumunu öne çıkaran
  brief". Net bir tez kurulabilen ve kuralın içtihat/öğretiyle yorumunun önem
  taşıdığı savunma ve briefler için güçlüdür. Çıktı docx/html/udf/pdf üretilir.
---

# TREAC / TREACC ile Dilekçe Oluşturma

TREAC, CREAC'e çok yakın bir analiz/yazım şemasıdır; sonucu baştan **tez (thesis)**
olarak koyar ve kuralın içtihat/öğretiyle yorumunu **ayrı bir Açıklama katmanı**
hâline getirir. Net bir tezin kurulabildiği, kuralın ne anlama geldiğinin (yorumun)
sonucu belirlediği savunma ve briefler için güçlüdür. **TREACC**, uygulamadan önce
karşı argümanın çürütüldüğü bir **Counterargument** katmanı ekler.

## Ne zaman kullanılır

- Net bir tez kurulabiliyor; vardığın sonucu baştan açıkça koymak istiyorsun.
- Uyuşmazlığın kalbi kuralın **yorumunda**; kuralı içtihat/öğretiyle açmak belirleyici.
- Karşı tarafın bir argümanı baştan çürütülecekse (TREACC).
- Savunma dilekçesi, replik/düplik veya hukuki brief tarzı metinlerde.
- Dava, cevap, replik, düplik veya ceza savunması — tür fark etmez.

## TREAC / TREACC mantığı

1. **T — Tez (Thesis):** Vardığın sonucu baştan, net bir cümleyle koy.
2. **R — Kural (Rule):** Uygulanacak mevzuat/içtihat/ilke.
3. **E — Açıklama (Explanation):** Kuralın içtihat/öğretiyle yorumu; ne anlama geldiği (ayrı katman).
4. **A — Uygulama (Application):** Yorumlanmış kuralı somut vakıaya tatbik et (işin kalbi).
5. **C — Sonuç (Conclusion):** Tezi pekiştiren kapanış.

TREACC'te, **A**'dan önce bir adım eklenir:

- **C — Karşı argüman (Counterargument):** Karşı tarafın olası tezini ortaya koyup çürüt; ardından **Sonuç**.

## Çalışma akışı

1. **Dilekçe türünü belirle** (dava/cevap/replik/düplik/savunma) — `references/bicim-ve-cikti.md`.
2. **Bilgileri topla:** mahkeme ve dosya no, taraflar, konu, talepler, vakıalar, deliller.
   Eksikleri `AskUserQuestion` veya kısa sorularla tamamla. Dava dosyası verildiyse oku:
   `.udf` → `udf-cli udf2md`; çok sayfalı `.tiff/.tif` → sayfalara böl, tek tek oku; PDF/foto/metin → doğrudan oku.
3. **TREAC/TREACC iskeletini kur** — adım tanımları ve eşleme tablosu için `references/cerceve-yapisi.md`.
   Karşı argüman çürütmesi gerekiyorsa TREACC'i, gerekmiyorsa TREAC'i seç.
4. **Gövdeyi yaz:** AÇIKLAMALAR'ı `T → R → E → A → C` (TREACC'te `T → R → E → (Karşı argüman) → A → C`)
   akışıyla başlıklandır. Tezi girişte net koy; her hukuki mesele için ayrı bir TREAC bloğu kurabilirsin.
5. **Çıktıyı üret** (docx/html/udf/pdf) — `references/bicim-ve-cikti.md`.
6. **Doğrula ve sun.**

## TREAC/TREACC adımlarının dilekçe bölümlerine eşlemesi

| TREAC/TREACC adımı | Dilekçe bölümü | İçerik |
|--------------------|----------------|--------|
| Tez | KONU + AÇIKLAMALAR girişi | Baştan konulan tez cümlesi |
| Kural | HUKUKİ NEDENLER (+ gövdede atıf) | Dayanak mevzuat/içtihat/ilke |
| Açıklama | AÇIKLAMALAR (kuralın açılımı) | Kuralın içtihat/öğretiyle yorumu |
| Karşı argüman (TREACC) | AÇIKLAMALAR (çürütme alt başlığı) | Karşı tezin ortaya konup çürütülmesi |
| Uygulama | AÇIKLAMALAR (irdeleme) | Yorumlanmış kuralın vakıaya tatbiki |
| Sonuç | Bölüm sonu + NETİCE VE TALEP | Tezi pekiştiren kapanış → kesin talep |

## Çıktı formatları

docx (varsayılan) · html (standalone) · udf (UYAP) · pdf. Ayrıntı: `references/bicim-ve-cikti.md`.

## Doğrulama listesi

- Tez → Kural → Açıklama → Uygulama → (Karşı argüman) → Sonuç adımları tam mı; tez baştan net konuldu mu?
- Açıklama, kuralı gerçekten yorumladı mı (içtihat/öğreti ile açıldı mı), yoksa kuralın tekrarı mı?
- TREACC kullanıldıysa karşı argüman önce dürüstçe ortaya konup sonra çürütüldü mü?
- Sonuç ile baştaki tez tutarlı mı; NETİCE VE TALEP'teki kesin talebe bağlanıyor mu?
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
