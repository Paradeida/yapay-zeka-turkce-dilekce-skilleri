---
name: dilekce-mirat
description: >-
  MIRAT (Material facts → Issue → Rule → Application → Tentative conclusion /
  Maddi Vakıalar → Mesele → Kural → Uygulama → Geçici Sonuç) yöntemiyle Türk
  hukukunda dilekçe ve savunma hazırlamak için kullanılır. Tetikleyiciler:
  "MIRAT yöntemiyle/şemasıyla dilekçe", "MIRAT ile dava/cevap/savunma yaz",
  "maddi vakıaları süzerek dilekçe", "geçici sonuçlu / kademeli talep dilekçesi".
  Vakıası bol veya ihtimalli/alternatif talep içeren dosyalarda vakıayı süzüp
  meseleyi netleştirir. Çıktı docx/html/udf/pdf üretilir.
---

# MIRAT ile Dilekçe Oluşturma

MIRAT, IRAC'in başına süzülmüş **maddi vakıaları** ekleyen ve sonucu **geçici
(tentative)** olarak sunan bir analiz/yazım şemasıdır. Vakıa örgüsünün kalabalık
olduğu, ya da talebin ihtimalli/kademeli kurulduğu dosyalarda; ilgili vakıaları
baştan süzüp meseleyi netleştirmek için güçlüdür.

## Ne zaman kullanılır

- Vakıa örgüsü kalabalık; hangi vakıaların hukuken ilgili olduğunu baştan süzmek gerekiyor.
- Talep ihtimalli/alternatif/kademeli (asıl–terditli) kurulacak.
- Sonucun mahkemenin takdirine açık, "geçici" bir nitelendirmeyle sunulması tercih ediliyor.
- Dava, cevap, replik, düplik veya ceza savunması — tür fark etmez.

## MIRAT mantığı

1. **M — Maddi Vakıalar:** Olay örgüsünden yalnızca hukuken ilgili vakıaları süz.
2. **I — Mesele (Issue):** Çözülecek hukuki soruyu net koy.
3. **R — Kural (Rule):** Uygulanacak mevzuat/içtihat/ilke.
4. **A — Uygulama (Application):** Kuralı süzülmüş vakıalara tatbik et (işin kalbi).
5. **T — Geçici Sonuç (Tentative conclusion):** Vardığın sonuç; kesin dayatma değil, takdire açık.

## Çalışma akışı

1. **Dilekçe türünü belirle** (dava/cevap/replik/düplik/savunma) — `references/bicim-ve-cikti.md`.
2. **Bilgileri topla:** mahkeme ve dosya no, taraflar, konu, talepler, vakıalar, deliller.
   Eksikleri `AskUserQuestion` veya kısa sorularla tamamla. Dava dosyası verildiyse oku:
   `.udf` → `udf-cli udf2md`; çok sayfalı `.tiff/.tif` → sayfalara böl, tek tek oku; PDF/foto/metin → doğrudan oku.
3. **MIRAT iskeletini kur** — adım tanımları ve eşleme tablosu için `references/cerceve-yapisi.md`.
4. **Gövdeyi yaz:** AÇIKLAMALAR'ı `M → I → R → A → T` akışıyla başlıklandır. Her hukuki
   mesele için ayrı bir MIRAT bloğu kurabilirsin; maddi vakıaları girişte süz.
5. **Çıktıyı üret** (docx/html/udf/pdf) — `references/bicim-ve-cikti.md`.
6. **Doğrula ve sun.**

## MIRAT adımlarının dilekçe bölümlerine eşlemesi

| MIRAT adımı | Dilekçe bölümü | İçerik |
|-------------|----------------|--------|
| Maddi Vakıalar | AÇIKLAMALAR / GİRİŞ | Süzülmüş, hukuken ilgili olay örgüsü |
| Mesele | Her bölümün başı | Çözülecek hukuki soru (tek cümle) |
| Kural | HUKUKİ NEDENLER (+ gövdede atıf) | Dayanak mevzuat/içtihat/ilke |
| Uygulama | AÇIKLAMALAR (irdeleme) | Kuralın süzülmüş vakıalara tatbiki |
| Geçici Sonuç | Bölüm sonu + NETİCE VE TALEP | Ara sonuç; netice'de pekiştirilir |

## Çıktı formatları

docx (varsayılan) · html (standalone) · udf (UYAP) · pdf. Ayrıntı: `references/bicim-ve-cikti.md`.

## Doğrulama listesi

- M-I-R-A-T adımlarının beşi de var mı; her mesele için süzülmüş vakıa → mesele → kural → uygulama → geçici sonuç akışı kuruldu mu?
- Maddi vakıalar gerçekten süzüldü mü (ilgisiz olaylar gövdeye taşınmadı mı)?
- Geçici sonuç, NETİCE VE TALEP'teki kesin taleple tutarlı mı?
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
