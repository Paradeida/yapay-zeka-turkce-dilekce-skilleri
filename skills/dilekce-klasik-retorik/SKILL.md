---
name: dilekce-klasik-retorik
description: >-
  Klasik Retorik Düzeni (Cicero/Quintilian) — Exordium → Narratio → Partitio →
  Confirmatio → Refutatio → Peroratio (Giriş → Olay Anlatımı → Konu Bölümleme →
  İspat → Çürütme → Sonuç) yöntemiyle Türk hukukunda dilekçe ve savunma
  hazırlamak için kullanılır. Tetikleyiciler: "klasik retorik düzeniyle dilekçe",
  "Cicero/Quintilian düzeni", "Exordium-Narratio-Partitio-Confirmatio-Refutatio-Peroratio",
  "anlatı gücü yüksek kapsamlı dilekçe". Olay örgüsü zengin, çok bölümlü ve hem
  ispat hem çürütme gerektiren dosyalarda anlatıyı güçlü bir iskelete oturtur.
  Çıktı docx/html/udf/pdf üretilir.
---

# Klasik Retorik Düzeniyle Dilekçe Oluşturma

Klasik Retorik Düzeni (Cicero/Quintilian), modern dava dilekçesinin **atasıdır**:
bugünkü "Açıklamalar → karşı tarafın çürütülmesi → sonuç" akışı doğrudan buradan
gelir. Olay anlatımının güçlü, uyuşmazlığın çok başlıklı ve hem kendi iddianı
ispatlamayı hem karşı tarafı çürütmeyi gerektirdiği dosyalarda; anlatıyı düzenli
ve ikna edici bir iskelete oturtmak için elverişlidir.

## Ne zaman kullanılır

- Olay örgüsü zengin; akıcı ve ikna edici bir **anlatı** kurmak gerekiyor.
- Uyuşmazlık çok başlıklı; iddialar ayrı bölümlere ayrılarak işlenecek.
- Hem kendi iddianı ispatlamak (Confirmatio) hem de karşı tarafı çürütmek (Refutatio) ayrı ayrı ele alınacak.
- Kapsamlı, uzun ve çok bölümlü dava/savunma dilekçeleri — tür fark etmez.

## Klasik retorik mantığı

1. **Exordium — Giriş:** Dikkat çeken, ölçülü bir açılış; meseleyi ve duruşunu kısaca tanıt.
2. **Narratio — Olay Anlatımı:** Uyuşmazlığa esas olayı akıcı, kronolojik ve ikna edici biçimde anlat.
3. **Partitio — Konu Bölümleme:** Uyuşmazlığı başlıklara ayır; ele alınacak iddiaları sıraya koy.
4. **Confirmatio — İspat:** Kendi iddianı delil ve hukuki dayanakla ispatla (işin kalbi).
5. **Refutatio — Çürütme:** Karşı tarafın iddialarını tek tek ele alıp çürüt.
6. **Peroratio — Sonuç:** Vurgulu kapanış; özet ve net talep.

## Çalışma akışı

1. **Dilekçe türünü belirle** (dava/cevap/replik/düplik/savunma) — `references/bicim-ve-cikti.md`.
2. **Bilgileri topla:** mahkeme ve dosya no, taraflar, konu, talepler, vakıalar, deliller.
   Eksikleri `AskUserQuestion` veya kısa sorularla tamamla. Dava dosyası verildiyse oku:
   `.udf` → `udf-cli udf2md`; çok sayfalı `.tiff/.tif` → sayfalara böl, tek tek oku; PDF/foto/metin → doğrudan oku.
3. **Klasik retorik iskeletini kur** — adım tanımları ve eşleme tablosu için `references/cerceve-yapisi.md`.
4. **Gövdeyi yaz:** Akışı `Exordium → Narratio → Partitio → Confirmatio → Refutatio → Peroratio`
   sırasıyla kur. Narratio'da olayı akıcı anlat; Partitio ile uyuşmazlığı bölümlere ayır;
   Confirmatio'da ispatla, Refutatio'da karşı tarafı çürüt; Peroratio'da vurguyla kapat.
5. **Çıktıyı üret** (docx/html/udf/pdf) — `references/bicim-ve-cikti.md`.
6. **Doğrula ve sun.**

## Klasik retorik adımlarının dilekçe bölümlerine eşlemesi

| Klasik retorik adımı | Dilekçe bölümü | İçerik |
|----------------------|----------------|--------|
| Exordium | GİRİŞ / KONU | Dikkat çeken, ölçülü açılış; meselenin tanıtımı |
| Narratio | AÇIKLAMALAR (olay anlatımı) | Akıcı, kronolojik, ikna edici olay örgüsü |
| Partitio | Konu bölümleme (I. BÖLÜM / II. BÖLÜM …) | Uyuşmazlığın başlıklara ayrılması, iddia sırası |
| Confirmatio | AÇIKLAMALAR (ispat) + HUKUKİ NEDENLER | Kendi iddianın delil ve hukukla ispatı |
| Refutatio | AÇIKLAMALAR (çürütme) | Karşı tarafın iddialarının tek tek çürütülmesi |
| Peroratio | NETİCE VE TALEP | Vurgulu özet ve kapanış + net talep |

## Çıktı formatları

docx (varsayılan) · html (standalone) · udf (UYAP) · pdf. Ayrıntı: `references/bicim-ve-cikti.md`.

## Doğrulama listesi

- Exordium/Narratio/Partitio/Confirmatio/Refutatio/Peroratio adımları sırasıyla var mı; olay anlatımı ile ispat ve çürütme ayrı ele alındı mı?
- Narratio akıcı ve kronolojik mi; ilgisiz ayrıntı anlatıyı boğmuyor mu?
- Partitio'da kurulan başlıklar Confirmatio ve Refutatio'da gerçekten karşılanıyor mu?
- Karşı tarafın iddiaları Refutatio'da tek tek ve eksiksiz çürütüldü mü?
- Peroratio, NETİCE VE TALEP'teki net taleple tutarlı mı?
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
