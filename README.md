# Öğrenci Gelişim Sistemi · Claude Skill

> **Hızlı başlangıç**
> 1. [Son sürümden](https://github.com/akaytaran/ogrenci-gelisim-sistemi/releases/latest) `ogrenci-gelisim-sistemi.zip` dosyasını indirin.
> 2. Claude'da **Ayarlar > Skills** bölümünden zip'i yükleyin.
> 3. Yeni bir sohbet açıp **"skili kur"** yazın.

Bir öğrencinin ders, sınav, spor, hobi ve günlük yaşamını tek bir sistemde toplayan; aileyle konuşarak **kendi hayatınıza göre** kuran bir Claude skill'i.

"Skili kur" yazarsınız. Claude size öğrenciyi, gününüzü, hedeflerinizi ve nasıl takip etmek istediğinizi sorar. Sonra takvimi bildirimli bloklarla doldurur, bir takip defteri ve yol haritası açar, ders ders mentorluk yapar, aileye raporlar gönderir ve sistemi ayakta tutan otomatik görevleri kurar.

> Bu skill, bir ailenin LGS'ye hazırlanan çocukları için kurduğu sistemden genelleştirildi. Her sınıf düzeyine, spor yapan ya da yapmayan, hobisi olan ya da olmayan her öğrenciye uyarlanacak şekilde yazıldı.

---

## İçindekiler

- [Ne yapar?](#ne-yapar)
- [Kimler için?](#kimler-için)
- [Nasıl çalışır?](#nasıl-çalışır)
- [Kurulunca elinizde ne olur?](#kurulunca-elinizde-ne-olur)
- [Gereksinimler](#gereksinimler)
- [Skill'i yükleme](#skilli-yükleme)
- [İlk kurulum: "skili kur"](#ilk-kurulum-skili-kur)
- [Günlük kullanım](#günlük-kullanım)
- [Yeni dönem, yeni sınıf: güncelleme](#yeni-dönem-yeni-sınıf-güncelleme)
- [İlkeler](#ilkeler)
- [Gizlilik](#gizlilik)
- [Sınırlamalar](#sınırlamalar)
- [Özelleştirme](#özelleştirme)
- [Klasör yapısı](#klasör-yapısı)
- [Sık sorulan sorular](#sık-sorulan-sorular)
- [Katkı ve lisans](#katkı-ve-lisans)

---

## Ne yapar?

- **Görüşerek kurar.** Hazır bir şablon dayatmaz. Okul saatlerinden yatış saatine, antrenman günlerinden hobilere, sınav hedefinden rapor tercihine kadar sorar; bilmediğiniz yerde makul bir varsayılan önerir.
- **Takvimi bildirimli bir yol arkadaşına çevirir.** Her bildirimin başlığı "şimdi ne", açıklaması "nasıl" (kaynak, sıra, soru sayısı, süre) söyler. Öğrenci plan yapmaz; plan hazırdır.
- **Okulla eş zamanlı gider.** Okulun gerçek konusunu takip eder. Bilgi gelmezse makul tahminle ilerler ve bunu açıkça işaretler; sistem asla takılmaz.
- **Ders ders mentorluk yapar.** Test ve deneme fotoğraflarını analiz eder, açıkları kaydeder ve kapatma planı çıkarır, konu anlatır, haftalık özet notlar (PDF) hazırlar.
- **Aileye rapor verir.** Gece raporu, haftalık değerlendirme, yarının programı ve dönemsel durum raporu arasından aile ne isterse onu kurar.
- **Mutluluğu izler.** Öğrencinin günlük enerji/keyif puanını takip eder. Aşırı yükte veliyi uyarır ve yükü azaltır.
- **Kendini öğretir.** Öğrenciye 5 dakikalık bir sistem tanıtımı yapar. Aksama görürse 2 dakikalık bir hatırlatma önerir.
- **Büyür.** Yeni dönemde ya da yeni sınıfta yalnız değişeni sorar ve sistemi günceller.

## Kimler için?

- İlkokuldan liseye her sınıf düzeyi (üniversite öğrencisi kendisi için de kurabilir).
- Büyük sınav yılı (LGS, YKS vb.) ya da sınavsız bir yıl.
- Spor yapan (kulüp, okul takımı) ya da yapmayan öğrenci.
- Hobisi olan (müzik, resim, kodlama…) ya da olmayan öğrenci.
- Telefonu olan ya da bildirimleri velinin cihazından alan öğrenci.
- Yurt dışı değişim/eğitim, burs ya da özel okul gibi başvuru hedefi olan aileler (isteğe bağlı belge arşiviyle).

Sistemi veli, öğrencinin kendisi ya da bir öğretmen/koç kurabilir.

## Nasıl çalışır?

```
0 · Ortam kontrolü   → Hangi araçlar bağlı? Eksik olan için alternatif.
1 · Görüşme          → 10 modül, kısa sorular, varsayılanlar; gerekli dosyaları ister.
2 · Tasarım ve onay  → Yük, günlük akış, hedefler, raporlar. Tek ekranlık plan; onayınız olmadan kurmaz.
3 · Kurulum          → Belgeler, takvim, sayfalar, otomatik görevler, öğretici.
4 · Doğrulama        → 7 günü kontrol eder, bir raporu test eder, size teslim e-postası yollar.
```

Görüşme modülleri: roller ve iletişim · öğrenci profili · gün ve hafta · spor · hobiler · hedefler · kaynaklar · denetim ve rapor tercihleri · beslenme (isteğe bağlı) · hassasiyetler.

Görüşme sırasında istenebilecek dosyalar (hiçbiri zorunlu değil; eksikse sistem varsayılanla kurulur ve "doğrulanmadı" diye işaretler):

- Ders programı (fotoğraf yeter)
- Okulun yıllık planı ya da konu sırası
- Sınav ve deneme takvimi
- Son karne / transkript
- Son deneme ya da test sonuçları
- Antrenman, kurs programı
- Başvuru hedefi varsa sertifikalar ve belgeler

## Kurulunca elinizde ne olur?

| Parça | Ne işe yarar | Kim kullanır |
|---|---|---|
| **Takvim** | Renkli, bildirimli bloklar; her açıklamada ne yapılacağı | Öğrenci (veli görevleri veliye davet olarak) |
| **Takip Defteri** | Durum panosu, günlük kayıt, açık haritası, testler, spor, program bilgisi, raporlar | Aile + sistem |
| **Yol Haritası** | Hedefler, kilometre taşları, okul/kurum listesi, tahmin bantları | Aile |
| **Öğrenci Rehberi** | "Başlarken", rapor nasıl verilir, takıldığında ne yazılır | Öğrenci |
| **Dosya Kutusu** | Öğrenciye hazırlanan özet notlar ve testler; indirildi mi takibi | Öğrenci |
| **Belge Arşivi** (isteğe bağlı) | Karne, sertifika, sınav sonucu; başvuru gereksinimleri | Aile |
| **Otomatik görevler** | Gece raporu, haftalık planlayıcı, özet notlar, değerlendirmeler, hatırlatmalar | Arka planda (bulutta) |

## Gereksinimler

Skill, bulunduğu ortamdaki araçlara göre kendini ayarlar. En iyi deneyim için:

| Araç | Ne için | Yoksa |
|---|---|---|
| Skill destekleyen bir Claude ortamı (Claude uygulaması / Cowork, ya da Claude Code) | Skill'i çalıştırmak | — |
| Google Calendar bağlayıcısı | Bildirimli takvim | .ics dosyası ya da takvim belgesi |
| Gmail bağlayıcısı | Raporlar | Raporlar belgeye yazılır |
| Claude Docs (sekmeli belgeler) | Takip Defteri, Yol Haritası, Rehber | Google Docs / Notion bağlayıcısı ya da markdown dosyaları |
| Yayınlanan sayfalar (Artifacts; veritabanı ve dosya deposu) | Dosya Kutusu, Belge Arşivi | Bulut klasörü ya da sohbette dosya |
| Bulutta zamanlanmış görevler | Raporlar ve planlayıcı bilgisayar kapalıyken de çalışsın | Haftalık elle çalıştırılacak komut listesi |

Bu araçların hangi planlarda ve hangi uygulamalarda bulunduğu zamanla değişebilir; güncel bilgi için Claude'un yardım sayfalarına bakın.

## Skill'i yükleme

1. Bu depodaki `ogrenci-gelisim-sistemi` klasörünü zip'leyin (ya da Releases'tan hazır zip'i indirin). Zip'in içinde doğrudan `SKILL.md` ve `references/`, `assets/` klasörleri olmalı.
2. **Claude uygulaması:** Ayarlar'daki Skills (Yetenekler) bölümünden zip'i yükleyin. Menü adları sürüme göre değişebilir.
3. **Claude Code:** Klasörü `~/.claude/skills/ogrenci-gelisim-sistemi/` altına kopyalayın.
4. Takvim, e-posta ve belge bağlayıcılarınızı bağlayın (yukarıdaki tablo).

## İlk kurulum: "skili kur"

Yeni bir sohbet açın ve yazın:

```
skili kur
```

Örnek akış:

```
Claude: Önce hangi araçların bağlı olduğuna bakayım... Takvim ✓, e-posta ✓, belgeler ✓,
        otomatik görevler ✓. Her şey hazır. Birkaç soruyla başlayalım:
        1) Sistemi kim kuruyor: veli, öğrenci, öğretmen?
        2) Öğrencinin adı (ya da takma ad)?
        3) Bildirimleri hangi takvim hesabından alacak?
Siz:    Veliyim. Deniz. Kendi telefonundaki deniz@... hesabı.
Claude: ...
```

Kurulum genelde 20–40 dakika sürer (çoğu sorulara cevap vermek). Sonunda size bir teslim e-postası gelir: ne kuruldu, bağlantılar, sizin yapacaklarınız (davetleri kabul etmek, öğrencinin telefonunda takvim bildirimlerini açmak).

İlk akşam öğrencinin takviminde 15 dakikalık bir "Sistemle tanışma" etkinliği olur. Öğrenci Claude'a "sistemi tanıt" yazınca kısa bir tanıtım başlar.

## Günlük kullanım

**Öğrenci yazar:**

| Yazdığı | Ne olur |
|---|---|
| `günlük rapor` | Günün görevleri listelenir; "1 tamam, 2 yarım çünkü…" diye tek mesajla cevaplar |
| Test fotoğrafı + `analiz et` | Ders mentoru yanlışları sınıflar, açıkları kaydeder, kısa geri bildirim verir |
| Soru fotoğrafı + `anlamadım` | Konu anlatımı, çözümlü örnek, 3 benzer soru |
| `bugün ne yapıyorum?` | Bugünün listesi |
| `yorgunum, bugün hafif olsun` | Yük hafifler; telafi uykudan yemez |
| `sistemi tanıt` | 5 dakikalık tanıtım |

**Veli yazar:**

| Yazdığı | Ne olur |
|---|---|
| `nasıl gidiyor?` | Kısa durum özeti |
| `okulda bu hafta şu konular işlendi: …` | Müfredat senkronu güncellenir |
| `programı güncelle: antrenman Çarşamba'ya kaydı` | Yalnız değişen kısım güncellenir |
| Karne / sertifika fotoğrafı | Belge arşivine işlenir, önemli veri panoya yazılır |
| `koç evde kuvvet çalışmasına onay verdi` | Ev rutini güncellenir |

## Yeni dönem, yeni sınıf: güncelleme

```
yeni dönem başladı, yeni ders programı ekte
```
ya da
```
sınıf atladı, 9. sınıfa göre sistemi güncelle
```

Skill, Takip Defteri'ndeki "Sistem Kimliği" bölümünden mevcut kurulumu bulur, yalnız değişeni sorar, geçmişi arşivler, takvimi ve otomatik görevleri yeniler.

## İlkeler

Sistemin karakterini belirleyen kurallar (`references/ilkeler.md`):

- **Öğrenci boğulmaz.** Uyku, serbest zaman ve eve varış sonrası dinlenme korunur.
- **Robot değiliz.** Uyum hedefi %100 değil, ~%80. Aksama suçlanmaz; sistem ayarlanır.
- **Sistem takılmaz.** Bilgi gelmezse tahminle ilerler, işaretler, sonra kendini düzeltir.
- **Ton:** takım arkadaşı gibi; kıyaslama, korkutma, "neden yapmadın" yok.
- **Sağlık:** teşhis yok; kilo/diyet öğrenciyle konuşulmaz; kuvvet çalışması koç onayıyla.
- **Dürüstlük:** tahminler aralıkla verilir; sınav bilgileri her seferinde güncel kaynaktan doğrulanır.

## Gizlilik

- Öğretmenlere yalnız akademik bilgi gider. Aile notları, ruh hali ve sağlık bilgisi asla gitmez. Öğretmenlere e-posta ancak aile adresleri verip istedikten sonra gönderilir.
- Kişisel belgeler e-postaya eklenmez; arşiv sayfasında durur.
- Veriler sizin hesabınızdaki belgelerde, takvimde ve sayfalarda durur. Öğrencinin hesabındaki belgeleri öğrencinin de görebileceğini unutmayın; sistem hassas notları buna göre yazar.
- Bu depo hiçbir gerçek öğrenci verisi içermez; örnekler kurgusaldır.

## Sınırlamalar

- **E-posta ekleri:** Claude büyük dosyaları e-postaya güvenilir şekilde ekleyemeyebilir. Bu yüzden içerik e-postanın gövdesinde gelir, dosya Dosya Kutusu'nda durur.
- **Araç bağımlılığı:** Bağlayıcı ya da zamanlanmış görev desteği olmayan ortamlarda sistem daha sade kurulur (bkz. Gereksinimler).
- **Tahminler garanti değildir.** Puan/sonuç tahminleri aralıktır ve ilk verilerle güncellenir.
- **Tavsiye sınırı:** Tıbbi, psikolojik, hukuki ya da göçmenlik tavsiyesi vermez; ilgili uzmana yönlendirir.
- **Resmi bilgiler değişir:** Sınav tarihleri, formatlar ve taban puanlar her kurulumda web'den doğrulanır; yine de resmi kaynağı kontrol edin.

## Özelleştirme

- **İlkeler:** `references/ilkeler.md` içindeki "robot değiliz" metnini kendi aile mesajınızla değiştirebilirsiniz (kurulumda da sorulur).
- **Yük tablosu:** `references/yuk-ve-ritim.md` başlangıç sürelerini içerir; kendi deneyiminize göre değiştirin.
- **Yeni sınav sistemi:** `references/sinav-sistemleri.md` dosyasına ekleyin (ne aranacağını yazın; rakamları sabitlemeyin).
- **Otomatik görevler:** `references/zamanlanmis-gorevler.md` şablonlarını düzenleyin ya da yenilerini ekleyin.
- **Sayfa şablonları:** `assets/` altındaki HTML dosyaları; `{{...}}` alanları kurulumda doldurulur.

## Klasör yapısı

```
ogrenci-gelisim-sistemi/
├── SKILL.md                       # Sihirbazın ana talimatı (modlar, adımlar)
├── references/
│   ├── ilkeler.md                 # Ton, sağlık, gizlilik, "robot değiliz"
│   ├── gorusme-sorulari.md        # 10 modüllük soru bankası + dosya talebi
│   ├── yuk-ve-ritim.md            # Sınıfa göre süre, uyku, günlük akış
│   ├── sinav-sistemleri.md        # LGS, YKS ve uluslararası sınavlar (doğrulama rehberi)
│   ├── hedefler.md                # Hedef yazma, yol haritası, tahmin bantları
│   ├── takip-defteri.md           # Belge yapıları ve tablo şemaları
│   ├── takvim.md                  # Takvim kuralları, etiketler, veli görevleri
│   ├── zamanlanmis-gorevler.md    # Otomatik görev şablonları
│   ├── mentorlar.md               # Ders mentorları, test analizi, müfredat senkronu
│   ├── isletim.md                 # Kurulum sonrası günlük işletim
│   ├── ogretici.md                # Öğrenciye sistem tanıtımı ve tekrar
│   └── ornek-kurulumlar.md        # İki kurgusal örnek
└── assets/
    ├── dosya-kutusu.html          # Dosya Kutusu sayfa şablonu
    └── belge-arsivi.html          # Belge Arşivi sayfa şablonu
```

## Sık sorulan sorular

**Bilgisayarımın açık kalması gerekiyor mu?**
Hayır. Otomatik görevler bulutta çalışacak şekilde kurulur. Ortamınız bulut görevlerini desteklemiyorsa skill bunu söyler ve alternatif önerir.

**Çocuğumun telefonu yok, olur mu?**
Olur. Bildirimler velinin takvimine kurulur, günlük rapor birlikte verilir.

**Her şeyi kurmak zorunda mıyım?**
Hayır. Raporları, özet notları ve öğün bildirimlerini siz seçersiniz. Az ve işe yarar olanı önerilir.

**Sistem yanlış konuyu çalıştırırsa?**
Tek cümleyle düzeltirsiniz ("okulda şu an X işleniyor"). Sistem o haftanın içeriğini tekrara çevirir ve doğru konudan devam eder.

**Öğretmenimizle paylaşabilir miyim?**
Evet. Dönemsel bir akademik rapor (yalnız akademik bilgi) hazırlanabilir; isterseniz siz iletirsiniz.

**Başka bir ülkenin eğitim sisteminde çalışır mı?**
Evet. Sınav ve müfredat bilgisi kurulumda web'den doğrulanır. Türkiye dışı sistemler için `sinav-sistemleri.md` yalnızca bir başlangıç rehberidir.

## Katkı ve lisans

Bu depo kod katkısına (pull request) kapalıdır; gelen PR'lar kapatılır. Hata bildirimi ve önerileriniz için [Issues](https://github.com/akaytaran/ogrenci-gelisim-sistemi/issues) bölümünü kullanabilirsiniz. Lütfen gerçek öğrenci verisi içeren hiçbir şey göndermeyin.

Lisans: MIT © 2026 Ali Tutku Kaytaran. Ayrıntılar için LICENSE dosyasına bakın.
