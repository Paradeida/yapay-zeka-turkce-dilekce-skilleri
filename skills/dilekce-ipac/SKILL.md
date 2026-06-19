---
name: dilekce-ipac
description: >-
  IPAC / IDAR (Issue → Principle/Doctrine → Application → Conclusion/Result /
  Mesele → İlke/Doktrin → Uygulama → Sonuç) yöntemiyle Türk hukukunda dilekçe ve
  savunma hazırlamak için kullanılır. Somut kural yerine genel hukuk ilkesini
  veya öğreti doktrinini merkeze alır. Tetikleyiciler: "IPAC yöntemiyle dilekçe",
  "IDAR ile dilekçe", "ilke/doktrin-merkezli dilekçe", "dürüstlük kuralına /
  genel hukuk ilkesine dayanan dilekçe". Somut kanun maddesinin yetersiz veya
  bulunmadığı, argümanın genel ilke ve öğretiye dayandığı dosyalarda güçlüdür.
  Çıktı docx/html/udf/pdf üretilir.
---

# IPAC / IDAR ile Dilekçe Oluşturma

IPAC ve IDAR, IRAC'in "Kural (Rule)" basamağını genel hukuk **İlkesi (Principle)**
veya öğreti **Doktrini (Doctrine)** ile değiştiren analiz/yazım şemalarıdır. Somut
kanun maddesinin yetersiz kaldığı ya da bulunmadığı; argümanın dürüstlük kuralı,
hakkın kötüye kullanılması yasağı, ahde vefa, sebepsiz zenginleşme veya iyiniyet
gibi genel ilke ve öğretilere dayandığı dosyalarda güçlüdür.

## Ne zaman kullanılır

- Somut kanun maddesi yetersiz veya yok; argüman genel hukuk ilkesine/öğretiye dayanacak.
- Dürüstlük kuralı (TMK m. 2), hakkın kötüye kullanılması, ahde vefa, sebepsiz zenginleşme, iyiniyet gibi bir ilke merkeze alınacak.
- Somut maddeden çok, ilkenin/doktrinin gerekçesi ve değer yargısı öne çıkarılacak.
- Dava, cevap, replik, düplik veya ceza savunması — tür fark etmez.

## IPAC / IDAR mantığı

1. **I — Mesele (Issue):** Çözülecek hukuki soruyu net koy.
2. **P/D — İlke/Doktrin (Principle/Doctrine):** Dayanılacak genel hukuk ilkesi veya öğreti doktrini; somut maddeden çok ilkenin gerekçesi.
3. **A — Uygulama (Application):** İlkeyi/doktrini somut olaya tatbik et (işin kalbi).
4. **C/R — Sonuç (Conclusion/Result):** İlkeden hareketle vardığın sonuç ve talep.

## Çalışma akışı

1. **Dilekçe türünü belirle** (dava/cevap/replik/düplik/savunma) — `references/bicim-ve-cikti.md`.
2. **Bilgileri topla:** mahkeme ve dosya no, taraflar, konu, talepler, vakıalar, deliller.
   Eksikleri `AskUserQuestion` veya kısa sorularla tamamla. Dava dosyası verildiyse oku:
   `.udf` → `udf-cli udf2md`; çok sayfalı `.tiff/.tif` → sayfalara böl, tek tek oku; PDF/foto/metin → doğrudan oku.
3. **IPAC/IDAR iskeletini kur** — adım tanımları, ilke/doktrin vurgusu ve eşleme tablosu için `references/cerceve-yapisi.md`.
4. **Gövdeyi yaz:** AÇIKLAMALAR'ı `I → P/D → A → C/R` akışıyla başlıklandır. Her hukuki
   mesele için ayrı bir IPAC/IDAR bloğu kurabilirsin; dayanılan ilke/doktrini açıkça göster.
5. **Çıktıyı üret** (docx/html/udf/pdf) — `references/bicim-ve-cikti.md`.
6. **Doğrula ve sun.**

## IPAC / IDAR adımlarının dilekçe bölümlerine eşlemesi

| IPAC/IDAR adımı | Dilekçe bölümü | İçerik |
|-----------------|----------------|--------|
| Mesele | Her bölümün başı | Çözülecek hukuki soru (tek cümle) |
| İlke/Doktrin | HUKUKİ NEDENLER + AÇIKLAMALAR'da ilke vurgusu | Dayanılan genel ilke/öğreti; somut maddeden çok ilkenin gerekçesi |
| Uygulama | AÇIKLAMALAR (irdeleme) | İlkenin/doktrinin somut olaya tatbiki |
| Sonuç | Bölüm sonu + NETİCE VE TALEP | İlkeden çıkan sonuç → kesin talep |

## Çıktı formatları

docx (varsayılan) · html (standalone) · udf (UYAP) · pdf. Ayrıntı: `references/bicim-ve-cikti.md`.

## Doğrulama listesi

- Mesele → İlke/Doktrin → Uygulama → Sonuç adımları tam mı; dayanılan ilke/öğreti net gösterildi mi?
- İlke/doktrin somut maddeyle değil, gerekçesiyle (değer yargısıyla) temellendirildi mi?
- Uygulama basamağında ilke–olay bağı açıkça kuruldu mu?
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
