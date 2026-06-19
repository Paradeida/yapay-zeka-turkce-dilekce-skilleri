# Yapay Zeka için Türkçe Dilekçe Skilleri

Türk hukukunda dilekçe ve savunma yazımını, **hukuki argüman çerçevelerine** göre
yapılandıran yapay zeka skill'leri (Claude Code / AI ajanları için). Her skill, bir
argüman/yazım şemasını (IRAC ailesi, CREAC ailesi, Toulmin, klasik retorik) Türk
dilekçe pratiğine eşler; bilgileri toplar, uygun iskeleti kurar ve **docx / html /
udf (UYAP) / pdf** çıktısı üretir.

> Bu skill'ler bir **taslak yardımcısıdır**. Üretilen metnin hukuki sorumluluğu,
> son kontrolü ve imzası kullanıcıya (avukata) aittir.

## Çerçeveler

| Skill | Çerçeve | Şema |
|-------|---------|------|
| `dilekce-mirat` | MIRAT | Maddi Vakıalar → Mesele → Kural → Uygulama → Geçici Sonuç |
| `dilekce-iraac` | IRAAC / IRRAC | Mesele → Kural → Uygulama → Karşı-Uygulama / İkinci Kural → Sonuç |
| `dilekce-ilac` | ILAC | Mesele → Mevzuat (Law) → Uygulama → Sonuç |
| `dilekce-ipac` | IPAC / IDAR | Mesele → İlke / Doktrin → Uygulama → Sonuç |
| `dilekce-treac` | TREAC / TREACC | Tez → Kural → Açıklama → Uygulama → Sonuç (+Karşı argüman) |
| `dilekce-crac` | CRAC | Sonuç → Kural → Uygulama → Sonuç |
| `dilekce-crupac` | CRuPAC | Sonuç → Kural → Kuralın İspatı → Uygulama → Sonuç |
| `dilekce-crexac` | CREXAC | Sonuç → Kural → Açıklama → Emsal Örnek → Uygulama → Sonuç |
| `dilekce-treat` | TREAT | Tez → Kural → Açıklama → Uygulama → Tez (tekrar) |
| `dilekce-crracc` | CRRACC | Sonuç → Kural → Açıklama → Uygulama → Karşı argüman/menfaat → Sonuç |
| `dilekce-toulmin` | Toulmin | İddia → Dayanak → Gerekçe/Köprü → Destek → Çekince → Çürütme |
| `dilekce-klasik-retorik` | Cicero/Quintilian | Exordium → Narratio → Partitio → Confirmatio → Refutatio → Peroratio |

## Hangi çerçeve ne zaman?

- **Sonucu sona koyanlar** (MIRAT, ILAC, IPAC, IRAAC): mesele-temelli, klasik analiz.
- **Sonucu/tezi başa koyanlar** (CRAC, CRuPAC, CREXAC, TREAC, TREAT, CRRACC): savunma/brief; hâkimi baştan yönlendirir.
- **Toulmin**: argümandaki örtük köprüyü (warrant) görünür kılar; karşı tarafın zayıf halkasını hedeflemek ve itiraz dilekçeleri için güçlü.
- **Klasik retorik**: kapsamlı, anlatı gücü yüksek, çok bölümlü dilekçeler.

## Her skill'in içeriği

```
dilekce-<cerceve>/
├── SKILL.md                   # çerçeve mantığı, çalışma akışı, dilekçeye eşleme, doğrulama
└── references/
    ├── cerceve-yapisi.md      # adım adım çerçeve + eşleme tablosu + örnek blok
    └── bicim-ve-cikti.md      # ortak: biçim, hizalama, üslup, KVKK ve docx/html/udf/pdf üretimi
```

### Biçim / hizalama
- Mahkeme başlığı **ortalı**, gövde metni **iki yana yaslı (justify)**, vekil adı ve imza **sağa yaslı**.
- Times New Roman 12, satır aralığı 1,5; bölüm başlıkları kalın ve BÜYÜK harf.

## Kurulum (Claude Code)

Skill klasörlerini bir Claude Code eklentisinin ya da projenin `skills/` dizinine
kopyalayın; Claude Code skill'leri otomatik tanır:

```bash
git clone https://github.com/Paradeida/yapay-zeka-turkce-dilekce-skilleri.git
# skills/ altındaki klasörleri kendi eklenti/proje skills dizininize kopyalayın
```

Kullanırken çerçeve adıyla tetikleyin: örn. *"CREAC ... "*, *"MIRAT yöntemiyle cevap dilekçesi yaz"*, *"Toulmin ile bilirkişi raporuna itiraz"*.

## KVKK ve gizlilik

Bu depodaki **hiçbir dosya gerçek kişisel veri içermez** — referans metinleri ve
örnek bloklar dahil. Tüm taraf/vekil alanları `[KÖŞELİ PARANTEZ]` yer tutucudur.
Skill'ler, üretilen dilekçeye yalnızca kullanıcının verdiği bilgileri yazar; başka
kaynaktan kişisel veri taşımaz.

## Sorumluluk reddi

Bu skill'ler hukuki tavsiye değildir; bir avukatın çalışmasını hızlandıran taslak
araçlarıdır. Üretilen her metnin mevzuat/içtihat güncelliği, doğruluğu ve nihai
sorumluluğu kullanıcıya aittir.

## Lisans

[MIT](LICENSE)
