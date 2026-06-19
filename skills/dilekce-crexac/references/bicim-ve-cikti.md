# Ortak Biçim, Üslup, KVKK ve Çıktı Formatları

Bu dosya, dilekçe çerçevesi ne olursa olsun geçerli olan ortak kuralları içerir:
dilekçe türü seçimi, taraf bloğu biçimi, kalıp ifadeler, üslup, KVKK ve dört çıktı
formatı (docx / html / udf / pdf). Çerçeveye özgü iskelet için `cerceve-yapisi.md`.

## 1. Önce dilekçe türünü belirle

Çerçeve, dilekçenin türünden bağımsızdır; aynı çerçeve dava, cevap, replik, düplik
veya ceza savunmasında uygulanabilir. Ayırt edici soru:

> "Süreci ben mi başlatıyorum, yoksa karşı tarafın beyanına mı yanıt veriyorum?"

| Durum | Tür | Not |
|------|-----|-----|
| Yeni dava/talep açılıyor | **Dava dilekçesi** | Dosya no yok; harca esas değer + ekler |
| Aleyhine dava açıldı | **Cevap dilekçesi** | İlk itirazlar burada (yetki, görev, derdestlik, zamanaşımı def'i) |
| Davacı, cevaba yanıt veriyor | **Cevaba cevap (replik)** | İddiayı genişletme yasağı |
| Davalı, replike yanıt veriyor | **İkinci cevap (düplik)** | Teatiyi kapatır |
| Ceza dosyasında mütalaaya yanıt | **Savunma dilekçesi** | Sonuçta beraat/lehe karar talebi |

## 2. Ortak iskelet (etiket + iki nokta hizalı)

```
[... MAHKEMESİ] SAYIN HÂKİMLİĞİNE
                                                                    [İl]

DOSYA NO          : E. [yıl]/[____]            (dava dilekçesinde bulunmaz)
DAVACI            : [Ad Soyad] – TC: [TCKN] – Adres: [adres]
VEKİLİ            : Av. [Ad Soyad] – [Baro] Sicil No: [____] – [adres]
DAVALI            : [Ad Soyad] – TC: [TCKN] – Adres: [adres / mernis notu]
KONU              : [tek cümle]
(DAVA DEĞERİ      : [tutar] TL — yalnızca dava dilekçesinde)
AÇIKLAMALAR       :
HUKUKİ NEDENLER   :
HUKUKİ DELİLLER   :
NETİCE VE TALEP   :
EKLER             :
```

> Yukarıdaki tüm kişi/adres/sicil alanları **YER TUTUCUDUR**. Şablona gerçek ad,
> TCKN, baro, sicil, adres **yazılmaz**; bunlar yalnızca üretim anında kullanıcının
> verdiği bilgilerle doldurulur.

Birden çok taraf varsa `DAVACILAR` / `DAVALILAR` ve altta `1- ... 2- ...`.

## 3. Kalıp ifadeler

- Netice başı: "Yukarıda arz ve izah edilen ve re'sen gözetilecek nedenlerle;"
- Kapanış (çoğul, vekâleten): "... karar verilmesini saygılarımızla vekaleten arz ve talep ederiz."
- Kapanış (tekil): "... saygılarımla vekâleten arz ve talep ederim."
- Delil saklısı: "Karşı tarafın sunacağı delillere karşı delil sunma ve beyanda bulunma hakkımız saklıdır."
- Belirsiz alacak: "(HMK m. 107 uyarınca, fazlaya ilişkin her türlü talep ve dava hakkımız saklı kalmak kaydıyla)".
- Re'sen araştırma: "Sayın Mahkemenizce re'sen gözetilecek hususlar saklı kalmak üzere".

## 4. Üslup kuralları

- Resmî, üçüncü tekil, edilgen ve saygılı dil; "Sayın Mahkeme", "müvekkil", "karşı taraf/davalı".
- TDK yazımı: "hâkim, hâkimliğine, vekâleten, müdafi, def'i" gibi sözcüklerde doğru yazım.
- İddialar madde madde ve başlıklı; her başlık olay → delil → hukuki nitelendirme akışını korur.
- İçtihat: karar metni yığını yapıştırılmaz; kısa atıf + esas alınan ilke bir-iki cümle.
- Abartı ve hakaretten kaçınılır; üslup ölçülü tutulur.

## 5. KVKK ve gizlilik (internet paylaşımına uygun)

- Bu skill ve referansları **hiçbir gerçek kişisel veri içermez**; tüm taraf/vekil
  bilgileri `[KÖŞELİ PARANTEZ]` yer tutucudur.
- Örnek bloklar isimsiz ve varsayımsaldır (gerçek dosya/kişi değil).
- Üretilen dilekçeye yalnızca kullanıcının o an verdiği bilgiler yazılır; başka
  kaynaktan (emsal dilekçe vb.) kişisel veri taşınmaz.
- Davalı adresi bilinmiyorsa "mernis adresine tebligat talep ederiz" notu kullanılır.
- Bilinmeyen her bilgi yer tutucu bırakılır ve kullanıcıya bildirilir.

## 6. Çıktı formatları

Kullanıcı hangisini isterse o üretilir; belirtmezse **docx** varsayılandır. Aynı
gövde dört formatta da kullanılabilir.

### Hizalama (tüm formatlarda ortak — docx / html / udf / pdf)

| Öğe | Hizalama |
|-----|----------|
| Mahkeme başlığı (`... MAHKEMESİ SAYIN HÂKİMLİĞİNE`) ve altındaki il | **ORTALI (center)** |
| Gövde metni (AÇIKLAMALAR, HUKUKİ NEDENLER, DELİLLER, NETİCE metni vb.) | **İki yana yaslı (justify)** |
| Taraf bloğu (DAVACI / VEKİLİ / DAVALI / KONU ...) | Sola yaslı, etiketler hizalı (justify uygulanmaz) |
| Tarih, sıfat + vekil adı ("Davacı/Davalı Vekili / Av. [Ad Soyad]") ve imza | **Sağa yaslı (right)** |

Bu hizalama dört çıktı türünde de aynen korunur.

### docx — `docx` skill
- Times New Roman 12 punto; satır aralığı 1,5.
- Mahkeme başlığı **ortalı** ve kalın; altında il de **ortalı**.
- Gövde paragrafları **iki yana yaslı (justify)**.
- Taraf bloğu etiketleri kalın; **sola yaslı**, etiket–içerik hizalı (kenarlıksız 2 sütunlu tablo veya sekme — bu bloğa justify uygulanmaz).
- Bölüm başlıkları (AÇIKLAMALAR, HUKUKİ NEDENLER, HUKUKİ DELİLLER, NETİCE VE TALEP, EKLER) kalın ve BÜYÜK harf.
- Netice talepleri numaralı liste.
- Altta: tarih, sıfat + vekil adı ("Davacı/Davalı Vekili / Av. [Ad Soyad]") ve imza **sağa yaslı**; ıslak imza için boşluk bırakılır.

### html — tek dosya (standalone)
- Aynı yapı; stil gömülü (`<style>`); harici bağımlılık yok.
- Hizalama CSS ile uygulanır: başlık `text-align:center`, gövde `text-align:justify`, vekil/imza bloğu `text-align:right`.
- Hem doğrudan paylaşılabilir hem de udf üretiminin kaynağıdır.

### udf — `udf` / `udf-cli` skill (UYAP)
- HTML gövde `html2udf` ile `.udf`'e çevrilir; UYAP avukat portalına yüklemeye hazır.
- Okuma gerekiyorsa `udf-cli udf2md` (Read tool .udf okuyamaz; .udf bir ZIP arşividir).

### pdf — `pdf` skill
- docx veya html'den PDF üretilir; yukarıdaki hizalama (başlık ortalı, gövde justify, vekil/imza sağda) korunur; ıslak imza için altta boşluk bırakılır.

### Dosya adı
`[DosyaNo]_[Tür]_[Çerçeve]_[gg_aa_yyyy].<uzantı>`
(örn. `2025-123_Cevap_MIRAT_19_06_2026.docx`)

## 7. Sorumluluk

Üretilen taslağın hukuki sorumluluğu kullanıcıya (avukata) aittir; son kontrol,
mevzuat/içtihat güncelliği ve imza ona aittir. Bu, dilekçe sonunda veya kullanıcıya
sunumda kısaca hatırlatılır.
